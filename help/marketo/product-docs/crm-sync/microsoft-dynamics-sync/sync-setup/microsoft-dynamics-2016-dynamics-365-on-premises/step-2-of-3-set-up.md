---
unique-page-id: 7504739
description: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3 - Marketo Docs - produktdokumentation
title: Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 1e20fdd1d3c6bba265ceabe499e0d7a4babf4ef1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Steg 2 av 3 Konfigurera Marketo för Dynamics (On-Prem/Dynamics 365 On-Premises 2016){#step-of-set-up-for-marketo-on-premises-2016}

Utmärkt jobb med att slutföra föregående steg. Vi går igenom det här.

>[!PREREQUISITES]
>
>[Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Om du vill uppgradera din Marketo går du till [Uppgradera Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för Synkronisera användare [ska anges till engelska](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Under **Inställningar**, klicka **Säkerhet**.

   ![](assets/assign1.png)

1. Klicka **Användare**.

   ![](assets/assign2.png)

1. En lista över användare visas här. Välj en dedikerad Marketo Sync-användare eller kontakta din [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)-administratör för att skapa en dedikerad användare för Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka **Hantera roller**.

   ![](assets/assign4.png)

   Markera Marketo Sync User och klicka på OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) och importera lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare kommer att **not** synkas tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Under **Inställningar**, klicka **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicera Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) eller prova att logga ut och in igen.

1. Klicka **Standard**.

   ![](assets/configure2.png)

1. Klicka på **Marketo-användare** och välj synkroniseringsanvändare.

   ![](assets/configure3.png)

1. Klicka på ikonen Spara längst ned till höger.

   ![](assets/configure4.png)

1. Klicka **Publicera alla anpassningar**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar, [konfigurera ett eget synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) -processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installera Marketo för Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 3 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
