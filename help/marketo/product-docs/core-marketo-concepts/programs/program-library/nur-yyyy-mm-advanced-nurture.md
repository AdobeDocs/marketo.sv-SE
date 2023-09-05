---
description: NUR-YYYY-MM-Advanced Nurture - Marketo Docs - produktdokumentation
title: NUR-YYYY-MM-Advanced Nurture
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# NUR-YYYY-MM-Advanced Nurture {#nur-yyyy-mm-advanced-nurture}

Detta är ett exempel på avancerade utbildningsprogram som använder Marketo Engage Engagement Program. Kapslade e-postprogram hindrar människor från att ta emot innehåll som de redan har konsumerat eller styr vilken typ av innehåll de ska använda i varje ström. Attributrapportering kan köras för varje enskilt kapslat e-postprogram. Kanaler: &quot;Inturer&quot; och en dedikerad &quot;Inurture Email&quot;-kanal för kapslade e-postprogram skickar ett nyhetsbrev via ett Marketo Engage-e-postprogram. E-postmeddelandet kan innehålla ett A/B-test eller inte.

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
  <tr> 
   <td>E-postmeddelande</td> 
   <td>01 - Hoppa över 
<br/>02 - Skickat
<br/>03 - Aktiverad - Slutförd</td>
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
   <td>Kapslat program</td> 
   <td> </td>
   <td>01 - Ämne X</td>
  </tr>
  <tr> 
   <td>Kapslat program</td> 
   <td> </td>
   <td>02 - Ämne Y</td>
  </tr>
  <tr> 
   <td>Kapslat program</td> 
   <td> </td>
   <td>03 - Ämne Z</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>01 - E-post (live i kapslade program)</td>
  </tr>
   <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>02 - E-post (live i kapslade program)</td>
  </tr>
   <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>03 - E-post (live i kapslade program)</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>E-postprestanda</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>E-postlänkens prestanda</td>
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
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 - Hoppa över e-post (finns i varje kapslat program)</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 - Skicka e-post (finns i varje kapslat program)</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 - Engaged-Success (finns i varje kapslat program)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Resurser (Innehåller kapslade program och resursmappar finns också i kapslade program för att innehålla e-post)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Kapslade program (bor i resursmappen)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Campaigns - Placerar alla smarta kampanjer i det överordnade strukturprogrammet och kampanjmapparna finns också i varje kapslat program</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Rapporter</td>
  </tr>
 </tbody> 
</table>

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

SCREENSHOT OF PROGRAM

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

SKÄRMBILD AV KONFLIKTREGLER

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
