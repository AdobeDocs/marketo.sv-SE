---
unique-page-id: 7504238
description: Anpassade RTP-instrumentpaneler i Google Universal Analytics - Marketo Docs - Produktdokumentation
title: Anpassade RTP-instrumentpaneler i Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---


# Anpassade RTP-instrumentpaneler i Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrera RTP med Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

I det här inlägget beskrivs hur du konfigurerar RTP-instrumentpaneler i Google Universal Analytics (GUA).  Data som skickas från RTP till GUA kan konfigureras som två separata anpassade kontrollpaneler som kallas:

* RTP B2B
* RTP-engagemang

## Konfigurera en anpassad kontrollpanel {#setting-up-a-custom-dashboard}

1. Logga in på Google Analytics. Klicka på **Reporting **på den översta menyn. Klicka på **Kontrollpaneler **och **+Ny anpassad kontrollpanel.**

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Välj **Tom arbetsyta**, lägg till ett **instrumentpanelsnamn** och klicka på **Skapa instrumentpanel**.

1. Klicka på **Lägg till widget** för att skapa en ny widget.\
   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B-instrumentpanel {#rtp-b-b-dashboard}

Med den här kontrollpanelen kan användarna analysera webbplatsens prestanda ur B2B-perspektiv.

Det ger information om besökskälla och beteenden på plats per bransch, intäkt, storlek, kontobaserade listor och målsegment.

Kontrollpanelen består av tre kolumner

* Trafikkälla
* Segmentering
* Firmografisk detaljnivå

1. Skapa en ny instrumentpanel med namnet **RTP B2B Dashboard **och definiera följande widgetar:

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
    <div> <strong>Kolumn 3 - Firmografisk detaljnivå</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Namn: Sessioner efter segment och kanaler</li> 
     <li>Widgettyp: Liggande<br></li> 
     <li>Skapa ett stapeldiagram som visar: Session</li> 
     <li>Grupperad av: Etikett för händelse</li> 
     <li>Pivotera efter: Standardkanalgruppering</li> 
     <li>Filter: <br>Visa endast | Händelsekategori (innehållande) RTP-segment</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Namn: Antal RTP-segmenterade användare</li> 
     <li>Typ: 2.1 Metrisk</li> 
     <li>Visa följande mått: Användare<br></li> 
     <li>Filter: <br>Visa endast | Händelsekategori (innehållande) RTP-segment</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Namn: Sessioner per bransch</li> 
     <li>Typ: Cirkel<br></li> 
     <li>Skapa ett cirkeldiagram som visar: Sessioner</li> 
     <li>Grupperad av: RTP-Bransch</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Namn: Sessioner per bransch och kanal</strong></li> 
     <li><strong>Widgettyp: Liggande</strong></li> 
     <li><strong>Skapa ett stapeldiagram som visar: Session</strong></li> 
     <li><strong>Grupperad av: RTP-Bransch</strong></li> 
     <li><strong>Pivotera efter: Standardkanalgruppering</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Namn: Segmenterade sessioner per land</strong></li> 
     <li><strong>Typ: Geomap</strong></li> 
     <li><strong>Rita valda mått: Land | Sessioner</strong></li> 
     <li><strong>Välj en region: Världen</strong></li> 
     <li><strong>Filter: Visa endast | Händelsekategori (innehållande) RTP-segment</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Namn: Sessioner efter RTP-kategori</strong></li> 
     <li><strong>Typ: Cirkel</strong></li> 
     <li><strong>Skapa ett cirkeldiagram som visar: Sessioner</strong></li> 
     <li><strong>Grupperad av: RTP-kategori</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Namn: Övre målsegment</li> 
     <li>Typ: Liggande</li> 
     <li>Skapa ett stapeldiagram som visar: Användare</li> 
     <li>Grupperad av: Händelseåtgärd</li> 
     <li>Filter: Visa endast | Händelsekategori (innehållande) RTP-segment</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Namn: Sessioner av RTP-Groups</li> 
     <li>Typ: Liggande<br></li> 
     <li>Skapa ett stapeldiagram som visar: Sessioner</li> 
     <li>Grupperad av: RTP-grupp</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Namn: Sessioner och mål per segment</li> 
     <li>Typ: Tabell<br></li> 
     <li>Visa följande kolumner: <br>Händelseetikett | Sessioner | Målkonverteringsgrad</li> 
     <li>Filter: <br>Visa endast | Händelsekategori (innehållande) RTP-segment</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Instrumentpanel för RTP-engagemang {#rtp-engagement-dashboard}

På den här kontrollpanelen kan användare analysera sina RTP-kampanjer och rekommendationer. Den ger en jämförelse av genomskinlighet. sessionens längd och antal sidor per session mellan:

* 

   * Olåst
   * Engagerade (visningar och klickningar på en personaliserad kampanj)
   * Klicka på rekommendationsmotorn och det rekommenderade innehållet

Skapa en ny instrumentpanel som kallas **RTP Engagement Dashboard** och definiera följande widgetar:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Kolumn 1 Kampanjexponering</strong> 
    </div></th> 
   <th> 
    <div> <strong>Klickfrekvens för kolumn 2-kampanjer</strong> 
    </div></th> 
   <th> 
    <div> <strong>Rekommendationsmotor för kolumn 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Namn: <strong>Totalt CTA (engagemang)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Totalt antal händelser</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (innehåller): RTP-Campaigns</strong><br><strong>[show only show] Händelseåtgärd (exakt matchning): Händelseetiketten Impression</strong><strong>[visa inte] (som innehåller): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Namn: <strong>Total CTA (klickfrekvens)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Totalt antal händelser</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (innehåller): RTP-Campaigns</strong><br><strong>[endast show] Händelseåtgärd (exakt matchning): Klicka</strong><strong>[visa inte] på händelseetiketten (innehåller): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Namn: <strong>CRE - totalt antal klick</strong></li> 
     <li>Typ: <strong>2.1 Metrisk</strong><br></li> 
     <li>Visa följande mått: <strong>Sidor</strong></li> 
     <li>Filter: <strong>[endast visa] sida (innehåller): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Namn: <strong>Medel. Sessionslängd (engagemang)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Medel. Sessionsvaraktighet</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[endast show] Händelseåtgärd (exakt matchning): intrycket</strong><strong>[visa inte] Händelseetikett (innehåller): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Namn: <strong>Medel. Sessionslängd (klickning)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Medel. Sessionsvaraktighet</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[endast show] Händelseåtgärd (exakt matchning): click</strong><strong>[don't show] Event Label (containing): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Namn: <strong>CRE - Rekommenderat innehåll i toppklass</strong></li> 
     <li>Typ: <strong>Tabell</strong><br></li> 
     <li>Visa följande kolumner: <br><strong>Sidrubrik | Sidor</strong><br></li> 
     <li>filter:<br>Filter: <strong>[endast visa] sida (innehåller): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Namn: <strong>Sidor/session (engagemang)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Sidor/session</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-kampanjer</strong></li> 
     <li><strong>[show only] Händelseåtgärd (exakt matchning): intrycket</strong></li> 
     <li><strong>[don't show] Event Label (containing): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Namn: <strong>Sidor/session (klickning)</strong></li> 
     <li>Typ: <strong>2.1 Metrisk </strong></li> 
     <li>Visa följande mått: <strong>Sidor/session</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-kampanjer</strong></li> 
     <li><strong>[show only] Händelseåtgärd (exakt matchning): klickningar</strong></li> 
     <li><strong>[don't show] Event Label (containing): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Namn: <strong>Impressions av CTA</strong></li> 
     <li>Typ: <strong>Tabell</strong></li> 
     <li>Visa följande kolumner: <strong>Händelseetikett | Totalt antal händelser | Användare</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[endast show] Händelseåtgärd (exakt matchning): intrycket</strong><strong>[visa inte] Händelseetikett (innehåller): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Namn: <strong>Klickar igenom av CTA</strong></li> 
     <li>Typ: <strong>Tabell</strong></li> 
     <li>Visa följande kolumner: <strong>Händelseetikett | Totalt antal händelser | Användare</strong></li> 
     <li>Filter:<br><strong>[endast visa] händelsekategori (exakt matchning): RTP-Campaigns</strong><br><strong>[endast show] Händelseåtgärd (exakt matchning): klickningar</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Integrera RTP med Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)
>
>[Anpassade RTP-rapporter i Google Universal Analytics](custom-rtp-reports-in-google-universal-analytics.md)

