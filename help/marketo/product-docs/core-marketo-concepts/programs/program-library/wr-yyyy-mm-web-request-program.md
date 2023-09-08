---
description: WR-YYYY-MM-Web Request Program - Marketo Docs - Produktdokumentation
title: WR-YYYY-MM-Web Request Program
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# WR-YYYY-MM-Web Request Program {#wr-yyyy-mm-web-request-program}

Det här är ett exempelprogram som är idealiskt för kontaktförfrågningar, offertförfrågningar, demonstrationsförfrågningar eller testförfrågningar med hjälp av ett Marketo Engage-standardprogram. Kan användas med Marketo landningssidor eller som ett inbäddat formulär på landningssidor som inte kommer från Marketo. Ett varningsmeddelande skickas till en angiven person när formuläret skickas in.

Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontogruppen på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} sida.

## Kanalsammanfattning {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Kanal</th> 
   <th>Status för medlemskap</th>
   <th>Analysbeteende</th>
   <th>Programtyp</th>
  </tr> 
  <tr> 
   <td>Webbförfrågan</td> 
   <td>01 - Aktiverad - Slutförd</td>
   <td>Inkluderande</td>
   <td>Standard</td>
  </tr>
 </tbody> 
</table>

## Programmet innehåller följande resurser {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Typ</th> 
   <th>Mallnamn</th>
   <th>Resursnamn</th>
  </tr>
  <tr> 
   <td>Formulär</td> 
   <td> </td>
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>Alert-WebRequest</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>01 - LP - Begäran</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>02 - LP - Tack</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>Prestanda för landningssida</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Ny person från webbförfrågan</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Ny person från webbinariet</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Assets - Houses all creative assets 
<br/>(undermappar för varningar och landningssidor)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Kampanjer - omfattar alla smarta kampanjer</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Rapporter</td>
  </tr>
 </tbody> 
</table>

![](assets/wr-yyyy-mm-web-request-program-1.png)

## Mina token inkluderade {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tokentyp</th> 
   <th>Tokennamn</th>
   <th>Värde</th>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Request-Type}}</code></td>
   <td>Kontakta oss</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.TackYouPageURL?without the http://</td>
  </tr>
 </tbody> 
</table>

## Konfliktregler {#conflict-rules}

* **Programtaggar**
   * Skapa taggar i den här prenumerationen - _Rekommenderas_
   * Ignorera

* **Landningssidmall med samma namn**
   * Kopiera ursprunglig mall
   * Använd målmall - _Rekommenderas_

* **Bilder med samma namn**
   * Behåll båda filerna
   * Ersätt artikel i den här prenumerationen - _Rekommenderas_

* **E-postmallar med samma namn**
   * Behåll båda mallarna
   * Ersätt befintlig mall - _Rekommenderas_

## Bästa praxis {#best-practices}

* När du har importerat webbinariet flyttar du formuläret från en lokal resurs till en global resurs som finns i Design Studio.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger också flexibilitet för regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den anpassas till namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!IMPORTANT]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
