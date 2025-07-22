---
unique-page-id: 4719400
description: Skapa en ny webbkampanj i zonen - Marketo Docs - Produktdokumentation
title: Skapa en ny webbkampanj i zonen
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Skapa en ny webbkampanj i zonen {#create-a-new-in-zone-web-campaign}

En webbkampanj är en anpassad reaktion som är kopplad till ett visst segment och kan vara en [dialogruta](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) på webbplatsen, en in zone-ersättning, en [widget-funktion](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) eller en e-postavisering. En In Zone-webbkampanj ersätter ett element på din webbplats baserat på Zone-id med innehåll eller grafiska banners.

## Skapa en webbkampanj i zonen {#create-an-in-zone-web-campaign}

1. Gå till **[!UICONTROL Web Campaigns]**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Välj **[!UICONTROL Create New Web Campaign].**

   ![](assets/create-new-web-campaign-hand.png)

1. Välj kampanjtypen **[!UICONTROL In Zone]**. Anpassa och lägg till en **[!UICONTROL Zone id].** Ställ in kampanjen på **[!UICONTROL Sticky]** och lägg till din kreativitet i redigeraren. Lägg till sidans URL för att förhandsgranska och klicka på **[!UICONTROL Preview]** för att se hur kampanjen kommer att reagera på din webbplats.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Vad är ett zon-ID?**
   >
   >Ett zon-ID är där du vill att webbkampanjen [!UICONTROL In Zone] ska placeras på webbplatsen. Om du vill hitta [!UICONTROL Zone ID] går du till webbplatsen och väljer det område som du vill ersätta med en webbkampanj och högerklickar. I Chrome är alternativet &quot;Inspect Element&quot; (Inspektera element). I andra webbläsare kan det variera.
   >
   >Sedan söker du efter det ID som är kopplat till det här avsnittet på webbplatsen, som är markerat eftersom du undersöker elementet. Om du till exempel högerklickar i Chrome och den markerade texten säger `<div id="featured-slider">` är &quot;featured-slider&quot; det som du bör skriva i &quot;zone id&quot;-avsnittet. Vanligtvis används &quot;div id&quot;, men alla ID:n kan också användas, till exempel h1 id, p id osv.

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
   <td colspan="1" rowspan="1"><p><strong> Toning</strong> </p></td> 
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
     <li>Enhet - Förhandsgranska hur kampanjen kommer att se ut på olika enheter: Stationär dator, Mobilt stående, Mobilt liggande, Stående surfplatta, Stående liggande.</li> 
     <li> Förhandsgranska - Klicka på <strong>Förhandsgranska</strong> för att öppna ett nytt fönster med exempel-URL:en för att se hur kampanjen reagerar.</li> 
     <li> Dela - Använd knappen Dela för att skicka ett e-postmeddelande till en kollega med en länk för att se proxykampanjen.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Snabba upp och förenkla processen för att skapa kampanjer genom att använda våra [inbyggda mallar](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) eller genom att [spara din befintliga kampanj](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) som en mall för återanvändning.

>[!NOTE]
>
>**Vill du testa dina webbkampanjer?** En eller flera webbkampanjer kan [A/B-testas för optimala resultat](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Med funktionen Automatisk justering känner plattformen automatiskt igen de kampanjer som presterar bättre, fortsätter med de mest konverterande kampanjerna och pausar de andra.

## Redigera en webbkampanj {#edit-a-web-campaign}

På sidan **Webbkampanjer** klickar du på **Redigera** i kampanjen.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Använd [filterfunktionen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md) för att göra det enklare att hitta kampanjen.

## Förhandsgranska en webbkampanj {#preview-a-web-campaign}

1. Klicka på [!UICONTROL Web Campaigns] på webbkampanjen som du vill visa på sidan **[!UICONTROL Preview]**.

   ![](assets/in-zone-web-campaign-preview.png)

## Klona en webbkampanj {#clone-a-web-campaign}

Se [Klona en webbkampanj](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Ta bort en webbkampanj {#delete-a-web-campaign}

1. Klicka på **[!UICONTROL Delete]** på den kampanj du vill ta bort på sidan Webbkampanjer.

   ![](assets/in-zone-web-campaign-delete.png)

1. Ett bekräftelsemeddelande visas som bekräftar om du vill ta bort kampanjen.

>[!MORELIKETHIS]
>
>* [Skapa en ny webbkampanj för widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Skapa en ny webbkampanj för dialogrutor](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
