---
unique-page-id: 4719402
description: Skapa en ny webbkampanj för widget - Marketo Docs - Produktdokumentation
title: Skapa en ny webbkampanj för widget
exl-id: e00f5be7-1d33-4659-8f38-b74b53eeb09f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Skapa en ny webbkampanj för widget {#create-a-new-widget-web-campaign}

En webbkampanj är en anpassad reaktion som är kopplad till ett visst segment och kan vara en [dialogruta](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) på din webbplats, en [ i zonersättning](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md), en widgetfunktion eller en e-postavisering. Widgetens webbkampanj är en text eller en banderoll som visas på den lodräta sidan av webbsidan med möjlighet att expandera och dra samman, samtidigt som den är fast på webbplatsens sida under hela besöket.

## Skapa en webbkampanj för widget {#create-a-widget-web-campaign}

1. Gå till **[!UICONTROL Web Campaigns]**.

   ![](assets/image2016-8-18-15-3a57-3a46.png)

1. Välj **[!UICONTROL Create New Web Campaign]**.

   ![](assets/create-new-web-campaign-hand-1.png)

1. Välj kampanjtypen **[!UICONTROL Widget]**.

   ![](assets/3.png)

1. Använd de olika alternativen för att anpassa widgeten.

   ![](assets/4.png)

1. Klicka på **[!UICONTROL Preview]** om du vill se hur webbkampanjen kommer att reagera på din webbplats.

   ![](assets/preview.png)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">Namn</th>
   <th colspan="1" rowspan="1">Beskrivning</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1"><strong>Mallar</strong></td>
   <td colspan="1">Välj bland flera färdiga mallar.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Visa på</strong></td>
   <td colspan="1">Gör att du kan <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/set-how-your-web-campaign-displays.md" rel="nofollow">anpassa när och hur</a> webbkampanjen visas.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Animera in/ut</strong></td>
   <td colspan="1">Ange vid dialogrutans inmatning och/eller avslutning. Välj effekt (släpp, blinda, glid, tona, ingen effekt), varaktighet (i sekunder) och riktning (upp, ned, vänster, höger).</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Position</strong></td>
   <td colspan="1">Välj ett av de fyra alternativen för widgetens position på sidan: Höger, Vänster, Överkant, Underkant. Position % är den procentandel av placeringen där widgeten ska visas på webbläsarsidan (t.ex. "50 % nederkant" gör att widgeten visas halvvägs nedåt på sidan, "10 % vänster" gör att widgeten visas uppe till vänster på sidan, osv.).<br></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><strong>Widget Color</strong></td>
   <td colspan="1" rowspan="1"><p>Välj widgetfärgen från ett färgdiagram eller ange den som en RGB-färgkod. Du kan också välja genomskinlighetsnivån för widgetens bakgrund genom att flytta fältet längst ned i någon av riktningarna.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Widget-knapp</strong><br></p></td>
   <td colspan="1" rowspan="1">Anpassa själva widgetknappen.<br>Pil: Gör att du kan välja mellan flera olika ikoner i den högra listrutan. Den vänstra listrutan avgör dess färg.<br>Anpassad: Infoga URL:en för en värdbild. Godkända filtyper - .JPEG, .GIF (inklusive animerade), .PNG, .APNG, .SVG, .BMP.<br>Text: Widgeten kan vara text - anpassa färg, storlek och teckensnitt.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Fäst</strong></td>
   <td colspan="1">Om du väljer det här alternativet visas widgeten på alla webbsidor under besökarens session.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Minimera widget på kampanjvisning</strong></td>
   <td colspan="1">Infogar widgeten men behåller den minimerad, vilket kräver att användaren klickar på den för att maximera den.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Återställ standard </strong></td>
   <td colspan="1">Återställer den ursprungliga standardinställningen för widgeten genom att ställa in widgetfärgen på standardalternativet för genomskinligt grått.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Förhandsgranska på plats </strong></td>
   <td colspan="1">Förhandsgranska kampanjer innan de startas.<br>
    <ul>
     <li>URL - Ange en exempel-URL där kampanjen körs för att se ett förhandsgranskningsexempel på hur kampanjen skulle se ut live.</li>
     <li>Förhandsgranska - Klicka på <strong>Förhandsgranska </strong> för att öppna ett nytt fönster med exempel-URL:en för att se hur kampanjen reagerar (lägg till <a href="https://chrome.google.com/extensions/detail/ldiddonjplchallbngbccbfdfeldohkj?hl=en" rel="nofollow">Chrome-tillägget</a> för att få den bästa förhandsvisningen för webbkampanjen.) </li>
     <li>Dela - Använd knappen Dela för att skicka ett e-postmeddelande till en kollega med en länk för att se proxykampanjen.</li>
    </ul></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>**Vill du testa dina webbkampanjer?** En eller flera webbkampanjer kan [A/B-testas för optimala resultat](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Med funktionen [!UICONTROL Auto Tune] känner plattformen automatiskt igen de kampanjer som fungerar bättre, fortsätter med de mest konverterande kampanjerna och pausar de andra.

## Redigera en webbkampanj {#edit-a-web-campaign}

Klicka på [!UICONTROL Web Campaigns] på Campaign på sidan **[!UICONTROL Edit]**.

![](assets/image2016-11-4-13-3a2-3a20.png)

>[!NOTE]
>
>Använd [filterfunktionen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md) för att göra det enklare att hitta kampanjen.

## Klona en webbkampanj {#clone-a-web-campaign}

Se [Klona en webbkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Förhandsgranska en webbkampanj {#preview-a-web-campaign}

Klicka på [!UICONTROL Web Campaigns] på webbkampanjen som du vill förhandsgranska på sidan **[!UICONTROL Preview]**

![](assets/widget-campaign-preview-hand.png)

## Ta bort en webbkampanj {#delete-a-web-campaign}

1. Klicka på [!UICONTROL Web Campaigns] på webbkampanjen som du vill ta bort på sidan **[!UICONTROL Delete]**.

   ![](assets/widget-campaign-delete-hand.png)

1. Ett bekräftelsemeddelande visas som bekräftar om du vill ta bort webbkampanjen.

>[!MORELIKETHIS]
>
>* [Skapa en ny webbkampanj i zon](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Skapa en ny webbkampanj för dialogrutor](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
