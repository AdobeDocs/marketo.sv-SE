---
unique-page-id: 4720810
description: Personaliserad Remarketing i Google - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Personaliserad marknadsföring i Google {#personalized-remarketing-in-google}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och Google Analytics med hjälp av Google Display Network.

>[!PREREQUISITES]
>
>* Slutför konfigurationen för [återmarknadsföring med Web Personalization Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Granska dokumentationen för [Återmarknadsföring med hjälp av Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645).

## Creating a Remarketing Audience in Google {#creating-a-remarketing-audience-in-google}

1. Logga in på Google Analytics. Klicka på **Admin**, **Konto**, **Egenskap**. Klicka på **Målgruppsdefinitioner** och **Målgrupper**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicka på **+Ny publik**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Länkkonfiguration**: Länka till ditt Google Adwords-konto. **Definiera målgrupp**: Klicka på **Skapa ny**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicka på **Sekvenser** och **Hitta RTP-data** under Anpassade Dimensioner, Anpassade variabler och Händelser i Audience Builder.

>[!TIP]
>
>Hur hittar man RTP-data i Analytics för att bygga upp sin målgrupp?
>
>I Google Analytics:
>
>* Anpassade variabler: Organisation, Bransch
>* Händelsekategori: Segment, Insightera-CTA, RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat publiknamn
>
>I Google Universal Analytics:
>
>* Anpassade Dimensioner: Organisation, Industri, Kategori (Fortune 500, 1000, Global 2000), Grupp (Enterprise, SMB), ABM-lista (lista över namngivna konton)
>* Händelsekategori: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat publiknamn

**Exempel på återmarknadsföring av målgrupp från segmenterade RTP-målgruppsdata**

1. Klicka på **Sekvenser.**
1. Välj **Händelseetikett.**
1. Ange **namnet på den segmenterade målgruppen** (så som det visas i RTP).
1. Klicka på **Använd**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exempel på publik från RTP-branschdata**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicka på **Sekvenser**.
1. Välj **RTP-Industry**.
1. Ange **namnet på branschen** (t.ex. Finansiella tjänster, utbildning..).
1. Klicka på **Använd**.
1. Ange ett **publiknamn**. Klicka på **Spara**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Skapa en reklamkampanj på nytt i Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Logga in på **Google Adwords**. Klicka på **Kampanjer** och välj **Visa endast nätverk**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Ange **kampanjnamn**, välj **Skriv om marknadsföring.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Ange **annonsgruppsnamn,** ange **Förbättrad CPC**, välj **Återmarknadsföringslista**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicka på Spara och fortsätt.
1. Lägg till din bild- eller textannons och starta din marknadsföringskampanj.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Återmarknadsföring med Personalization-data på webben](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring i Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
