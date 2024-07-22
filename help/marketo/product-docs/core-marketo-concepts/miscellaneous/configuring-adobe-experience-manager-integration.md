---
unique-page-id: 30081815
description: Konfigurera Adobe Experience Manager-integrering - Marketo Docs - produktdokumentation
title: Konfigurera Adobe Experience Manager-integrering
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Konfigurera Adobe Experience Manager-integrering {#configuring-adobe-experience-manager-integration}

Konfigurera Adobe Experience Manager (AEM) så att du kan komma åt, välja och importera AEM i Marketo Engage Design Studio.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!IMPORTANT]
>
>* Den här integreringen fungerar bara med implementeringar av AEM lokalt och stöds inte för AEM Cloud Service-implementeringar.
>
>* För närvarande stöds den här funktionen endast fullt ut i Firefox. Det stöds inte i Safari och kanske inte fungerar i den senaste versionen av Chrome, beroende på inställningarna för cookie-filen för samma plats.

1. Gå till Adobe Experience Manager (URL:en är specifik för ditt företag).

   ![](assets/one.png)

1. Du kan logga in med Adobe eller logga in lokalt. I det här exemplet loggar vi in lokalt.

   ![](assets/two.png)

1. I **[!UICONTROL Tools]** klickar du på **[!UICONTROL Operations]** och väljer **[!UICONTROL Web Console]**.

   ![](assets/2a.png)

1. I webbläsaren söker du efter &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot; (på Windows, cmd+f på Mac).

   ![](assets/three.png)

1. Klicka på **+** till höger.

   ![](assets/four.png)

1. Skriv `https://.*\.marketo\.com` i textrutan **[!UICONTROL Allowed Origins (Regexp)]** och klicka på **[!UICONTROL Save]**.

   ![](assets/five-psd.png)

1. Klicka på **[!UICONTROL Web Console]** i sidhuvudet högst upp på sidan och välj **[!UICONTROL System Information]**.

   ![](assets/six.png)

1. Klicka på knappen **[!UICONTROL Restart]** under Serverinformation.

   ![](assets/seven.png)

1. Bekräfta genom att klicka på **[!UICONTROL OK]**.

   ![](assets/eight.png)

1. Klicka på **[!UICONTROL Admin]** i Marketo Engage.

   ![](assets/nine.png)

1. Välj **[!UICONTROL Adobe Experience Manager]** under Integrering.

   ![](assets/ten.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/eleven.png)

1. Ange AEM URL och klicka på **[!UICONTROL OK]**.

   ![](assets/twelve.png)
