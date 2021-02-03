---
unique-page-id: 11383953
description: Konfigurera offlinekonverteringar för Facebook - Marketo Docs - Produktdokumentation
title: Konfigurera offlinekonverteringar för Facebook
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Konfigurera offlinekonverteringar för Facebook {#set-up-facebook-offline-conversions}

Genom att skicka offlinekonverteringsdata tillbaka till Facebook för personer som skapats via Lead Ads kan ert annonsteam optimera sina annonskostnader bättre än någonsin. Så här ställer du in det.

>[!PREREQUISITES]
>
>* Du måste [konfigurera Facebook-annonser](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Du måste ha en godkänd modell i [Intäktscykelmodelleraren](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## Administratörskonfiguration {#admin-configuration}

1. Gå till Marketo **Admin**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Gå till **LaunchPoint** och dubbelklicka på Facebook-tjänsten Lead Ads som du skapade tidigare.

   >[!NOTE]
   >
   >Om du inte har gjort det, gå vidare och [Konfigurera Facebook-annonser](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) och kom sedan tillbaka hit.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Om du vill kan du redigera **visningsnamnet** och inkludera offlinekonverteringar. Klicka på **Nästa**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Markera **Aktivera offlinekonvertering** och klicka på **Nästa**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Klicka på **Nästa**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Klicka på **Spara**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Söt! Du är halvvägs färdig med att aktivera offlinekonverteringar för Facebook. Låt oss gå till Revenue Cycle Modeler för att kartlägga faserna.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Konfiguration av intäktscykelmodelleraren {#revenue-cycle-modeler-configuration}

1. Gå till **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Markera modellen och klicka på **Redigera utkast**.

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
   >* Övriga
   >* Inköp
   >* Sökningar
   >* Innehållsvyer


1. Markera den scen som du vill mappa och välj sedan den Facebook-händelse som du vill mappa den till i listrutan **Facebook-konvertering**. Upprepa det här steget om du vill mappa alla faser i RCM till offlinekonverteringsfaser på Facebook.

   ![](assets/1-1.png)

1. Stäng modellen när du är klar med mappningen.

   ![](assets/2.png)

1. Godkänn din modell så är du klar!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   När Lead Ad-leads når de stadier du mappat skickas konverteringarna till Facebook för rapportering.

   >[!CAUTION]
   >
   >Kontrollera ditt Facebook-konto och se till att alla [annonser är associerade](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) till händelseuppsättningen Marketo Offline Conversions. Om de inte är det kanske inte annonseringen fungerar.

   >[!NOTE]
   >
   >Konverteringsdata offline skickas flera gånger dagligen från Marketo till Facebook.

>[!MORELIKETHIS]
>
>[Förstå offlinekonverteringar för Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
