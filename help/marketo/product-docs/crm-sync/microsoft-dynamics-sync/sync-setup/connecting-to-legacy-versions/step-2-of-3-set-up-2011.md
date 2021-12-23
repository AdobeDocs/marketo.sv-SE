---
unique-page-id: 3571807
description: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics (On-Premises 2011) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Marketo Sync User in Dynamics (On-Premises 2011)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Marketo Sync User i Dynamics (lokal 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Bra jobb med att slutföra de föregående stegen - vi går igenom det här.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo Solution (2011 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo plugin version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Om du vill uppgradera Marketo går du till [Uppgradera Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för Synkronisera användare [ska anges till engelska](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Välj **Inställningar**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Välj **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Välj **Användare**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. En lista över användare visas här. Välj en dedikerad Marketo-synkroniseringsanvändare eller kontakta din [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) administratör för att skapa en ny användare som är dedikerad till Marketo. Klicka **Hantera roller**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Kontrollera **Marketo Sync User** och klicka **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) och importera lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare kommer att **not** synkas tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Välj **Inställningar**. Välj sedan **Marketo Config** i trädet.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Om Marketo Config saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicera Marketo-lösningen igen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) eller logga ut och in igen.

1. Klicka **Standard**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Klicka på ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Markera synkroniseringsanvändaren i popup-fönstret. Klicka sedan på **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Klicka **Spara** för att spara ändringarna.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Klicka **Publicera alla anpassningar**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

    * Om du vill begränsa antalet poster som du synkroniserar [konfigurera ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
    * Kör processen [Validera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
    * Logga in i Marketo Sync User i Microsoft Dynamics CRM.

Bra jobbat!

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Microsoft Dynamics med Marketo (lokal version 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
