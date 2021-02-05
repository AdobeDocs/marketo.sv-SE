---
unique-page-id: 4720917
description: Personaliserad Remarketing i Facebook - Marketo Docs - Produktdokumentation
title: Personaliserad marknadsföring på Facebook
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Anpassad marknadsföring på Facebook {#personalized-remarketing-in-facebook}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och kraften i Facebook Remarketing.

>[!PREREQUISITES]
>
>* Slutför installationen av [Återmarknadsföring med webbpersonaliseringsdata](retargeting-with-web-personalization-data.md)
>* Granska [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook-dokumentationen om anpassade målgrupper](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)och ommarketing

>



## Skapa en publik i Facebook {#creating-an-audience-in-facebook}

1. Gå till fliken [Målgrupp](https://www.facebook.com/ads/audience_manager) i Ads Manager på Facebook.
1. Klicka på **Verktyg** och välj **Publiker**.

   ![](assets/one-1.png)

1. Klicka på **Skapa en anpassad målgrupp**.

   ![](assets/two-1.png)

1. Välj **Webbplatstrafik**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. I listan Webbplatstrafik väljer du** Anpassad kombination**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Välj **Händelse** i listan Inkludera.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Välj **RTP Remarketing **och välj en parameter i händelselistan.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. I det här exemplet väljer du Bransch som ska innehålla **Utbildning**. Ange **Utbildning** och redigera **De sista** ska vara 180 dagar. Ange målgruppsnamn: **Skolbranschen**. Klicka på **Skapa målgrupp**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Du har nu skapat en ny anpassad målgrupp med RTP-data på Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## RTP-datapunkter på Facebook {#rtp-data-points-in-facebook}

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
        <td><p>Försvar</p><p>Utbildning</p><p>Finansiella tjänster</p><p>Offentlig sektor</p><p>Sjukvård, farmakologi, bioteknik</p><p>Programvara och Internet</p><p>osv.. (enligt RTP:s branschalternativ)</p></td> 
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

Mer information finns i [Facebooks dokumentation](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

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

1. Nu har ni alla en personaliserad marknadsföringskampanj på Facebook.

>[!MORELIKETHIS]
>
>* [Återannonsering med webbpersonaliseringsdata](retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring i Google](personalized-remarketing-in-google.md)

>



