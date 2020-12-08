---
unique-page-id: 1146999
description: Token för intressanta ögonblick - Marketo Docs - produktdokumentation
title: Token för intressanta ögonblick
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Token för intressanta ögonblick {#tokens-for-interesting-moments}

>[!NOTE]
>
>**Förutsättningar**
>
>* Lär dig använda flödessteget [Intressant stund](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).
>* Läs mer om [variabler](http://docs.marketo.com/display/docs/tokens).

>



## Tillgängliga token {#available-tokens}

Kolla in [Token Overview](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) för att se alla tokens du kan sätta i en intressant stund.

## Utlösartoken {#trigger-tokens}

Beroende på vilken utlösare som används i en smart kampanj blir ytterligare utlösartoken tillgängliga.

* `{{trigger.Trigger Name}}` som alltid är själva utlösaren. Till exempel: Klicka på Länk i e-post.
* `{{trigger.Name}}` är namnet på den tillgång som utlöste kampanjen. Till exempel: Klicka på Länk på webbsida om du vill se själva webbadressen, ämne för Salesforce-utlösare osv.
* Ytterligare utlösare är tillgängliga baserat på begränsningar, som listas nedan:

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
  </tr> 
  <tr> 
   <td>Klicka på Länk i e-post</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-poststudsar hårt</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-poststudsar mjuka</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-post levereras</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Öppnar e-post</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Avbeställ e-post</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Klicka på Länk i e-postadress för försäljning</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-post för skickad försäljning</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Öppnar e-postadress för försäljning</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-postförsäljning mottagen</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">E-postförsäljning studsade</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
  <tr> 
   <td>Fyller i formulär</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Besök webbsida*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Om den inte har en check ![(tick)](assets/check.svg) returnerar den en tom sträng (ingenting) i det intressanta ögonblicket.

*Utlösaren **besöker webbsidan** har några extra tokens:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testa alltid intressanta ögonblick för att säkerställa att de återges som du tänkt dig.
>
>Se även till att det är intressant för säljaren, inte bara för dig. ![(blinka)](assets/wink.svg)>

