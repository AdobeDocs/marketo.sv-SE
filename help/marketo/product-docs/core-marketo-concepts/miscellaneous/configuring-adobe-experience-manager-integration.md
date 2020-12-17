---
unique-page-id: 30081815
description: Konfigurera Adobe Experience Manager-integrering - Marketo Docs - Produktdokumentation
title: Konfigurera Adobe Experience Manager Integration
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Konfigurerar Adobe Experience Manager-integrering {#configuring-adobe-experience-manager-integration}

Konfigurera AEM så att du kan komma åt, välja och importera AEM till Marketos Design Studio.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!CAUTION]
>
>För närvarande stöds den här funktionen endast fullt ut i Firefox. Det stöds inte i Safari och kanske inte fungerar i den senaste versionen av Chrome (version 80), beroende på inställningarna för cookie-filen för samma plats.

1. Gå till Adobe Experience Manager (URL:en är specifik för ditt företag).

   ![](assets/one.png)

1. Du kan logga in med Adobe eller logga in lokalt. I det här exemplet loggar vi in lokalt.

   ![](assets/two.png)

1. I **Verktyg** klickar du på **Åtgärder** och väljer **Webbkonsol**.

   ![](assets/2a.png)

1. I webbläsaren söker du efter &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot; (på Windows, cmd+f på Mac).

   ![](assets/three.png)

1. Klicka på **+**-tecknet till höger.

   ![](assets/four.png)

1. I textrutan **Tillåtna original (Regexp)** skriver du &quot;https://.*\.marketo\.com&quot; (utan citattecken) och klicka på **Spara**.

   ![](assets/five-psd.png)

1. Klicka på **Webbkonsol** i sidhuvudet överst på sidan och välj **Systeminformation**.

   ![](assets/six.png)

1. Klicka på knappen **Starta om** under Serverinformation.

   ![](assets/seven.png)

1. Bekräfta genom att klicka på **OK**.

   ![](assets/eight.png)

1. I Marketo Classic klickar du på **Admin**.

   ![](assets/nine.png)

1. Under Integrering väljer du **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Klicka på **Redigera**.

   ![](assets/eleven.png)

1. Ange din AEM-URL och klicka på **OK**.

   ![](assets/twelve.png)

   Du är redo! Du kan nu [importera AEM till Design Studio i Marketo Skyn](http://help.marketo.com/hc/en-us/articles/360036765993).

