---
unique-page-id: 11383953
description: Konfigurera offlinekonverteringar för Facebook - Marketo Docs - produktdokumentation
title: Konfigurera offlinekonverteringar för Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Konfigurera offlinekonverteringar för Facebook {#set-up-facebook-offline-conversions}

Genom att skicka offlinekonverteringsdata tillbaka till Facebook för personer som skapats via Lead Ads kan ert annonsteam optimera sina annonskostnader bättre än någonsin. Så här ställer du in det.

>[!PREREQUISITES]
>
>* Du måste [konfigurera Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Du måste ha en godkänd modell i [Intäktscykelmodelleraren](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Administratörskonfiguration {#admin-configuration}

1. Gå till Marketo **Administratör**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Gå till **LaunchPoint** och dubbelklicka på tjänsten Facebook Lead Ads som du skapade tidigare.

   >[!NOTE]
   >
   >Om du inte har gjort det, så gå vidare och [Konfigurera Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), och sedan komma tillbaka hit.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Om du vill kan du redigera **Visningsnamn** för att inkludera offlinekonverteringar. Klicka **Nästa**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Kontrollera **Aktivera offlinekonverteringar** och klicka **Nästa**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Klicka **Nästa**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Klicka **Spara**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Söt! Du är halvvägs färdig med att aktivera Facebook offlinekonverteringar. Låt oss gå till Revenue Cycle Modeler för att kartlägga faserna.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Konfiguration av intäktscykelmodell {#revenue-cycle-modeler-configuration}

1. Gå till **Analyser**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Välj modell och klicka på **Redigera utkast**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >För närvarande finns det 10 Facebook-händelser som du kan mappa intäktscykelsteg till:
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

1. Markera den scen som du vill mappa och gå sedan till **Facebook Conversion** väljer du den Facebook-händelse som du vill mappa den till. Upprepa det här steget om du vill mappa alla faser i RCM till offlinekonverteringsfaser på Facebook.

   ![](assets/1-1.png)

1. Stäng modellen när du är klar med mappningen.

   ![](assets/2.png)

1. Godkänn din modell så är du klar!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   När Lead Ad-ledarna når de stadier ni mappat skickas konverteringarna till Facebook för rapportering.

   >[!CAUTION]
   >
   >Kontrollera ditt Facebook-konto och se till att alla [annonser är associerade](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) till händelseuppsättningen Marketo Offline Conversions. Om de inte är det kanske inte annonseringen fungerar.

   >[!NOTE]
   >
   >Konverteringsdata offline skickas från Marketo till Facebook flera gånger dagligen.

>[!MORELIKETHIS]
>
>[Förstå Facebook offlinekonverteringar](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
