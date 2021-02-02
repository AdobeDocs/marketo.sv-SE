---
unique-page-id: 3571807
description: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics (On-Premises 2011) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics (On-Premises 2011)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Steg 2 av 3: Konfigurera Marketo Sync User in Dynamics (On-Premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Bra jobb med att slutföra de föregående stegen - vi går igenom det här.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen (2011 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo-synkroniseringsanvändarrollen till Marketför att synkronisera användare. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo plugin version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Uppgradera Marketo-lösningen för Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Välj **Inställningar** i den nedre vänstra menyn.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Välj **Administration** i trädet.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Välj **Användare**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. En lista över användare visas här. Markera din dedikerade Marknad för att synkronisera användare eller kontakta din [AFDS-administratör (Active Directory Federation Services)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) för att skapa en ny användare som är dedikerad till Marketo. Klicka på **Hantera roller**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Markera **Marketo Sync User** och klicka på **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) och importerar lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Sync User kommer **inte** att synkroniseras tillbaka till Marketo.

## Konfigurera Marketo-lösning {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Välj **Inställningar**. Välj sedan **Marketo Config** i trädet.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår kan du [publicera Marketo-lösningen igen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) eller logga ut och in igen.

1. Klicka på **Standard**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Klicka på ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Markera synkroniseringsanvändaren i popup-fönstret. Klicka sedan på **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Klicka på **Spara** för att spara ändringarna.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Klicka på **Publicera alla anpassningar**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

    * Om du vill begränsa antalet poster som du synkroniserar [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
    * Kör processen [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
    * Logga in på Marketo Sync User i Microsoft Dynamics CRM.

Bra jobbat!

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
