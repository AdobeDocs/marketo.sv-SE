---
unique-page-id: 4720810
description: Personaliserad Remarketing i Google - Marketo Docs - produktdokumentation
title: Personaliserad marknadsföring i Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# Personaliserad marknadsföring i Google {#personalized-remarketing-in-google}

Med personligt anpassad marknadsföring kan ni återengagera era användare med hjälp av RTP-data och styrkan hos Google Analytics med hjälp av Google Display Network.

>[!PREREQUISITES]
>
>* Slutför [återmarknadsföring med  [!DNL Web Personalization] Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)-konfigurationen
>* Granska dokumentationen för [Återmarknadsföring med Google Analytics Hjälp](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645).

## Creating a Remarketing Audience in Google {#creating-a-remarketing-audience-in-google}

1. Logga in på din Google Analytics. Klicka på **[!UICONTROL Admin]**, **[!UICONTROL Account]**, **[!UICONTROL Property]**. Klicka på **[!UICONTROL Audience Definitions]** och **[!UICONTROL Audiences]**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicka på **[!UICONTROL +New Audience]**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Link Configuration]**: Länka till ditt [!DNL Google Adwords]-konto. **[!UICONTROL Define Audience]**: Klicka på **[!UICONTROL Create New]**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicka på **[!UICONTROL Sequences]** och **[!UICONTROL Find the RTP Data]** under [!UICONTROL Custom Dimensions], [!UICONTROL [!]UICONTROL Custom Variables], [!UICONTROL Events] i Audience Builder.

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
>* Anpassade dimensioner: Organisation, Industri, Kategori (Fortune 500,1000, Global 2000), Grupp (Enterprise, SMB), ABM-lista (lista över namngivna konton)
>* Händelsekategori: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Händelseetikett: Segmentnamn, kampanjnamn, segmenterat publiknamn

**Exempel på återmarknadsföring av målgrupp från segmenterade RTP-målgruppsdata**

1. Klicka på **[!UICONTROL Sequences].**
1. Välj **[!UICONTROL Event Label].**
1. Ange **[!UICONTROL Name of Segmented Audience]** (så som det visas i RTP).
1. Klicka på **[!UICONTROL Apply]**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exempel på publik från RTP-branschdata**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicka på **[!UICONTROL Sequences]**.
1. Välj **[!UICONTROL RTP-Industry]**.
1. Ange **Namn på bransch** (t.ex. [!UICONTROL Financial Services], [!UICONTROL Education]...).
1. Klicka på **[!UICONTROL Apply]**.
1. Ange en **[!UICONTROL Audience Name]**. Klicka på **[!UICONTROL Save]**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Skapa en reklamkampanj för återmarknadsföring i [!DNL Google Adwords] {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Logga in på **[!DNL Google Adwords]**. Klicka på **[!UICONTROL Campaigns]** och välj **[!UICONTROL Display Network only]**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Ange **[!UICONTROL Campaign Name]**, välj **[!UICONTROL Type Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Ange **[!UICONTROL Ad Group Name],** ange **[!UICONTROL Enhanced CPC]**, välj **[!UICONTROL Remarketing List]**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicka på **[!UICONTROL Save]** och fortsätt.
1. Lägg till din bild- eller textannons och starta din marknadsföringskampanj.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Återmarknadsföring med  [!DNL Web Personalization] data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personaliserad återmarknadsföring i [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
