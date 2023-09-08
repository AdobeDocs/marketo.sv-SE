---
description: NUR-YYY-MM-Simple Inurture - Marketo Docs - produktdokumentation
title: NUR-YYY-MM-Simple Nurture
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# NUR-YYY-MM-Simple Nurture {#nur-yyyy-mm-simple-nurture}

Det här är ett exempel på enkla strukturprogram, som använder Marketo Engage Engagement Program, med cadenced content to drip over time to your database while utilizing streams to guide records through travel based on behavior based on behavior.

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
   <td>Nätur</td> 
   <td>01 - Medlem 
<br/>02 - Aktiverad - Slutförd</td>
   <td>Inkluderande</td>
   <td>Engagemang</td>
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
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>01 - E-post</td>
  </tr>
   <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>02 - E-post</td>
  </tr>
   <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>03 - E-post</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>E-postprestanda</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>Prestanda för engagemangsström</td>
  </tr>
  <tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 - Lägg till i struktur</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 - Pausa Struktur</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>03 - Återuppta struktur</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>04 - Aktiverat (programmet lyckades)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Assets - Houses all creative assets
   <br/>(undermappar för e-post)</td>
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

![](assets/nur-yyyy-mm-simple-nurture-1.png)

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
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
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

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

* Se till att du har regler för att pausa och återuppta din vårdnad. Dessa smarta kampanjer bör aktiveras eller schemaläggas innan engagemangsprogrammet aktiveras.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;04 - engagerad (programmet lyckades)&quot; för att spåra lyckade försök! Gör så här _före_ dina e-postmeddelanden skickas.
