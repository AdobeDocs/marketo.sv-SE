---
unique-page-id: 2950561
description: Konverteringsskript för anpassade händelser - Marketo Docs - Produktdokumentation
title: Konverteringsskript för anpassade händelser
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Konverteringsskript för anpassade händelser {#conversion-script-for-custom-events}

Du definierar leveransmålet när du skapar ett hänvisningserbjudande. Om den åtgärd som är inriktad på målet är en specifik händelse på din egen webbsida kan du använda ett konverteringsskript för att anropa vårt JavaScript API.

## Hämta konverteringsskriptet {#retrieve-the-conversion-script}

1. Klicka på **Erbjudandeinformation** i redigeraren för hänvisningserbjudandet och välj sedan **Kund-JavaScript-händelse** i listrutan för mål.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Kopiera det översta skriptet i den grå rutan och placera det på webbsidan i `<body>`-taggarna. Det nedersta skriptet placeras inuti `<header>`-taggarna.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Kom ihåg att kopiera och klistra in båda skripten om de finns på en annan webbplats än Marketo.

## Hämta Loader-skriptet {#retrieve-the-loader-script}

1. Välj hänvisningserbjudandet i trädet och klicka sedan på **Åtgärder för hänvisningserbjudande** och **Bädda in kod**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Högerklicka på **sidhuvudskoden** och infoga den i sidhuvudet på webbsidan. Gör sedan samma sak med **Body Code**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Klistrar in skript på din webbsida {#pasting-the-scripts-onto-your-webpage}

Klistra in konverteringsskripten i HTML för brödtexten och rubriken. Placera sedan inläsarskripten i HTML för brödtexten och rubriken.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Ansluta konverteringsskriptet {#connecting-the-conversion-script}

Här skriver du en JavaScript-funktion som använder det specifika HTML-id:t för det sidelement som du vill aktivera målslutförandet för. Till exempel:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

I det här exemplet finns det en knapp på webbsidan med ID &quot;#myButtonId&quot;. När användaren klickar på den knappen registreras personen som slutförd målet.

Häftig! Er webbplats har nu hämtat skräddarsydda mål för social marknadsföring med Marketo.

>[!MORELIKETHIS]
>
>* [Ange mål för hänvisningserbjudande](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Skapa ett hänvisningserbjudande](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Distribuera sociala medier på din webbplats](deploy-social-on-your-website.md)

