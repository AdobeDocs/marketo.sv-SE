---
unique-page-id: 7504238
description: Anpassade RTP-instrumentpaneler i Google Universal Analytics - Marketo Docs - produktdokumentation
title: Anpassade RTP-instrumentpaneler i Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Anpassade RTP-instrumentpaneler i Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrera RTP med Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

I det här inlägget beskrivs hur du konfigurerar RTP-instrumentpaneler i Google Universal Analytics (GUA). Data som skickas från RTP till GUA kan konfigureras som två separata anpassade kontrollpaneler som kallas:

* RTP B2B
* RTP-engagemang

## Konfigurera en anpassad kontrollpanel {#setting-up-a-custom-dashboard}

1. Logga in på Google Analytics. Klicka på **[!UICONTROL Reporting]** på den översta menyn. Klicka på **[!UICONTROL Dashboards]** och **[!UICONTROL New Dashboard]**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Välj **Tom arbetsyta**, lägg till ett **instrumentpanelsnamn** och klicka på **[!UICONTROL Create Dashboard]**.

1. Klicka på **[!UICONTROL Add Widget]** för att skapa en ny widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B-instrumentpanel {#rtp-b-b-dashboard}

Med den här kontrollpanelen kan användarna analysera webbplatsens prestanda ur B2B-perspektiv.

Det ger information om besökskälla och beteenden på plats per bransch, intäkt, storlek, kontobaserade listor och målsegment.

Kontrollpanelen består av tre kolumner

* Trafikkälla
* Segmentering
* Firmografisk detaljnivå

1. Skapa en ny instrumentpanel med namnet **RTP B2B Dashboard** och definiera följande widgetar:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table>
 <thead>
  <tr>
   <th>
    <div>
      Kolumn 1 - Trafikkällor
    </div></th>
   <th>
    <div> <strong>Kolumn 2 - Segmentering</strong>
    </div></th>
   <th>
    <div> <strong>Kolumn 3 - Inledande grafisk detaljnivå</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>Namn: Sessioner efter segment och kanaler</li>
     <li>Widgettyp: <span class="uicontrol">Bar</span><br></li>
     <li><span class="uicontrol">Skapa ett stapeldiagram som visar</span>: <span class="uicontrol">Session</span></li>
     <li><span class="uicontrol">Grupperad av</span>: <span class="uicontrol">Etikett för händelse</span></li>
     <li><span class="uicontrol">Pivot av</span>: <span class="uicontrol">Standardkanalgruppering</span></li>
     <li>Filter: <br><span class="uicontrol">Visa bara</span> | <span class="uicontrol"> Händelsekategori </span> (<span class="uicontrol">innehållande</span>) RTP-segment</li>
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: # RTP-segmenterade användare</li>
     <li>Typ: <span class="uicontrol">2.1 Metrisk</span></li>
     <li><span class="uicontrol">Visa följande mått</span>: <span class="uicontrol">Användare</span><br></li>
     <li>Filter: <br><span class="uicontrol">Visa bara</span> | <span class="uicontrol"> Händelsekategori </span> (som innehåller) RTP-segment</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: Sessioner efter bransch</li>
     <li>Typ: <span class="uicontrol">Cirkel</span><br></li>
     <li><span class="uicontrol">Skapa ett cirkeldiagram som visar</span>: <span class="uicontrol">Sessioner</span></li>
     <li><span class="uicontrol">Grupperad av</span> : <span class="uicontrol">RTP-Industry</span></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <th>
    <ul>
     <li><strong>Namn: Sessioner per bransch och kanaler</strong></li>
     <li><strong>Widgettyp: <span class="uicontrol">Bar</span></strong></li>
     <li><strong><span class="uicontrol">Skapa ett stapeldiagram som visar</span>: <span class="uicontrol">Session</span></strong></li>
     <li><strong><span class="uicontrol">Grupperad av</span>: <span class="uicontrol">RTP-Industry</span></strong></li>
     <li><strong><span class="uicontrol">Pivot av</span>: <span class="uicontrol">Standardkanalgruppering</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li>
    </ul></th>
   <th>
    <ul>
     <li><strong>Namn: Segmenterade sessioner per land</strong></li>
     <li><strong>Typ: <span class="uicontrol">Geomap</span></strong></li>
     <li><strong><span class="uicontrol">Rita valda mått</span>: <span class="uicontrol">Land</span> | <span class="uicontrol">Sessioner</span></strong></li>
     <li><strong><span class="uicontrol">Välj en region</span>: <span class="uicontrol">Världen</span></strong></li>
     <li><strong>Filter: <span class="uicontrol">Visa bara</span> | <span class="uicontrol"> Händelsekategori </span> (som innehåller) RTP-segment</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li><strong>Namn: Sessioner efter RTP-kategori</strong></li>
     <li><strong>Typ: <span class="uicontrol">Cirkel</span></strong></li>
     <li><strong><span class="uicontrol">Skapa ett cirkeldiagram som visar</span>: <span class="uicontrol">Sessioner</span></strong></li>
     <li><strong><span class="uicontrol">Grupperad av</span>: <span class="uicontrol">RTP-kategori</span></strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>Namn: Översta målsegment</li>
     <li>Typ: <span class="uicontrol">Bar</span></li>
     <li><span class="uicontrol">Skapa ett stapeldiagram som visar</span>: <span class="uicontrol">Användare</span></li>
     <li><span class="uicontrol">Grupperad av</span>: <span class="uicontrol">Händelseåtgärd</span></li>
     <li>Filter: <span class="uicontrol">Visa bara</span> | <span class="uicontrol"> Händelsekategori </span> (som innehåller) RTP-segment</li>
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th>
    <ul>
     <li>Namn: Sessioner efter RTP-Groups</li>
     <li>Typ: Stapel<br></li>
     <li>Skapa ett stapeldiagram som visar: Sessioner</li>
     <li>Grupperad av: RTP-Group</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
  </tr>
  <tr>
   <th> </th>
   <th>
    <ul>
     <li>Namn: Sessioner och mål efter övre segment</li>
     <li>Typ: Tabell<br></li>
     <li>Visa följande kolumner: <br>Händelseetikett | Sessioner | Målkonverteringsgrad</li>
     <li>Filter: <br>Visa bara | Händelsekategori (innehållande) RTP-segment</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th>
   <th> </th>
  </tr>
 </tbody>
</table>

## Instrumentpanel för RTP-engagemang {#rtp-engagement-dashboard}

På den här kontrollpanelen kan användare analysera sina RTP-kampanjer och rekommendationer. Den ger en jämförelse av genomskinlighet. sessionens längd och antal sidor per session mellan:

* Olåst
* Engagerade (visningar och klickningar på en personaliserad kampanj)
* Klicka på rekommendationsmotorn och det rekommenderade innehållet

Skapa en ny instrumentpanel med namnet **RTP Engagement Dashboard** och definiera följande widgetar:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table>
 <thead>
  <tr>
   <th>
    <div> <strong>Kolumn 1 - Kampanjexponering</strong>
    </div></th>
   <th>
    <div> <strong>Kampanjklickning i kolumn 2</strong>
    </div></th>
   <th>
    <div> <strong>Kolumn 3, rekommendationsmotor</strong>
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>
    <ul>
     <li>Namn: <strong>Totalt CTA (engagemang)</strong></li>
     <li>Typ: <strong>2.1 Mått </strong></li>
     <li>Visa följande mått: <strong>Totalt antal händelser</strong></li>
     <li>Filter:<br><strong>[visa endast] Händelsekategori (innehåller): RTP-kampanjer</strong><br><strong>[visa endast] Händelseåtgärd (exakt matchning): Impression</strong>[visa inte] Händelseetikett (innehåller): #</li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: <strong>Totalt CTA (klickbart)</strong></li>
     <li>Typ: <strong>2.1 Mått </strong></li>
     <li>Visa följande mått: <strong>Totalt antal händelser</strong></li>
     <li>Filter:<br><strong>[visa endast] Händelsekategori (innehåller): RTP-Campaigns</strong><br><strong>[visa endast] Händelseåtgärd (exakt matchning): Klicka </strong><strong>[visa inte] Etikett för händelse (innehåller): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: <strong>CRE - totalt antal klick</strong></li>
     <li>Typ: <strong><span class="uicontrol">2.1 Metrisk</span></strong><br></li>
     <li><span class="uicontrol">Visa följande mått</span>: <strong><span class="uicontrol">Sidor</span></strong></li>
     <li>Filter: <strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Sida</span> (<span class="uicontrol">innehåller</span>): rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td colspan="1">
    <ul>
     <li>Namn: <strong>Medel. Sessionsvaraktighet (engagemang)</strong></li>
     <li>Typ: <strong>2.1 Mått </strong></li>
     <li>Visa följande mått: <strong>Medel. Sessionsvaraktighet </strong></li>
     <li>Filter:<br><strong>[visa endast] Händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[visa endast] Händelseåtgärd (exakt matchning): intrycket </strong><strong>[visa inte] Händelseetikett (innehåller): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>Namn: <strong>Medel. Sessionsvaraktighet (klickning) </strong></li>
     <li>Typ: <strong>2.1 Mått </strong></li>
     <li>Visa följande mått: <strong>Medel. Sessionsvaraktighet </strong></li>
     <li>Filter:<br><strong>[visa endast] Händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[visa endast] Händelseåtgärd (exakt matchning): klickningar </strong><strong>[visa inte] Händelseetikett (innehåller): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td colspan="1">
    <ul>
     <li>Namn: <strong>CRE - Rekommenderat toppinnehåll</strong></li>
     <li>Typ: <strong><span class="uicontrol">Tabell</span></strong><br></li>
     <li><span class="uicontrol">Visa följande kolumner</span>: <br><strong><span class="uicontrol">Sidtitel</span> | <span class="uicontrol">Sidvisningar</span></strong><br></li>
     <li>Filter:<br>Filter: <strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Sida</span> (<span class="uicontrol">innehåller</span>): rcmd</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>Namn: <strong>Sidor/session (engagemang)</strong></li>
     <li>Typ: <strong><span class="uicontrol">2.1 Mått </span> </strong></li>
     <li><span class="uicontrol">Visa följande mått</span>: <strong><span class="uicontrol">Sidor/session</span></strong></li>
     <li>Filter:<br><strong>[<span class="uicontrol">visa bara</span>] <span class="uicontrol">händelsekategori</span> (<span class="uicontrol">matchar exakt</span>): RTP-kampanjer</strong></li>
     <li><strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Händelseåtgärd</span> (<span class="uicontrol">matchar exakt</span>): intryck</strong></li>
     <li><strong>[<span class="uicontrol">visa inte</span>] <span class="uicontrol">Händelseetikett</span> (<span class="uicontrol">innehåller</span>): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: <strong>Sidor/session (klickning)</strong></li>
     <li>Typ: <strong>2.1 Mått </strong></li>
     <li>Visa följande mått: <strong>Sidor/session</strong></li>
     <li>Filter:<br><strong>[endast visa] Händelsekategori (exakt matchning): RTP-kampanjer</strong></li>
     <li><strong>[endast show] Händelseåtgärd (exakt matchning): klickningar</strong></li>
     <li><strong>[visa inte] Händelseetikett (innehåller): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
  <tr>
   <td>
    <ul>
     <li>Namn: <strong>Impressions av CTA</strong></li>
     <li>Typ: <strong><span class="uicontrol">Tabell</span></strong></li>
     <li><span class="uicontrol">Visa följande kolumner</span>: <strong><span class="uicontrol">Etikett för händelse</span> | <span class="uicontrol">Totalt antal händelser</span> | <span class="uicontrol">Användare</span></strong></li>
     <li>Filter:<br><strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Händelsekategori</span> (<span class="uicontrol">exakt matchande</span>): RTP-kampanjer</strong><br><strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Händelseåtgärd</span> (<span class="uicontrol">exakt matchning</span>): intryck</strong><strong>[<span class="uicontrol"> 17}visa inte</span>] <span class="uicontrol">händelseetikett</span> (<span class="uicontrol">innehåller</span>): #</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td>
    <ul>
     <li>Namn: <strong>Klicka genom CTA</strong></li>
     <li>Typ: <strong><span class="uicontrol">Tabell</span></strong></li>
     <li><span class="uicontrol">Visa följande kolumner</span>: <strong><span class="uicontrol">Etikett för händelse</span> | <span class="uicontrol">Totalt antal händelser</span> | <span class="uicontrol">Användare</span></strong></li>
     <li>Filter:<br><strong>[<span class="uicontrol">show</span>] <span class="uicontrol">Händelsekategori</span> (<span class="uicontrol">exakt matchning</span>): RTP-kampanjer</strong><br><strong>[<span class="uicontrol">visa endast</span>] <span class="uicontrol">Händelseåtgärd</span> (<span class="uicontrol">exakt matchning</span>): klicka</strong></li>
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td>
   <td> </td>
  </tr>
 </tbody>
</table>

>[!MORELIKETHIS]
>
>[Integrera RTP med Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Anpassade RTP-rapporter i Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
