---
unique-page-id: 4720796
description: Återannonsering med Web Personalization Data - Marketo Docs - produktdokumentation
title: Återannonsering med Web Personalization Data
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 1%

---

# Återmarknadsföring med [!DNL Web Personalization]-data {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Omdirigering av webbplatser faller nu under Web Personalization. Om du bara har köpt återmarknadsföring visas den här rutan och du får tillgång till produkten [!DNL Web Personalization] med återmarknadsföringsfunktionerna **only** aktiverade. Detta ger dig tillgång till kontoinställningar, sidan för omdirigering, segment och ytterligare spårningssidor.

Återmarknadsföring riktar sig till potentiella kunder som tidigare har besökt er webbplats med webbannonsering baserat på vem de är och vad de gjorde. Personaliserad återmarknadsföring riktar sig till specifika målgrupper med relevanta annonser baserade på bransch, namngivna konton och kända persondata.

Web Personalization lägger för närvarande till data till följande återmarknadsföringsplattformar:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] skickar följande data till återmarknadsföringsplattformarna för att skapa målgrupper och köra återmarknadsföringskampanjer:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">[!DNL Web Personalization] Data</th> 
  </tr> 
  <tr> 
   <th><p>Bransch</p></th> 
  </tr> 
  <tr> 
   <th><p>Grupp (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Kategori (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM-lista (lista över namngivna konton)</p></th> 
  </tr> 
  <tr> 
   <th><p>Segmenterad publik (baserad på segment)</p></th> 
  </tr> 
  <tr> 
   <th><p>Webbkampanjer klickade</p></th> 
  </tr> 
 </tbody> 
</table>

## Remarketing-konfiguration {#remarketing-configuration}

1. Gå till **[!UICONTROL Retargeting]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Återmarknadsföringskonfigurationen är per domän eller underdomän. Aktivera de andra domänerna om du vill skicka data från de domänerna till återmarknadsföringsplattformen.

1. Aktivera inställningar för Google Analytics eller [!DNL Google Universal Analytics] per domän.

   >[!NOTE]
   >
   >Du måste implementera Google Retargeting Tag på din webbplats.
   >
   >Om du redan har konfigurerat integreringen med Web Personalization och Google Analytics behöver du inte redigera den här delen eftersom den är samma konfiguration under Kontoinställningar.

   ![](assets/two.png)

1. Aktivera konfigurationen för Facebook. Klicka på och expandera dragspelet [!DNL Facebook], klicka på **[!UICONTROL On]** för att skicka respektive händelse och data till Facebook Audience Manager. Klicka på **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Webbplatsen måste ha [[!DNL Facebook] Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) installerad för att den här funktionen ska fungera.

   ![](assets/three.png)

## Skapa segmenterad publik {#creating-segmented-audience}

Med en segmenterad publik kan ni välja ett befintligt segment som målgrupp för återmarknadsföringskampanjer. Du kan t.ex. markera dina kända personsegment.

>[!TIP]
>
>Det finns ingen anledning att skapa en segmenterad målgrupp för branschdata eller andra data som redan skickats in i domänkonfigurationen. Det är bäst att använda segmenterade målgrupper för segment baserat på kända persondata.

1. Klicka på **[!UICONTROL Create Segmented Audience]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Ange målgruppsnamn, välj Kanaler och välj Segment i listan över befintliga segment.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Klicka på **[!UICONTROL Save]**.

   Du har nu slutfört konfigurationen för återmarknadsföring i [!DNL Web Personalization], loggar in på dina återmarknadsföringsplattformar och skapar målgrupper baserat på dessa data och konfigurerar dina återmarknadsföringskampanjer.
