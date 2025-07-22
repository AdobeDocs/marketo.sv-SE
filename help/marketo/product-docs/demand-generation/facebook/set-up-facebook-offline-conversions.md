---
unique-page-id: 11383953
description: Konfigurera offlinekonverteringar för Facebook - Marketo Docs - produktdokumentation
title: Konfigurera offlinekonverteringar för Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Konfigurera [!DNL Facebook] offlinekonverteringar {#set-up-facebook-offline-conversions}

Genom att skicka offlinekonverteringsdata tillbaka till [!DNL Facebook] för personer som skapats via Lead Ads kan ert annonsteam optimera sina annonskostnader bättre än någonsin. Så här ställer du in det.

>[!PREREQUISITES]
>
>* Du måste [konfigurera Facebook-annonser](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Du måste ha en godkänd modell i [Inkomstcykeln Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Administratörskonfiguration {#admin-configuration}

1. Gå till Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Gå till **[!UICONTROL LaunchPoint]** och dubbelklicka på tjänsten Facebook Lead Ads som du skapade tidigare.

   >[!NOTE]
   >
   >Om du inte har gjort det går du vidare och [Konfigurera [!UICONTROL Facebook Lead Ads]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) och kommer sedan tillbaka hit.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Om du vill kan du redigera **[!UICONTROL Display Name]** så att den inkluderar offlinekonverteringar. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Markera **[!UICONTROL Enable Offline Conversions]** och klicka på **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Söt! Du är halvvägs färdig med att aktivera [!DNL Facebook] offlinekonverteringar. Låt oss gå över till Revenue Cycle Modeler för att kartlägga faserna.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Inkomstcykel, Modeler-konfiguration {#revenue-cycle-modeler-configuration}

1. Gå till **[!UICONTROL Analytics]**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Markera modellen och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >För närvarande finns det 10 [!DNL Facebook] händelser som du kan mappa intäktscykelsteg till:
   >
   >* Lägger till betalningsinformation
   >* Lägger till i kundvagnen
   >* Lägger till i önskelista
   >* Slutförda registreringar
   >* Utcheckningar har initierats
   >* Person
   >* Övrigt
   >* Inköp
   >* Sökningar
   >* Innehållsvyer

1. Markera den scen som du vill mappa och välj sedan den **[!UICONTROL Facebook Conversion]**-händelse som du vill mappa den till i listrutan [!DNL Facebook]. Upprepa det här steget om du vill mappa alla faser i RCM till offlinekonverteringsfaser på [!DNL Facebook].

   ![](assets/1-1.png)

1. Stäng modellen när du är klar med mappningen.

   ![](assets/2.png)

1. Godkänn din modell så är du klar!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   När Lead Ad-leads når de stadier som du har mappat skickas nu konverteringarna till [!DNL Facebook] för rapportering.

   >[!CAUTION]
   >
   >Kontrollera ditt [!DNL Facebook]-konto och se till att alla [annonser är kopplade](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer) till händelseuppsättningen Marketo Offline Conversions. Om de inte är det kanske inte annonseringen fungerar.

   >[!NOTE]
   >
   >Konverteringsdata offline skickas från Marketo till [!DNL Facebook] flera gånger dagligen.

>[!MORELIKETHIS]
>
>[Förstå [!DNL Facebook] Offlinekonverteringar](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
