---
unique-page-id: 3571816
description: Steg 2 av 3 - Konfigurera Sync User for Marketo (2013 On-Premises) - Marketo Docs - Produktdokumentation
title: Steg 2 av 3 - Konfigurera Synkronisera användare för Marketo (lokal version 2013)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Steg 2 av 3: Konfigurera Synkronisera användare för Marketo (lokal version 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Bra jobb med att slutföra de föregående stegen - vi går igenom det här.

>[!PREREQUISITES]
>
>[Steg 1 av 3: Installera Marketo-lösningen i [!DNL Dynamics] (2013 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)

## Tilldela synkroniseringsanvändarroll {#assign-sync-user-role}

Tilldela endast Marketo Sync User-rollen till Marketo sync-användaren. Du behöver inte tilldela den till andra användare.

>[!NOTE]
>
>Detta gäller Marketo plugin-version 4.0.0.14 och senare. I tidigare versioner måste alla användare ha synkroniseringsanvändarrollen. Mer information om hur du uppgraderar Marketo finns i [Uppgradera Marketo-lösningen för [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Språkinställningen för synkroniseringsanvändaren [ ska anges till engelska](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Administration]**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Välj **[!UICONTROL Users]**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. En lista över användare visas här. Välj en dedikerad Marketo Sync-användare eller kontakta din [Active Directory Federation Services-administratör (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} för att skapa en ny användare som är [dedikerad till Marketo](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx){target="_blank"}.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Välj synkroniseringsanvändare. Klicka på ![](assets/image2015-3-26-11-3a16-3a22.png) och välj **[!UICONTROL Manage Roles]**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Markera **[!UICONTROL Marketo Sync User]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Om du inte ser rollen går du tillbaka till [steg 1 av 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"} och importerar lösningen.

   >[!NOTE]
   >
   >Alla uppdateringar som görs i CRM av Synkronisera användare _synkroniseras inte_ tillbaka till Marketo.

## Konfigurera Marketo Solution {#configure-marketo-solution}

Nästan klart! Vi har bara några sista konfigurationer innan vi går vidare till nästa artikel.

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Marketo Config]**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Om **[!UICONTROL Marketo Config]** saknas kan du försöka uppdatera sidan. Om problemet kvarstår [publicerar du Marketo-lösningen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) igen eller försöker logga ut och in igen.

1. Klicka på **[!UICONTROL Default]**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Klicka på fältet **[!UICONTROL Marketo User]** och välj synkroniseringsanvändare.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Klicka på ![](assets/image2015-3-13-15-3a10-3a11.png) längst ned till höger för att spara ändringarna.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

## Innan du fortsätter till steg 3 {#before-proceeding-to-step}

* Om du vill begränsa antalet poster som du synkroniserar konfigurerar [ett anpassat synkroniseringsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) nu.
* Kör [Verifiera [!DNL Microsoft Dynamics] synkroniseringsprocessen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Den verifierar att dina initiala inställningar har gjorts korrekt.
* Logga in i Marketo Sync User i [!DNL Microsoft Dynamics] CRM.

Snyggt jobb!

>[!MORELIKETHIS]
>
>[Steg 3 av 3: Anslut Marketo och [!DNL Dynamics] (2013 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md)
