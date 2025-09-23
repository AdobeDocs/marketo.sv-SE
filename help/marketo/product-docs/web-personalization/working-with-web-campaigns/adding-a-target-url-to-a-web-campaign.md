---
unique-page-id: 6094879
description: Lägga till en mål-URL i en webbkampanj - Marketo Docs - produktdokumentation
title: Lägga till en mål-URL i en webbkampanj
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 1%

---

# Lägga till en mål-URL i en webbkampanj {#adding-a-target-url-to-a-web-campaign}

En mål-URL finns under sidan Ange kampanj och definierar den specifika URL eller URL:er som en webbkampanj visas på.

## Lägga till en mål-URL för dialogruta eller webbkampanjer för widget {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Gå till **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Välj **[!UICONTROL Create New Web Campaign]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Lägg till en **[!UICONTROL Campaign Name]**. Välj en **[!UICONTROL Target Segment]**. Lägg till **[!UICONTROL Target URL]**.

   ![](assets/set-web-campaign-hands.jpg)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">Namn</th>
   <th colspan="1" rowspan="1">Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Any Page]</strong></td>
   <td colspan="1" rowspan="1"><p>Tillåt att kampanjer visas på alla sidor.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL Include URL parameter when matching]</strong></p></td>
   <td colspan="1" rowspan="1">Lägg till URL-parameter för att matcha och visa kampanjer på URL:er inklusive den här parametern. T.ex. campaign=cpc</td>
  </tr>
 </tbody>
</table>

## Lägga till flera URL:er till mål-URL {#adding-multiple-urls-to-target-url}

Om du klickar på plusikonen (![—](assets/image2015-2-18-8-3a40-3a59.png)) öppnas dialogrutan [!UICONTROL Multiple Value Entry] där du kan lägga till flera URL:er. Lägg till en URL per rad.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Webbkampanjer för dialogrutor och widgetar kan använda alternativen Valfri sida och Jokertecken (&#42;).
>* I avancerade fall kan webbkampanjer i InZone använda jokertecken i slutet av URL-sökvägen. Exempel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL är skiftlägeskänslig

## Lägga till en mål-URL för webbkampanjer i zonen {#adding-a-target-url-for-in-zone-web-campaigns}

1. Gå till **[!UICONTROL Web Campaigns]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Välj **[!UICONTROL Create New Web Campaign]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Lägg till en **[!UICONTROL Campaign Name]**. Välj en **[!UICONTROL Target Segment]**. Lägg till **[!UICONTROL Target URL]**.

   >[!NOTE]
   >
   >Mål-URL:en med In Zones måste definiera en specifik URL eller URL:er. I avancerade fall kan webbkampanjer i InZone använda jokertecken i slutet av URL-sökvägen. Exempel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [Skapa en dialogkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Skapa en RTP i zonkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Skapa en Widget-kampanj för RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
