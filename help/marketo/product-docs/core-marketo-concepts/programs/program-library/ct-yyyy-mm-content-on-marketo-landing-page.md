---
description: CT-YYY-MM-Content on Marketo LP - Marketo Docs - Product Documentation
title: CT-YYY-MM-Content on Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# CT-YYY-MM-Content on Marketo Landing Page {#ct-yyyy-mm-content-on-marketo-landing-page}

Det här exemplet är utformat som ett innehållsprogram som använder en landningssida för Marketo Engage med ett Marketo Engage-formulär som använder ett standardprogram för Marketo Engage. Formuläret är för att få tillgång till innehållet/erbjudandet. Länken till erbjudandet kan visas på tacksidan, skickas i ett tackmeddelande eller båda.

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
   <td>Webbinnehåll</td> 
   <td>01-medlem 
<br/>02-Engaged-Success</td>
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
   <td>E-post</td> 
   <td>E-postmall för snabbstart</td>
   <td>01-Email-Tack</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td>Lathund för snabbstart</td>
   <td>01 - LP - Registrering</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td>Lathund för snabbstart</td>
   <td>02 - LP - Tack</td>
  </tr>
  <tr> 
   <td>Formulär</td> 
   <td> </td>
   <td>Innehållsregistreringsformulär</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>E-postprestanda</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>Prestanda för landningssida</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01-ifyllt formulär</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02-engagerade (programmet lyckades)</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Resurser - innehåller alla kreativa resurser 
<br/>(undermappar för e-post- och landningssidor)  </td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Kampanjer - innehåller alla smarta kampanjer</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Rapporter</td>
  </tr>
 </tbody> 
</table>

SCREENSHOT OF PROGRAM

## Mina token inkluderade {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tokentyp</th> 
   <th>Tokennamn</th>
   <th>Värde</th>
  </tr> 
  <tr> 
   <td>RTF</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Dubbelklicka för mer information  
<br/><code><--My Content Description Here--></code> 
<br/>Redigera den här innehållsbeskrivningen på programnivå på fliken Mina token. 
<br/>Du kommer att lära dig: 
<li>Punkt 1</li>
<li>Punkt 2</li>
<li>Punkt 3</li></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
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

SKÄRMBILD AV KONFLIKTREGLER

## Bästa praxis {#best-practices}

* När innehållsprogrammet har importerats flyttar du formuläret från en lokal resurs till en global resurs i Design Studio.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger även flexibilitet i regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;02-engagerad&quot; för att spåra framgångar! Gör så här _före_ formuläret är live och e-postmeddelanden skickas.

>[!IMPORTANT]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
