---
unique-page-id: 7504218
description: Anpassade RTP-rapporter i Google Universal Analytics - Marketo Docs - Produktdokumentation
title: Anpassade RTP-rapporter i Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Anpassade RTP-rapporter i Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrera RTP med Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

I den här artikeln beskrivs hur du konfigurerar anpassade RTP-rapporter för Google Universal Analytics (GUA).  Data som skickas från RTP till GUA kan ställas in som två separata anpassade rapporter som kallas:

* RTP B2B
* RTP-engagemang

## Konfigurera en anpassad rapport {#setting-up-a-custom-report}

1. Logga in på Google Analytics.

1. Klicka på **Anpassning** i den övre menyn.

1. Klicka **+Ny anpassad rapport**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B-rapport {#rtp-b-b-report}

1. Namnge rapporten **RTP B2B-rapport**.

1. Namnge den första fliken **Bransch**.

>[!NOTE]
>
>Du kommer att **Duplicera den här fliken** och skapa andra liknande - steg 5)

1. Välj **Utforskaren** rapporttyp.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. I **Måttgrupper** väljer du de mätvärden som är relevanta för ditt företag.

   a. Vi rekommenderar följande:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplicera den här fliken fyra gånger och namnge dem:

   1. **Bransch**
   1. **Grupp**
   1. **Kategori**
   1. **ABM**
   1. **Organisationer**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. I **Dimension - nedladdningar** anger de relevanta måtten för varje flik enligt nedan.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Fliknamn 
    </div></th> 
   <th> 
    <div>
      Dimension - nedladdningar
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Bransch</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Grupp</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Kategori</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organisationer</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Ange inga filter och ställ in den här rapporten som tillgänglig för **Alla webbplatsdata** (eller ändra om det är relevant för det specifika Analytics-kontot).

1. Klicka **Spara**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP-engagemangsrapport {#rtp-engagement-report}

1. Namnge rapporten **RTP-engagemangsrapport**.

1. Ange det första fliknamnet till **Alla engagemang**.

>[!NOTE]
>
>Du kommer att duplicera den här fliken och skapa andra liknande - steg 5)

1. Välj **Utforskaren** rapporttyp.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. I avsnittet Måttgrupper väljer du de mått som är relevanta för ditt företag. Här är en rekommendation:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplicera den här fliken fyra gånger och namnge dem:

   1. **Alla engagemang**
   1. **Engagemang per bransch**
   1. **Engagemang per grupp**
   1. **Engagemang efter kategori**
   1. **Åtagande av ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. I **Dimension - nedladdningar** anger du de relevanta måtten för varje flik enligt nedan:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Fliknamn 
    </div></th> 
   <th> 
    <div>
      Dimension - nedladdningar 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Alla engagemang</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Åtagande av ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagemang efter kategori</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagemang per grupp</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagemang per bransch</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Ange följande filter:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Fält 
    </div></th> 
   <th> 
    <div>
      Matcha typ 
    </div></th> 
   <th> 
    <div>
      Värden 
    </div></th> 
   <th colspan="1"> 
    <div>
      Kommentarer 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Inkludera</p></td> 
   <td><p>Händelsekategori</p></td> 
   <td>Regex</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtrerar alla andra anpassade händelser som inte är relaterade till RTP</td> 
  </tr> 
  <tr> 
   <td>Exkludera</td> 
   <td>Händelseetikett</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Gör att du kan filtrera från din rapportkampanj med # i kampanjnamnet</td> 
  </tr> 
 </tbody> 
</table>

1. Ange att den här rapporten ska vara tillgänglig för **Alla webbplatsdata** (eller ändra vid behov).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Klicka **Spara**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrera RTP med Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Anpassade RTP-instrumentpaneler i Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
