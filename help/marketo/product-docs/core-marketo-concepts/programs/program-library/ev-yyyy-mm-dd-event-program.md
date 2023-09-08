---
description: EV-YYYY-MM-DD-Event Program - Marketo Docs - Produktdokumentation
title: EV-YYYY-MM-DD-Event-programmet
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 1%

---

# EV-YYYY-MM-DD-Event-programmet {#ev-yyyy-mm-dd-event-program}

Det här är ett exempel på ett eventprogram med en registreringssida, tre inbjudningsmejl och uppföljningsmejl som använder ett Marketo Engage Event Program. Passar för alla evenemang där du behöver registrera dig, inklusive reklamutskick, luncher, middagar eller presentationer vid mässor.

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
   <td>Händelse</td> 
   <td>01-Inbjuden 
<br/>02-Väntelistat
<br/>03-Registrerad
<br/>04-Ingen visning
<br/>05-Attended-Success</td>
   <td>Inkluderande</td>
   <td>Händelse</td>
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
   <td>01-Email-Tack</td>
  </tr>
   <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>02a- E-post - inbjudan</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>02b - E-post - påminnelse om inbjudan</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>02c- Email - Invitation Reminder Last Chance</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>03 - E-post - påminnelse att delta</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>04a - E-post - uppföljning - Bifogad</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-postmall för snabbstart</a></td>
   <td>04b - E-post - Uppföljning - NoShow</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>01a - LP - Registrering</td>
  </tr>
  <tr> 
   <td>Landningssida</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Lathund för snabbstart</a></td>
   <td>01b - LP - Tack</td>
  </tr>
  <tr> 
   <td>Formulär</td> 
   <td> </td>
   <td>Registrering av FM-händelse</td>
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
   <td>01 - Processregistrering</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02a - Skicka inbjudan</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02b - Skicka påminnelse om inbjudan</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02c - Skicka inbjudan sista chansen</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>03 - Skicka påminnelse till Bifoga</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>04 - Deltas (programmet lyckades)</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>05 - Skicka uppföljningsmejl</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Assets - Houses all creative assets 
<br/>(undermappar för e-post- och landningssidor)</td>
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

![](assets/ev-yyyy-mm-dd-event-program-1.png)

## Mina token inkluderade {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tokentyp</th> 
   <th>Tokennamn</th>
   <th>Värde</th>
  </tr>
  <tr> 
   <td>Kalenderfil</td> 
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Dubbelklicka för detaljer</td>
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
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
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
   <td><code>{{my.Event-Location-Line1}}</code></td>
   <td><code><--XYZ Hotel--></code></td>
  </tr>
   <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line2}}</code></td>
   <td><code><--ABC Room--></code></td>
  </tr>
   <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line3}}</code></td>
   <td><code><--1234 Anystreet--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line4}}</code></td>
   <td><code><--Anytown, ZZ 99999--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Type}}</code></td>
   <td>Live Event</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-Download}}</code></td>
   <td>my.DownloadURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-Registration}}</code></td>
   <td>my.RegistrationPageURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>my.ThankYouPageURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker1-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker1-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker2-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker2-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker3-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
 <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker3-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
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
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger även flexibilitet i regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;06-Attended (Program Success)&quot; för att spåra lyckade försök! Gör så här _före_ formuläret är live och e-postmeddelanden skickas.

>[!IMPORTANT]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
