---
unique-page-id: 4720796
description: Återannonsering med webbpersonaliseringsdata - Marketo Docs - Produktdokumentation
title: Återannonsering med webbpersonaliseringsdata
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# Återannonsering med webbpersonaliseringsdata {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>
>Omdirigering av webbplatser ingår nu i panelen Webbanpassning. Om du bara har köpt återmarknadsföring visas den här rutan och du får tillgång till produkten för webbanpassning med **endast** återmarknadsföringsfunktioner aktiverade. Detta ger dig tillgång till kontoinställningar, sidan Återmarknadsföring, segment och ytterligare spårningssidor.

Återmarknadsföring riktar sig till potentiella kunder som tidigare har besökt er webbplats med webbannonsering baserat på vem de är och vad de gjorde. Personaliserad återmarknadsföring riktar sig till specifika målgrupper med relevanta annonser baserade på bransch, namngivna konton och kända persondata.

Webbpersonalisering lägger för närvarande till data på följande återmarknadsföringsplattformar:

* [Google](personalized-remarketing-in-google.md)
* [Facebook](personalized-remarketing-in-facebook.md)

Webbpersonalisering skickar följande data till återmarknadsföringsplattformarna för att skapa målgrupper och köra återmarknadsföringskampanjer:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Webbpersonlighetsdata</th> 
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

## Återmarknadsföringskonfiguration {#remarketing-configuration}

1. Gå till **Återmarknadsföring**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Återmarknadsföringskonfigurationen är per domän eller underdomän. Aktivera de andra domänerna om du vill skicka data från de domänerna till återmarknadsföringsplattformen.

1. Aktivera inställningar för Google Analytics eller Google Universal Analytics per domän.

   >[!NOTE]
   >
   >Google Retargeting Tag måste implementeras på din webbplats.
   >
   >
   >Om du redan har konfigurerat integreringen med Webbanpassning och Google Analytics behöver du inte redigera den här delen eftersom den är samma konfiguration under Kontoinställningar.

   ![](assets/two.png)

1. Aktivera konfigurationen för Facebook. Klicka på och expandera Facebook-dragspelet, klicka på **On **för att skicka respektive händelse och data till Facebook Audience Manager. Klicka på **Spara**.

   >[!NOTE]
   >
   >Du måste ha [Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)installerat din webbplats för att den här funktionen ska fungera.

   ![](assets/three.png)

## Skapar segmenterad publik {#creating-segmented-audience}

Med en segmenterad publik kan ni välja ett befintligt segment som målgrupp för återmarknadsföringskampanjer. Du kan t.ex. markera dina kända personsegment.

>[!TIP]
>
>Det finns ingen anledning att skapa en segmenterad målgrupp för branschdata eller andra data som redan skickats in i domänkonfigurationen. Det är bäst att använda segmenterade målgrupper för segment baserat på kända persondata.

1. Klicka på **Skapa segmenterad målgrupp**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Ange målgruppsnamn, välj Kanaler och välj Segment i listan över befintliga segment.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Klicka på **SPARA**.

   Du har nu slutfört konfigurationen av återmarknadsföring i webbpersonalisering, loggat in på era återmarknadsföringsplattformar och skapat era målgrupper baserat på dessa data och ställt in era återannonskampanjer.

>[!MORELIKETHIS]
>
>* [Personaliserad marknadsföring i Google](personalized-remarketing-in-google.md)
>* [Personaliserad marknadsföring på Facebook](personalized-remarketing-in-facebook.md)

