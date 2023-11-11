---
description: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 2%

---

# Steg 2 av 3 Konfigurera Marketo för Dynamics (On-Prem/Dynamics 365 On-Premises 2016){#step-of-set-up-for-marketo-on-premises-2016}

Utmärkt jobb med att slutföra föregående steg. Vi går igenom det här.

>[!PREREQUISITES]
>
>[Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## Skapa en ny användare {#create-a-new-user}

1. Logga in i Dynamics. Klicka på ikonen Inställningar och välj Avancerade inställningar.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Klicka på **[!UICONTROL Settings]** och välj **[!UICONTROL Security]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Klicka på **[!UICONTROL Add and License Users]**. En ny flik ska öppnas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Klicka **[!UICONTROL Admin]** överst på sidan. En annan ny flik bör öppnas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Klicka på **[!UICONTROL Add a user]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Ange all information. När du är klar klickar du **[!UICONTROL Add]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Det här namnet måste vara en dedikerad synkroniseringsanvändare och inte en befintlig CRM-användares konto. Det behöver inte vara en faktisk e-postadress.

1. Ange e-postadressen som ska ta emot inloggningsuppgifterna och klicka på Skicka e-post och stäng.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Skapa ett nytt klientprogram {#create-a-new-client-application}

Följ stegen i [den här Microsoft-artikeln](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} för att skapa ett nytt klientprogram och bevilja behörigheter. Observera klient-ID/hemlighet för Dynamics-klientprogrammet.

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Om du vill uppgradera din Marketo går du till [Uppgradera Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Språkinställningen för Synkronisera användare [ska anges till engelska](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Under **[!UICONTROL Settings]**, klicka **[!UICONTROL Security]**.

   ![](assets/assign1.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/assign2.png)

1. En lista över användare visas här. Välj en dedikerad Marketo Sync-användare eller kontakta din [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS)-administratör för att skapa en dedikerad användare för Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/assign4.png)

1. Markera Marketo Sync User och klicka på **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) och importera lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare kommer att _not_ synkas tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Under **[!UICONTROL Settings]**, klicka **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} eller prova att logga ut och in igen.

1. Klicka på **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Klicka på **[!UICONTROL Marketo User]** och välj synkroniseringsanvändare.

   ![](assets/configure3.png)

1. Klicka på ikonen Spara längst ned till höger.

   ![](assets/configure4.png)

1. Klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 3 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
