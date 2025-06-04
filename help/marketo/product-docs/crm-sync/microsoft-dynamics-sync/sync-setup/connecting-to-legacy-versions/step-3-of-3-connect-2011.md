---
unique-page-id: 3571809
description: Steg 3 av 3 - Ansluta Microsoft Dynamics med Marketo (On-Premises 2011) - Marketo Docs - produktdokumentation
title: Steg 3 av 3 - Ansluta Microsoft Dynamics med Marketo (lokal version 2011)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Steg 3 av 3: Anslut Microsoft Dynamics till Marketo (lokal version 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Okej! Vi installerade lösningen och konfigurerade synkroniseringsanvändaren. Därefter måste vi koppla Marketo och Dynamics.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Installera Marketo Solution (2011 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}
>* [Steg 2 av 3: Konfigurera Marketo Sync-användare i Dynamics (lokal version 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange användarinformation för Dynamics Sync {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicka på **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Klicka på **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Enter Credentials]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga uppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **[!UICONTROL Username]**, **[!UICONTROL Password]** och CRM **[!UICONTROL URL]** och klicka sedan på **[!UICONTROL Save]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara `user@domain.com` eller DOMÄN\användare.
   >* Om du inte känner till URL:en kan du [lära dig att hitta den här](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

Nu måste vi markera de fält vi vill synkronisera.

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Select Fields to Sync]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Det finns förmarkerade fält som kommer att synkroniseras. Lägg till mer om du vill och klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo lagrar en referens till de fält som ska synkroniseras. Om du tar bort ett fält i Dynamics rekommenderar vi att du gör det med [synkroniseringen inaktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Uppdatera sedan schemat i Marketo genom att redigera och spara [Markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till Admin och välj **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **[!UICONTROL Edit]** i Fältsynkroniseringsinformation.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Microsoft Dynamics-synkronisering eller när du anger personer eller leads manuellt.

1. Läs allt i popup-fönstret, ange din e-postadress och klicka på **[!UICONTROL Start Sync]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Beroende på antalet poster kan den inledande synkroniseringen ta från några timmar till några dagar var som helst. Du får ett e-postmeddelande när du är klar.

   ![](assets/image2014-12-11-11-3a55-3a15.png)
