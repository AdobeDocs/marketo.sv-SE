---
unique-page-id: 7504739
description: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3 - Marketo Docs - Produktdokumentation
title: Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 2 of 3
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Steg 2 av 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

Utmärkt jobb med att slutföra föregående steg. Vi går igenom det här.

>[!PREREQUISITES]
>
>* [Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 1 of 3](step-1-of-3-install.md)

>



## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo-synkroniseringsanvändarrollen till Marketför att synkronisera användare. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar din marknadsföring finns i [Uppgradera Marketo-lösningen för Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Under **Inställningar** klickar du på **Säkerhet**.

   ![](assets/assign1.png)

1. Klicka på **Användare**.

   ![](assets/assign2.png)

1. En lista över användare visas här. Markera den dedikerade Marketo-synkroniseringsanvändaren eller kontakta din [ADFS-administratör (Active Directory Federation Services)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) för att skapa en dedikerad användare för Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka på **Hantera roller**.

   ![](assets/assign4.png)

   Markera Marketo Sync User och klicka på OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](step-1-of-3-install.md) och importerar lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Sync User kommer **inte** att synkroniseras tillbaka till Marketo.

## Konfigurera Marketo-lösning {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Under **Inställningar** klickar du på **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår kan du [publicera Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) eller försöka logga ut och in igen.

1. Klicka på **Standard**.

   ![](assets/configure2.png)

1. Klicka på fältet **Marketo User** och välj synkroniseringsanvändare.

   ![](assets/configure3.png)

1. Klicka på ikonen Spara längst ned till höger.

   ![](assets/configure4.png)

1. Klicka på **Publicera alla anpassningar**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar [skapar du ett anpassat synkroniseringsfilter](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Verifiera Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)-processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Installera Marketo för Dynamics 2015 On-Prem och 2016 365 On-Prem Step 3 of 3](step-3-of-3-connect.md)
