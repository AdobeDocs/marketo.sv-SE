---
unique-page-id: 9437903
description: Skapa ett anpassat  [!DNL Dynamics] synkroniseringsfilter - Marketo Docs - produktdokumentation
title: Skapa ett anpassat  [!DNL Dynamics] synkroniseringsfilter
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Skapa ett anpassat [!DNL Dynamics]-synkroniseringsfilter {#create-a-custom-dynamics-sync-filter}

Med Marketo kan du konfigurera ett synkroniseringsfilter och bara synkronisera en del av dina poster.

## Översikt {#overview}

Så här konfigurerar du ett [!DNL Dynamics]-synkroniseringsfilter:

1. Skapa ett anpassat fält med två alternativ (booleskt) med namnet `new_synctomkto` i Dynamics CRM för alla objekt (lead, kontakt, konto, affärsmöjlighet och andra anpassade entiteter).
1. Tilldela det här fältet värdet Ja/Nej.

Du måste göra dessa ändringar i Dynamics CRM, inte i databasen eller Marketo.

>[!CAUTION]
>
>Om du inte tilldelar fältet och låter det vara tomt/NULL synkroniseras det ned, men uppdateras inte. Poster med fältvärdet blank/NULL i Dynamics CRM visar fältvärdet i Marketo som &quot;false&quot;.

Marketo letar efter det här fältet under den automatiska bakgrundssynkroniseringen och avgör vilka poster som ska synkroniseras över baserat på den här logiken:

| Fältvärde | Vill du synkronisera med Marketo? |
|---|---|
| Fältet finns inte | Ja |
| Fältet är tomt | Ja |
| Fältet har värdet Ja | Ja |
| Fältet har värdet Nej | Nej |

>[!CAUTION]
>
>Det enda sättet att tala om för Marketo att hoppa över en post är att explicit ange fältvärdet till **Nej**. Marketo synkroniserar fortfarande poster över även om fältvärdena är tomma.

>[!PREREQUISITES]
>
>Installera den senaste versionen av Marketo-plugin-programmet (3.0.0.1 eller senare). Gå till Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Download Marketo Solution].

## Skapa SyncToMkto-fält {#create-synctomkto-field}

1. Logga in i Dynamics CRM. Klicka på **Inställningar** och sedan på **Anpassningar**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Klicka på **[!UICONTROL Customize the System]**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Klicka på ![](assets/image2015-8-10-21-3a44-3a23.png) bredvid **[!UICONTROL Entities]**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Klicka på ![](assets/image2015-8-10-21-3a44-3a23.png) bredvid **[!UICONTROL Lead]** och välj **[!UICONTROL Fields]**. Klicka sedan på **[!UICONTROL New]**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Ange **SyncToMkto** i fältet **[!UICONTROL Display Name]** och välj **[!UICONTROL Two Options]** som **[!UICONTROL Data Type]**. Klicka sedan på **[!UICONTROL Save and Close]**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Välj ett visningsnamn för det här fältet, men fältet Namn måste vara exakt **new_synctomkto**. Du måste använda **new** som standardprefix. Om du har ändrat standardvärdet går du hit för att [återställa standardprefixet för de anpassade fältnamnen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Du kan ändra tillbaka när du har skapat de nya fälten.

   >[!NOTE]
   >
   >Om du har konfigurerat ett asynkront arbetsflöde får posten det standardvärde för SyncToMkto som du har konfigurerat i fältet och det korrekta värdet hämtas några sekunder senare när arbetsflödet har slutförts. Om standardvärdet är Ja skapas posterna i Marketo och blir sedan inaktuella. Använd **Nej** som standardvärde för att undvika detta.

1. Upprepa den här processen och skapa fältet **SyncToMkto** för andra entiteter som du vill begränsa synkroniseringen för, till exempel kontakter, konto, affärsmöjlighet och anpassade entiteter.

## Markera filtret i Marketo {#select-the-filter-in-marketo}

Även om du redan har gjort den första synkroniseringen går du in och väljer fälten som ska synkroniseras med Marketo.

1. Gå till Admin och välj **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **[!UICONTROL Edit]** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Bra, nu har du aktiverat synkroniseringsfiltret för Marketo.

## Skapa ett [!DNL Dynamics]-arbetsflöde för att tilldela synkroniseringsfiltervärden automatiskt {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Du kan alltid manuellt tilldela ett värde till SyncToMkto-fälten för dina poster. Men varför inte utnyttja kraften i ett [!DNL Dynamics]-arbetsflöde och automatiskt tilldela ett värde till SyncToMkto-fältet när en post skapas eller uppdateras?

>[!NOTE]
>
>Du kan inte göra detta på databasnivå. Det måste göras manuellt i CRM eller med hjälp av ett arbetsflöde.
>
>Ett [!DNL Dynamics]-arbetsflöde fungerar bara på nya poster som skapas framåt, inte på historiska data. Använd en batchuppdatering för att flytta över befintliga poster.

1. Gå till Dynamics CRM. Klicka på **Inställningar** och sedan på **Processer**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Ange ett namn för arbetsflödet och välj **[!UICONTROL Workflow]** som [!UICONTROL Category] och **[!UICONTROL Lead]** som [!UICONTROL Entity]. Klicka sedan på **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Skapa regler för att tilldela ett sant eller falskt värde till fältet **SyncToMkto** baserat på din organisations önskemål. Klicka på **[!UICONTROL Save and Close]**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definiera en standardåtgärd när du har klickat på **[!UICONTROL Add Step]** för att lägga till ett kontrollvillkor. Detta anger de poster som du inte vill synkronisera till **Nej**. Annars synkroniseras de.

1. Markera arbetsflödet och klicka på **[!UICONTROL Activate]**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Se [Anpassade synkroniseringsfilterregler för en e-postadress](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} om du vill konfigurera regler för att synkronisera endast poster för personer med e-postadresser.

## Information om synkroniseringsfilter {#sync-filter-details}

Här är några implementeringsdetaljer vi trodde att du borde veta:

* Starta en synkroniseringsåtgärd

  När värdet **SyncToMkto** ändras från **No** till **Yes** meddelar [!DNL Dynamics] Marketo omedelbart att synkronisera den här posten. Om posten redan finns uppdaterar Marketo den. Annars skapar Marketo posten.

* Stoppa en synkroniseringsåtgärd

  När en post ändrar sitt SyncToMkto-värde från Ja till Nej, meddelas Marketo om att den här posten inte ska synkroniseras. Posten tas dock inte bort, utan den slutar att hämta uppdateringar och blir föråldrad.

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics Sync-filter: Kvalificera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Microsoft Dynamics Sync-filter: Sammanfoga](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Anpassade synkroniseringsfilterregler för en e-postadress](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
