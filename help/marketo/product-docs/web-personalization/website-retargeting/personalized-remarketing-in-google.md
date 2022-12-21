---
unique-page-id: 4720810
description: Personaliserad Remarketing i Google - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Personaliserad marknadsföring i Google {#personalized-remarketing-in-google}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och Google Analytics med hjälp av Google Display Network.

>[!PREREQUISITES]
>
>* Slutför [Återannonsering med webbpersonaliseringsdata](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) konfiguration
>* Granska [Remarketing with Google Analytics Help](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) dokumentation.


## Creating a Remarketing Audience in Google {#creating-a-remarketing-audience-in-google}

1. Logga in på Google Analytics. Klicka **Administratör**, **Konto**, **Egenskap**. Klicka på **Målgruppsdefinitioner** och **Målgrupper**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicka **+Ny publik**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Länkkonfiguration**: Länka till ditt Google Adwords-konto. **Definiera målgrupp**: Klicka **Skapa nytt**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicka på **Sekvenser** och **Hitta RTP-data** under Anpassade Dimensioner, Anpassade variabler, Händelser.

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
>I Google Universal Analytics:
>
>* Anpassade Dimensioner: Organisation, bransch, kategori (Fortune 500,1000, Global 2000), grupp (Enterprise, SMB), ABM-lista (lista över namngivna konton)
>* Händelsekategori: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat målgruppsnamn


**Exempel på återmarknadsföring från RTP-segmenterade målgruppsdata**

1. Klicka **Sekvenser.**
1. Välj **Händelseetikett.**
1. Retur **Namn på segmenterad publik** (som det visas i RTP).
1. Klicka **Använd**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exempel på publik från RTP:s branschdata**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicka **Sekvenser**.
1. Välj **RTP-Bransch**.
1. Retur **Branschnamn** (t.ex. Finansiella tjänster, utbildning..).
1. Klicka **Använd**.
1. Ange en **Målgruppsnamn**. Klicka **Spara**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Skapa en reklamkampanj på nytt i Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Logga in på **Google Adwords**. Klicka på **Kampanjer**, markera **Visa endast nätverk**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Retur **Kampanjnamn**, välj **Skriv Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Retur **Annonsgruppsnamn,** enter **Förbättrad CPC**, välj **Remarketing List**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicka på Spara och fortsätt.
1. Lägg till din bild- eller textannons och starta din marknadsföringskampanj.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Återannonsering med webbpersonaliseringsdata](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring i Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

