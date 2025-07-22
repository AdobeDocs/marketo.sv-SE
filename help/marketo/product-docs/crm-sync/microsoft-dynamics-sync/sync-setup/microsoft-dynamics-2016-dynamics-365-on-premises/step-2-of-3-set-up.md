---
description: Installera Marketo för [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premises Step 2 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för  [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premises Step 2 of 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 1%

---

# Steg 2 av 3 Konfigurera Marketo för [!DNL Dynamics] (2016 On-Prem/[!DNL Dynamics] 365 On-Premises){#step-of-set-up-for-marketo-on-premises-2016}

Utmärkt jobb med att slutföra föregående steg. Vi går igenom det här.

>[!PREREQUISITES]
>
>[Installera Marketo för [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premises Steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Skapa en ny användare {#create-a-new-user}

1. Logga in på [!DNL Dynamics]. Klicka på ikonen Inställningar och välj Avancerade inställningar.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Klicka på **[!UICONTROL Settings]** och välj **[!UICONTROL Security]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Klicka på **[!UICONTROL Add and License Users]**. En ny flik ska öppnas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Klicka på **[!UICONTROL Admin]** överst på sidan. En annan ny flik bör öppnas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Klicka på **[!UICONTROL Add a user]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Ange all information. När du är klar klickar du på **[!UICONTROL Add]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Det här namnet måste vara en dedikerad synkroniseringsanvändare och inte en befintlig CRM-användares konto. Det behöver inte vara en faktisk e-postadress.

1. Ange e-postadressen som ska ta emot inloggningsuppgifterna och klicka på Skicka e-post och stäng.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Skapa ett nytt klientprogram {#create-a-new-client-application}

Följ stegen i [den här Microsoft-artikeln](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) för att skapa ett nytt klientprogram och bevilja behörigheter. Observera klient-ID/hemlighet för klientprogrammet [!DNL Dynamics].

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller för Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar din Marketo finns i [Uppgradera Marketo-lösningen för [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för synkroniseringsanvändaren [ ska anges till engelska](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Security]**.

   ![](assets/assign1.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/assign2.png)

1. En lista över användare visas här. Välj den dedikerade Marketo Sync-användaren eller kontakta din [ADFS-administratör (Active Directory Federation Services)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} för att skapa en dedikerad användare för Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/assign4.png)

1. Markera Marketo Sync User och klicka på **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) och importerar lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare _synkroniseras inte_ tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicerar du Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} eller försöker logga ut och sedan in igen.

1. Klicka på **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Klicka på fältet **[!UICONTROL Marketo User]** och välj synkroniseringsanvändare.

   ![](assets/configure3.png)

1. Klicka på ikonen Spara längst ned till höger.

   ![](assets/configure4.png)

1. Klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar konfigurerar [ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Verifiera [!DNL Microsoft Dynamics] synkroniseringsprocessen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i [!DNL Microsoft Dynamics] CRM.

>[!MORELIKETHIS]
>
>[Installera Marketo för [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premises Steg 3 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
