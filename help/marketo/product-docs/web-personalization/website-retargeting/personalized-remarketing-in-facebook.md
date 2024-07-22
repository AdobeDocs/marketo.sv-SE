---
unique-page-id: 4720917
description: Personaliserad Remarketing i Facebook - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Personaliserad marknadsföring i Facebook {#personalized-remarketing-in-facebook}

Med personaliserad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och styrkan i Facebook Remarketing.

>[!PREREQUISITES]
>
>* Slutför installationen av [återmarknadsföring med Web Personalization Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Granska [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook-dokumentationen om anpassade målgrupper](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) och återmarknadsföring.

## Skapa en publik i Facebook {#creating-an-audience-in-facebook}

1. I Facebook går du till [målgruppsfliken](https://www.facebook.com/ads/audience_manager) i annonshanteraren.

1. Klicka på **Verktyg** och välj **Publiker**.

   ![](assets/one-1.png)

1. Klicka på **Skapa en anpassad målgrupp**.

   ![](assets/two-1.png)

1. Välj **Webbplatstrafik**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Välj **Anpassad kombination** i listan över webbplatstrafik.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Välj **Händelse** i listan Inkludera.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Välj **RTP-ommarknadsföring** i händelselistan och välj en parameter.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. I det här exemplet väljer du Bransch som ska innehålla **Utbildning**. Ange **Utbildning** och redigera **Under de senaste** till 180 dagarna. Ange målgruppsnamn: **Utbildningsbranschen**. Klicka på **Skapa publik**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Du har nu skapat en ny anpassad målgrupp med RTP-data i Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## RTP-datapunkter i Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Händelsenamn</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP Remarketing</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parameter</th> 
        <th>Värde</th> 
       </tr> 
       <tr> 
        <td>ABM-lista</td> 
        <td>(Namn på kontobaserad lista)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Kategori</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Grupp</td> 
        <td colspan="1"><p>Enterprise</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Bransch</td> 
        <td><p>Försvar</p><p>Utbildning</p><p>Finansiella tjänster</p><p>Offentlig sektor</p><p>Sjukvård, farmakologi, bioteknik</p><p>Programvara och Internet</p><p>etc.. (enligt RTP-branschalternativ)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Segmenterad publik</td> 
        <td colspan="1">(Namn på segmenterad publik som skapats i RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Rikta in er målgrupp med en annons {#target-your-audience-with-an-ad}

Mer information finns i [Facebook-dokumentation](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Gå till annonshanteraren och klicka på **Skapa annons**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Välj **Skicka personer till din webbplats** som mål för din kampanj.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Ange webbplatsens URL.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Skapa er annonsuppsättning. Välj en anpassad målgrupp i listan över målgrupper som du har skapat, till exempel Education Industry.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Välj alla andra alternativ för annonsuppsättning, ange din budget och definiera era annonskreatörer.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Nu har ni alla en personaliserad marknadsföringskampanj i Facebook.

>[!MORELIKETHIS]
>
>* [Återmarknadsföring med Personalization-data på webben](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring i Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
