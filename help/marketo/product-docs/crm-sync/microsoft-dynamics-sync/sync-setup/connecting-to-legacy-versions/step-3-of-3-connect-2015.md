---
unique-page-id: 7504744
description: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 3 of 3 - Marketo Docs - Product Documentation
title: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 3 of 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# Steg 3 av 3: Anslut Marketo [!DNL Dynamics] (2015 On-Prem) {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [Installera Marketo för [!DNL Microsoft Dynamics] 2015 On-Premises, steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)
>* [Installera Marketo för [!DNL Microsoft Dynamics] 2015 On-Premises, steg 2 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Ange [!DNL Dynamics] synkroniseringsanvändarinformation {#enter-dynamics-sync-user-information}

1. Logga in på Marketo och klicka på **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Klicka på **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Välj **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Step 1: Enter Credentials]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Kontrollera att dina autentiseringsuppgifter är korrekta eftersom det inte går att återställa efterföljande schemaändringar efter överföringen. Om felaktiga uppgifter sparas måste du skaffa en ny Marketo-prenumeration.

1. Ange **[!UICONTROL Username]**, **[!UICONTROL Password]** a [!DNL Microsoft Dynamics] **URL** och en **[!UICONTROL Client Id]/[!UICONTROL Client Secret]**. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Om din Marketo etablerades före oktober 2020 är klient-ID och hemlighet valfria fält. Annars är de obligatoriska. Hur du får den här informationen beror på vilken version av MSD du använder.
   >* Användarnamnet i Marketo måste matcha användarnamnet för synkroniseringsanvändaren i CRM. Formatet kan vara `user@domain.com` eller DOMÄN\användare.
   >* Om du inte känner till URL:en kan du [lära dig att hitta den här](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Vet du inte URL:en? Vi visar dig hur du hittar din [Dynamics-organisationstjänsts URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"} här.

## Markera fält som ska synkroniseras {#select-fields-to-sync}

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Step 2: Select Fields to Sync]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Markera de fält som du vill synkronisera till Marketo så att de är förmarkerade. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo lagrar en referens till de fält som ska synkroniseras. Om du tar bort ett fält i [!DNL Dynamics] rekommenderar vi att du gör det med [synkroniseringen inaktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Uppdatera sedan schemat i Marketo genom att redigera och spara [[!UICONTROL Select Fields to Sync]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synkronisera fält för ett eget filter {#sync-fields-for-a-custom-filter}

Om du har skapat ett eget filter måste du gå in och välja de nya fält som ska synkroniseras med Marketo.

1. Gå till [!UICONTROL Admin] och välj **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicka på **[!UICONTROL Edit]** på [!UICONTROL Field Sync Details].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Rulla ned till fältet och kontrollera det. Det faktiska namnet måste vara new_synctomkto, men visningsnamnet kan vara vad som helst. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **[!UICONTROL Edit]** i **[!UICONTROL Step 3: Enable Sync]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en [!DNL Microsoft Dynamics]-synkronisering eller när du anger personer manuellt.

1. Läs allt i popup-fönstret, ange din e-postadress och klicka på **[!UICONTROL Start Sync]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Beroende på antalet poster kan den inledande synkroniseringen ta från några timmar till några dagar var som helst. Du får ett e-postmeddelande när du är klar.

   ![](assets/image2015-3-16-9-59-51.png)
