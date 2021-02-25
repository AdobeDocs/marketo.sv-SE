---
unique-page-id: 4720810
description: Personaliserad Remarketing i Google - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Google
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Anpassad marknadsföring i Google {#personalized-remarketing-in-google}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och Google Analytics med Google Display Network.

>[!PREREQUISITES]
>
>* Slutför konfigurationen [Återmarknadsföring med webbpersonaliseringsdata](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Granska [Marknadsföring med Google Analytics Help](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)-dokumentationen.


## Skapa en marknadsföringsmålgrupp i Google {#creating-a-remarketing-audience-in-google}

1. Logga in på Google Analytics. Klicka på **Admin**, **Konto**, **Egenskap**. Klicka på **Målgruppsdefinitioner** och **Målgrupper**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicka på **+Ny publik**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Länkkonfiguration**: Länka till ditt Google Adwords-konto. **Definiera målgrupp**: Klicka på  **Skapa nytt**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. I Audience Builder klickar du på **Sequences** och **Find the RTP Data** under Custom Dimensions, Custom Variables, Events.

>[!TIP]
>
>Hur hittar man RTP-data i Analytics för att bygga upp sin målgrupp?
>
>I Google Analytics:
>
>* Anpassade variabler: Organisation, industri
>* Händelsekategori: Segment, Insightera-CTA, RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat målgruppsnamn

>
>
I Google Universal Analytics:
>
>* Anpassade Dimensioner: Organisation, bransch, kategori (Fortune 500,1000, Global 2000), grupp (Enterprise, SMB), ABM-lista (lista över namngivna konton)
>* Händelsekategori: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat målgruppsnamn


**Exempel på återmarknadsföring från RTP-segmenterade målgruppsdata**

1. Klicka på **Sekvenser.**
1. Välj **Händelseetikett.**
1. Ange **Namn på segmenterad publik** (så som det visas i RTP).
1. Klicka på **Använd**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exempel på publik från RTP:s branschdata**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicka på **Sekvenser**.
1. Välj **RTP-Industry**.
1. Ange **Namn på bransch** (t.ex. Finansiella tjänster, utbildning..).
1. Klicka på **Använd**.
1. Ange ett **målgruppsnamn**. Klicka på **Spara**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Skapa en reklamkampanj för återmarknadsföring i Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Logga in på **Google Adwords**. Klicka på **Kampanjer** och välj **Visa endast nätverk**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Ange **kampanjnamn**, välj **Type Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Ange **Ad Group Name,** ange **Enhanced CPC**, Välj **Remarketing List**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicka på Spara och fortsätt.
1. Lägg till din bild- eller textannons och starta din marknadsföringskampanj.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Återannonsering med webbpersonaliseringsdata](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring på Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

