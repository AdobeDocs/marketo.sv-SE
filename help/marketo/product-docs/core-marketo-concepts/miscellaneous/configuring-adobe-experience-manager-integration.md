---
unique-page-id: 30081815
description: Konfigurera Adobe Experience Manager-integrering - Marketo Docs - produktdokumentation
title: Konfigurera Adobe Experience Manager Integration
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Konfigurera Adobe Experience Manager Integration {#configuring-adobe-experience-manager-integration}

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

1. I **verktyg**, klicka **Operationer** och markera **Webbkonsol**.

   ![](assets/2a.png)

1. I webbläsaren söker du efter &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot; (på Windows, cmd+f på Mac).

   ![](assets/three.png)

1. Klicka på **+** till höger.

   ![](assets/four.png)

1. I **Tillåtna original (Regexp)** textruta, skriva in `https://.*\.marketo\.com` och klicka **Spara**.

   ![](assets/five-psd.png)

1. Klicka på i sidhuvudet högst upp på sidan **Webbkonsol** och markera **Systeminformation**.

   ![](assets/six.png)

1. Klicka på **Starta om** -knappen.

   ![](assets/seven.png)

1. Klicka **OK** för att bekräfta.

   ![](assets/eight.png)

1. Klicka på Marketo Engage **Administratör**.

   ![](assets/nine.png)

1. Under Integrering väljer du **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Klicka **Redigera**.

   ![](assets/eleven.png)

1. Ange AEM URL och klicka på **OK**.

   ![](assets/twelve.png)
