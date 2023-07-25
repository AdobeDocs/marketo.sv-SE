---
unique-page-id: 4719400
description: Skapa en ny webbkampanj i zonen - Marketo Docs - Produktdokumentation
title: Skapa en ny webbkampanj i zonen
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Skapa en ny webbkampanj i zonen {#create-a-new-in-zone-web-campaign}

En webbkampanj är en anpassad reaktion som är kopplad till ett visst segment och kan vara en [dialogruta](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) på din webbplats, en in-zone-ersättning, en [widgetfunktion](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) eller en e-postavisering. En In Zone-webbkampanj ersätter ett element på din webbplats baserat på Zone-id med innehåll eller grafiska banners.

## Skapa en webbkampanj i zonen {#create-an-in-zone-web-campaign}

1. Gå till **Webbkampanjer**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Välj **Skapa ny webbkampanj.**

   ![](assets/create-new-web-campaign-hand.png)

1. Välj **I zon** kampanjtyp. Anpassa och lägga till en **Zon-id.** Ställ in kampanjen på **Fäst** och lägg in din kreativitet i redigeraren. Lägg till URL-adressen till sidan som ska förhandsgranskas och klicka på **Förhandsgranska** för att se hur kampanjen kommer att reagera på er webbplats.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Vad är ett zon-ID?**
   >
   >Ett zon-ID är där du vill att webbkampanjen In Zone ska placeras på plats. Om du vill hitta ett &quot;zon-ID&quot; går du till webbplatsen och väljer det område som du vill ersätta med en webbkampanj och högerklickar. I Chrome är alternativet&quot;Inspect Element&quot;, vilket kan variera i andra webbläsare.
   >
   >Sedan vill du hitta det ID som är kopplat till det här avsnittet på webbplatsen, som är markerat eftersom du undersöker elementet. Om du t.ex. högerklickar i Chrome visas den markerade texten `<div id="featured-slider">` &quot;featured-slider&quot; är det du ska skriva i avsnittet &quot;zone id&quot;. Vanligtvis används &quot;div id&quot;, men alla ID:n kan också användas, till exempel h1 id, p id osv.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Namn</th> 
   <th colspan="1" rowspan="1">Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> Zon-id </strong></td> 
   <td colspan="1" rowspan="1"><p>Ange namnet på det ID som finns i HTML-koden för det webbplatselement som kampanjen ersätter.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fäst </strong></p></td> 
   <td colspan="1" rowspan="1">Kryssrutan Fäst är markerad som standard för In Zone-kampanjen och behåller In Zone-kampanjen i sin Zon-id-position under besökarens session på webbplatsen. Vi rekommenderar att alltid ha en In Zone inställd på Sticky.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Tona</strong> </p></td> 
   <td colspan="1" rowspan="1">Om du markerar kryssrutan Använd effekt och toning tonas zonens id-område ut på webbplatsen. Om In Zone är en grafisk banderoll läses sidan först in och sedan aktiveras kampanjen med en toningseffekt.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Glidande</strong></td> 
   <td colspan="1">Om du markerar kryssrutan Använd effekt och alternativet Glidande visas en glidning för zonen med id-nummer på webbplatsen. Om In Zone är en grafisk banderoll läses sidan först in och sedan aktiveras kampanjen med en glidande effekt från vänster till höger.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> RTF-redigerare  </strong></td> 
   <td colspan="1">Med RTF-redigeraren kan du formatera, länka och infoga bilder. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Läs mer här</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Förhandsgranska på plats   </strong></td> 
   <td colspan="1">Förhandsgranska kampanjer innan de lanseras. <br> 
    <ul> 
     <li> URL - Ange en exempel-URL där kampanjen körs för att se ett förhandsgranskningsexempel på hur kampanjen skulle se ut live.</li> 
     <li>Enhet - Förhandsgranska hur kampanjen kommer att visas per enhet: Stationär dator, Mobile Portrait, Mobile Landscape, Tablet Portrait, Portrait Landscape.</li> 
     <li> Förhandsgranska - klicka <strong>Förhandsgranska</strong> om du vill öppna ett nytt fönster med exempel-URL:en för att se hur kampanjen reagerar.</li> 
     <li> Dela - Använd knappen Dela för att skicka ett e-postmeddelande till en kollega med en länk för att se proxykampanjen.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Snabba upp och förenkla processen för att skapa kampanjer med våra [inbyggda mallar](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) eller av [spara befintlig kampanj](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) som en mall för återanvändning.

>[!NOTE]
>
>**Vill du testa webbkampanjer?** En eller flera webbkampanjer kan [A/B-testad för optimala resultat](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Med funktionen Automatisk justering känner plattformen automatiskt igen de kampanjer som presterar bättre, fortsätter med de mest konverterande kampanjerna och pausar de andra.

## Redigera en webbkampanj {#edit-a-web-campaign}

Från **Webbkampanjer** sida, klicka **Redigera** på Campaign.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Om du vill göra det enklare att hitta den kampanj du vill ha använder du [filterfunktion](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Förhandsgranska en webbkampanj {#preview-a-web-campaign}

1. På webbkampanjsidan klickar du på **Förhandsgranska** på den webbkampanj du vill se.

   ![](assets/in-zone-web-campaign-preview.png)

## Klona en webbkampanj {#clone-a-web-campaign}

Se [Klona en webbkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Ta bort en webbkampanj {#delete-a-web-campaign}

1. På webbkampanjsidan klickar du på **Ta bort** på den kampanj du vill ta bort.

   ![](assets/in-zone-web-campaign-delete.png)

1. Ett bekräftelsemeddelande visas som bekräftar om du vill ta bort kampanjen.

>[!MORELIKETHIS]
>
>* [Skapa en ny webbkampanj för widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Skapa en ny webbkampanj för dialog](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
