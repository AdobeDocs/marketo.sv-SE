---
unique-page-id: 2950561
description: Konverteringsskript för anpassade händelser - Marketo Docs - produktdokumentation
title: Konverteringsskript för anpassade händelser
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Konverteringsskript för anpassade händelser {#conversion-script-for-custom-events}

Du definierar leveransmålet när du skapar ett hänvisningserbjudande. Om den åtgärd som är inriktad på målet är en specifik händelse på din egen webbsida kan du använda ett konverteringsskript för att anropa vårt JavaScript API.

## Hämta konverteringsskriptet {#retrieve-the-conversion-script}

1. Klicka på **Erbjudandeinformation** och sedan markera **Kundens JavaScript-händelse** från listrutan för att uppfylla målet.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Kopiera det översta skriptet i den grå rutan och placera det på webbsidan i `<body>` -taggar. Det nedersta skriptet placeras i `<header>` -taggar.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Kom ihåg att kopiera och klistra in båda skripten om de finns på en annan webbplats än Marketo.

## Hämta Loader-skriptet {#retrieve-the-loader-script}

1. Välj hänvisningserbjudandet från trädet och klicka sedan på **Referensåtgärder** och **Bädda in kod**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Högerklicka på **Huvudkod** och infoga den i webbsidans sidhuvud. Gör sedan samma sak med **Kroppskod**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Klistra in skript på din webbsida {#pasting-the-scripts-onto-your-webpage}

Klistra in konverteringsskripten i HTML för brödtexten och rubriken. Placera sedan inläsarskripten i HTML för brödtexten och rubriken.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Ansluta konverteringsskriptet {#connecting-the-conversion-script}

Här skriver du en JavaScript-funktion som använder det specifika HTML-id:t för det sidelement som du vill aktivera målslutförandet för. Exempel:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

I det här exemplet finns det en knapp på webbsidan med ID &quot;#myButtonId&quot;. När användaren klickar på den knappen registreras personen som slutförd målet.

Häftig! Din webbplats har nu anpassat sina mål för social marknadsföring med Marketo.

>[!MORELIKETHIS]
>
>* [Ange mål för hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Skapa ett hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Distribuera sociala medier på din webbplats](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

