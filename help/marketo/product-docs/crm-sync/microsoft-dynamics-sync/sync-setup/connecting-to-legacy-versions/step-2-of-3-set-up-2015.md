---
unique-page-id: 7504739
description: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 2 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 2 of 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Steg 2 av 3 Konfigurera Marketo för Dynamics (lokal version 2015){#step-of-set-up-for-marketo-on-premises-2015}

Utmärkt jobb med att slutföra föregående steg. Vi går igenom det här.

>[!PREREQUISITES]
>
>[Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

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

   >[!IMPORTANT]
   >
   >Synkroniseringsanvändaren bör ha läsbehörighet för Marketo Config.

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} och importera lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare kommer att _not_ synkas tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Under **[!UICONTROL Settings]**, klicka **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} eller prova att logga ut och in igen.

1. Klicka på **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Klicka på **[!UICONTROL Marketo User]** och välj synkroniseringsanvändare.

   ![](assets/configure3.png)

1. Klicka på ikonen Spara längst ned till höger.

   ![](assets/configure4.png)

1. Klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >Synkroniseringsanvändaren bör ha läsbehörighet för Marketo Config.

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installera Marketo för Microsoft Dynamics 2015 On-Premises Step 3 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
