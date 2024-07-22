---
unique-page-id: 4720796
description: Återannonsering med Web Personalization Data - Marketo Docs - produktdokumentation
title: Återannonsering med Web Personalization Data
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Återannonsering med Web Personalization Data {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Omdirigering av webbplatser faller nu under Web Personalization. Om du bara har köpt återmarknadsföring visas den här rutan och du får tillgång till Personalization-produkten på webben med funktionen **endast** återmarknadsföring aktiverad. Detta ger dig tillgång till kontoinställningar, sidan för omdirigering, segment och ytterligare spårningssidor.

Återmarknadsföring riktar sig till potentiella kunder som tidigare har besökt er webbplats med webbannonsering baserat på vem de är och vad de gjorde. Personaliserad återmarknadsföring riktar sig till specifika målgrupper med relevanta annonser baserade på bransch, namngivna konton och kända persondata.

Web Personalization lägger för närvarande till data till följande återmarknadsföringsplattformar:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Personalization skickar följande data till marknadsföringsplattformarna för att skapa målgrupper och köra reklamkampanjer:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Web Personalization Data</th> 
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

1. Gå till **Återmarknadsföring**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Återmarknadsföringskonfigurationen är per domän eller underdomän. Aktivera de andra domänerna om du vill skicka data från de domänerna till återmarknadsföringsplattformen.

1. Aktivera inställningar för Google Analytics eller Google Universal Analytics per domän.

   >[!NOTE]
   >
   >Du måste implementera Google Retargeting Tag på din webbplats.
   >
   >Om du redan har konfigurerat integreringen med Web Personalization och Google Analytics behöver du inte redigera den här delen eftersom den är samma konfiguration under Kontoinställningar.

   ![](assets/two.png)

1. Aktivera konfigurationen för Facebook. Klicka på och expandera Facebook-dragspelspanelen och klicka **På** för att skicka respektive händelse och data till Facebook Audience Manager. Klicka på **Spara**.

   >[!NOTE]
   >
   >Du måste ha [Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)installerat på din webbplats för att den här funktionen ska fungera.

   ![](assets/three.png)

## Skapa segmenterad publik {#creating-segmented-audience}

Med en segmenterad publik kan ni välja ett befintligt segment som målgrupp för återmarknadsföringskampanjer. Du kan t.ex. markera dina kända personsegment.

>[!TIP]
>
>Det finns ingen anledning att skapa en segmenterad målgrupp för branschdata eller andra data som redan skickats in i domänkonfigurationen. Det är bäst att använda segmenterade målgrupper för segment baserat på kända persondata.

1. Klicka på **Skapa segmenterad publik**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Ange målgruppsnamn, välj Kanaler och välj Segment i listan över befintliga segment.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Klicka på **Spara**.

   Du har nu slutfört konfigurationen av återmarknadsföring i Web Personalization, loggat in på era återmarknadsföringsplattformar och skapat era målgrupper baserat på dessa data och konfigurerat era återmarknadsföringskampanjer.
