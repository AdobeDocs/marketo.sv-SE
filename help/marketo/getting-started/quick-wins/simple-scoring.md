---
unique-page-id: 2359414
description: Enkel poängsättning - Marketo Docs - produktdokumentation
title: Enkel poängsättning
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Enkel poängsättning {#simple-scoring}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Steg 1: Skapa en resultatkampanj {#step-create-a-scoring-campaign}

1. Gå till **[!UICONTROL Marketing Activities]** område.

   ![](assets/simple-scoring-1.png)

1. Högerklicka på **Utbildning** mapp och klicka på **[!UICONTROL New Campaign Folder]**.

   ![](assets/simple-scoring-2.png)

1. Namnge kampanjmappen Scoring och klicka på **[!UICONTROL Create]**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Om du redan har en bedömningsmapp ger du den ett annat namn, till exempel Betygsättning 1. Mappnamn måste vara unika.

1. Högerklicka på **Poäng** mapp och markera **[!UICONTROL New Smart Campaign]**.

   ![](assets/simple-scoring-4.png)

1. Namnge kampanjen&quot;Change Score&quot; och klicka på **[!UICONTROL Create]**.

   ![](assets/simple-scoring-5.png)

1. Klicka på **[!UICONTROL Smart List]** -fliken.

   ![](assets/simple-scoring-6.png)

   Vi vill att den här kampanjen ska köras när en person fyller i din **Formulär för testbegäran**.

1. Sök och dra **[!UICONTROL Fills Out Form]** till vänster på arbetsytan.

   ![](assets/simple-scoring-7.png)

1. Välj **Mitt formulär**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Om du har slutfört [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} snabbt vinna, du borde ha formuläret. Om du har använt ett annat namn för formuläret väljer du det.

1. Klicka på **[!UICONTROL Flow]** -fliken.

   ![](assets/simple-scoring-9.png)

1. Dra **Ändra poäng** flöda åtgärd till den vänstra arbetsytan.

   ![](assets/simple-scoring-10.png)

1. Du kan skriva vilket värde som helst som ska läggas till i personens poäng. Vi skriver &quot;+5&quot; i **[!UICONTROL Change]** fält.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Bra poängsättningskampanjer är avgörande för att leverera högkvalitativa säljare. Läs [**The Definitive Guide to Lead Scoring**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}.

1. Klicka på **[!UICONTROL Schedule]** -fliken och **[!UICONTROL Activate]** -knappen.

   ![](assets/simple-scoring-12.png)

1. Klicka **[!UICONTROL Activate]** på bekräftelseskärmen.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>När kampanjen är aktiv körs den varje gång en person fyller i formuläret. Kampanjen fortsätter att löpa tills den har inaktiverats.

## Steg 2: Fyll i formuläret {#step-fill-out-the-form}

1. Välj den landningssida du skapade i dialogrutan [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} snabbvinn.

   ![](assets/simple-scoring-14.png)

1. Klicka på **[!UICONTROL Preview]**. Landningssidan öppnas på en ny flik.

   ![](assets/simple-scoring-15.png)

1. Fyll i formuläret med ditt förnamn, efternamn och e-postadress och klicka sedan på **[!UICONTROL Submit]**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Använd samma namn och e-postadress som du använde när du först angav dig själv som en person för att tillämpa poängökningen &quot;+5&quot;.

## Steg 3: Visa personinformation {#step-view-the-person-info}

1. Gå till **[!UICONTROL Database]** område.

   ![](assets/simple-scoring-17.png)

1. Sök efter den e-postadress som du använde när du fyllde i formuläret.

   ![](assets/simple-scoring-18.png)

1. Dubbelklicka på personen.

   ![](assets/simple-scoring-19.png)

Personuppgifterna öppnas på en ny flik eller i ett nytt fönster. Se hur poängen ökade med 5 poäng för att fylla i blanketten?

![](assets/simple-scoring-20.png)

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 2: Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Uppdrag 4: Automatiskt svar via e-post ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
