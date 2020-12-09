---
unique-page-id: 4720810
description: Personaliserad Remarketing i Google - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Google
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---


# Personaliserad marknadsföring i Google {#personalized-remarketing-in-google}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och Google Analytics med Google Display Network.

>[!PREREQUISITES]
>
>* Slutför konfigurationen av [återmarknadsföring med webbpersonaliseringsdata](retargeting-with-web-personalization-data.md)
>* Granska [kommentarsinformation med hjälpdokumentationen](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) för Google Analytics

>



## Creating a Remarketing Audience in Google {#creating-a-remarketing-audience-in-google}

1. Logga in på Google Analytics. Klicka på **Admin**, **Konto**, **Egenskap**. Klicka på **Målgruppsdefinitioner** och **Målgrupper**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicka **+Ny publik**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Länkkonfiguration**: Länka till ditt Google Adwords-konto
1. **Definiera målgrupp**: Klicka på **Skapa nytt**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. I Audience Builder klickar du på **Sequences** och **letar upp RTP-data** under Custom Dimensions, Custom Variables, Events.

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

>



**Exempel på återmarknadsföring från RTP-segmenterade målgruppsdata**

1. Klicka på **Sekvenser.**
1. Välj **Händelseetikett.**
1. Ange **namnet på segmenterad publik** (så som det visas i RTP).
1. Klicka på **Använd**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exempel på publik från RTP:s branschdata**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicka på **Sekvenser**.
1. Välj** RTP-Industry**.
1. Ange **namnet på branschen** (t.ex. Finansiella tjänster, utbildning..).
1. Klicka på **Använd**.
1. Ange ett **målgruppsnamn**. Klicka på **Spara**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Skapa en reklamkampanj för återmarknadsföring i Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Logga in på **Google Adwords**. Klicka på **Kampanjer** och välj **Visa endast** nätverk.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Ange **kampanjnamn**, välj **Typåtermarknadsföring.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Ange **annonsgruppnamn,** ange **Förbättrad CPC** och välj **Marknadsföringslista**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicka på Spara och fortsätt.
1. Lägg till din bild- eller textannons och starta din marknadsföringskampanj.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Återannonsering med webbpersonaliseringsdata](retargeting-with-web-personalization-data.md)
>* [Personaliserad marknadsföring på Facebook](personalized-remarketing-in-facebook.md)

