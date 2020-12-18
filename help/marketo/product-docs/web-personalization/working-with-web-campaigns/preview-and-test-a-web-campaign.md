---
unique-page-id: 10092925
description: Förhandsgranska och testa en webbkampanj - Marketo Docs - Produktdokumentation
title: Förhandsgranska och testa en webbkampanj
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Förhandsgranska och testa en webbkampanj {#preview-and-test-a-web-campaign}

I den här artikeln visas olika sätt att förhandsgranska en webbkampanj och även hur du testar den med ett sandlådesegment direkt på webbplatsen.

## Förhandsgranska en webbkampanj på sidan Skapa {#preview-a-web-campaign-on-the-creation-page}

1. Gå till **Webben** **Kampanjer**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Klicka på** Skapa ny webbkampanj**** **eller ikonen för att redigera en befintlig kampanj.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Lägg till sidans URL i Förhandsgranska på plats och klicka på **Förhandsgranska**. Ett nytt fönster/en ny flik öppnas som visar kampanjens förhandsgranskning.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Klicka på **Dela** för att öppna ett e-postmeddelande med en fast URL för kampanjens förhandsgranskning.

   >[!NOTE]
   >
   >Du kan också installera ett webbläsarplugin-program (antingen [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) eller [Firefox](http://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi)) för att få den bästa upplevelsen när du förhandsgranskar kampanjen. Se avsnittet nedan.

## Förhandsgranska en webbkampanj på sidan Skapa med plugin-programmet för webbläsare {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Följ steg 1 och 2 från `section above`.
1. Klicka på länken till webbläsarplugin-programmet (i det här fallet använder vi Chrome).

   ![](assets/4-1.png)

1. Ett nytt fönster/en ny flik öppnas. Klicka på **Lägg till i Chrome**.

   ![](assets/five.png)

1. Klicka på **Lägg till tillägg**.

   ![](assets/six.png)

1. Gå tillbaka till Marketo. Lägg till sidans URL och klicka på **Förhandsgranska**.

   ![](assets/seven.png)

1. Ett nytt fönster/flik öppnas där du kan förhandsgranska hur kampanjen ser ut på en dator, telefon eller surfplatta.

   ![](assets/campaign-preview.png)

## Förhandsgranska en webbkampanj på webbkampanjsidan {#preview-a-web-campaign-on-the-web-campaigns-page}

1. När du tittar på listan över dina webbkampanjer väljer du bara en kampanj och klickar på ikonen **Förhandsgranska**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Enkelt!

## Förhandsgranska en webbkampanj på din webbplats {#preview-a-web-campaign-on-your-website}

Skapa ett sandlådesegment och en kampanj.

1. Gå till **Segment**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Klicka på **Skapa ny**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Namnge segmentet.
1. Under Beteende drar du Inkludera sidor till arbetsytan. Lägg till värdet *sandbox=1*. Klicka på Spara och definiera kampanj.

   ![](assets/segment.png)

1. På sidan Ange webbkampanj ändrar du målsegmentet till sandlådesegmentet genom att markera det i listan.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Slutför kampanjkreativiteten och klicka på **Starta**.\
   ![](assets/click-launch.jpg)

1. Gå till webbplatsen och lägg till URL-parametern&quot;?sandbox=1&quot; i slutet av URL:en. Exempel: [www.marketo.com?sandbox=1](http://www.marketo.com/?sandbox=1)
1. Se kampanjens respons på er webbplats.

>[!NOTE]
>
>Kampanjerna reagerar bara en gång under en besökarsession. Rensa dina cookies i webbläsaren om du vill se kampanjen igen.

>[!NOTE]
>
>Omdirigeringskampanjer kan inte förhandsgranskas. Det enda sättet att testa dem är att använda ett sandlådesegment (som har specifika sidor som mål - *sandbox=redirect*)

