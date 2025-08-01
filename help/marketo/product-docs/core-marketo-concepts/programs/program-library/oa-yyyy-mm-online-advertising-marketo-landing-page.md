---
description: OA-YYYY-MM-Online Advertising Marketo landningssida - Marketo Docs - produktdokumentation
title: OA-YYY-MM-Online Advertising Marketo startsida
feature: Programs
exl-id: f7f17792-cc16-4a99-8683-68796770e42c
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# OA-YYY-MM-Online Advertising Marketo startsida {#oa-yyyy-mm-online-advertising-marketo-landing-page}

Detta är ett exempel på ett program för onlinereklam, som en Marketo Landing Page med registreringsblankett och ett Marketo standardprogram. Länken till erbjudandet kan visas på tacksidan, skickas i ett tackmeddelande eller båda.

Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du Adobe Account Team eller går till sidan [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} .

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
   <td>Online Advertising</td>
   <td>01 - Medlem
<br/>02 - Aktiverad - Slutförd</td>
   <td>Inkluderande</td>
   <td>Standard</td>
  </tr>
 </tbody>
</table>

## Programmet innehåller följande Assets {#program-contains-the-following-assets}

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
   <td>Registrering av FM-innehåll</td>
  </tr>
  <tr>
   <td>E-post</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>01-Email-Tack</td>
  </tr>
  <tr>
   <td>Landningssida</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>01 - LP - Registrering</td>
  </tr>
   <tr>
   <td>Landningssida</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>02 - LP - Tack</td>
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
   <td>00 - Capture Acquisition Program</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>01 - Ifyllt formulär</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>02 - Aktiverat (programmet lyckades)</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Assets - innehåller alla kreativa resurser
<br/>(undermappar för e-post och landningssidor)  </td>
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

![](assets/oa-yyyy-mm-online-advertising-marketo-landing-page-1.png)

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

SCREENSHOT OF PROGRAM

## Konfliktregler {#conflict-rules}

* **Programtaggar**
   * Skapa taggar i den här prenumerationen - _Rekommenderas_
   * Ignorera

* **Landningssidmall med samma namn**
   * Kopiera ursprunglig mall
   * Använd målmall - _Rekommenderad_

* **Bilder med samma namn**
   * Behåll båda filerna
   * Ersätt objekt i den här prenumerationen - _Rekommenderas_

* **E-postmallar med samma namn**
   * Behåll båda mallarna
   * Ersätt befintlig mall - _Rekommenderas_

SKÄRMBILD AV KONFLIKTREGLER

## Bästa praxis {#best-practices}

* När innehållsprogrammet har importerats flyttar du formuläret från en lokal resurs till en global resurs i Design Studio.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger även flexibilitet i regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Använd Programtaggar för att filtrera rapporter efter olika källor i Online Advertising.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;02 - Engaged (Program Success)&quot; för att spåra framgångar! Gör detta _innan_ ditt formulär är live och e-postmeddelanden skickas.

>[!IMPORTANT]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
