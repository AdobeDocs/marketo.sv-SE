---
unique-page-id: 3571816
description: Steg 2 av 3 - Configure Sync User for Marketo (2013 On-Premises) - Marketo Docs - produktdokumentation
title: Steg 2 av 3 - Konfigurera Synkronisera användare för Marketo (On-Premises 2013)
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Steg 2 av 3: Konfigurera Synkronisera användare för Marketo (lokal 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Bra jobb med att slutföra de föregående stegen - vi går igenom det här.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen i Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo-synkroniseringsanvändarrollen till Marketför att synkronisera användare. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo plugin version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Uppgradera Marketo-lösningen för Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Klicka på **Administration** under **Inställningar**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Välj **Användare**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. En lista över användare visas här. Välj din dedikerade Marketo-synkroniseringsanvändare eller kontakta din [AFDS-administratör (Active Directory Federation Services)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [administratör för att skapa en ny användare som är dedikerad till Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka på ![](assets/image2015-3-26-11-3a16-3a22.png) och välj **Hantera roller**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Markera **Marketo Sync User** och klicka på **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) och importerar lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Sync User kommer **inte** att synkroniseras tillbaka till Marketo.

## Konfigurera Marketo-lösning {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Under **Inställningar** klickar du på **Marketo Config**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Om **Marketo Config** saknas kan du försöka uppdatera sidan. Om problemet kvarstår kan du [publicera Marketo-lösningen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) igen eller försöka logga ut och in igen.

1. Klicka på **Standard**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicka på fältet **Marketo User** och välj synkroniseringsanvändare.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicka på ![](assets/image2015-3-13-15-3a10-3a11.png) längst ned till höger för att spara ändringarna.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicka på **Publicera alla anpassningar**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar [skapar du ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Verifiera Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)-processen. Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in på Marketo Sync User i Microsoft Dynamics CRM.

Bra jobbat!

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Connect Marketo och Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
