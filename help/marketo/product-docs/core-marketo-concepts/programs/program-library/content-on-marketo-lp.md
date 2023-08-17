---
description: Innehåll på Marketo LP - Marketo Docs - produktdokumentation
title: Innehåll i Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# Innehåll i Marketo LP {#content-on-marketo-lp}

Programnamn: CT-YYY-MM-Content on Marketo LP

Denna exempelreferens är utformad för att vara ett innehållsprogram som använder en Marketo landningssida med ett Marketo-formulär som använder ett Marketo standardprogram. Formuläret är för att få tillgång till innehållet/erbjudandet. Länken till erbjudandet kan visas på tacksidan, skickas i ett tackmeddelande eller båda. Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontogruppen på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) sida.

**Kanalsammanfattning**

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

**Programmet innehåller följande resurser:**

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
   <td>Assets - Houses all creative assets 
<br/>(undermappar för e-post- och landningssidor)  </td>
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

SCREENSHOT - Programbild

**Bland mina token finns:**

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
<br/>Redigera den här innehållsbeskrivningen på programnivå, under fliken Mina token. 
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.TackYouPageURL?without the http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Se Instruktioner för programimport för standardkonfliktregler.

**Rekommenderade standardkonfliktregler för import:**

* Programtaggar
   * Skapa taggar i den här prenumerationen (standard) - Rekommenderas
   * Ignorera

* Landningssidmall med samma namn
   * Kopiera ursprunglig mall (standard)
   * Använd målmall - rekommenderas

* Bilder med samma namn
   * Behåll båda filerna (standard)
   * Ersätt objekt i den här prenumerationen - rekommenderas

* E-postmallar med samma namn
   * Behåll båda mallarna (standard)
   * Ersätt befintlig mall - Rekommenderas

SCREENSHOT - Bild av standardkonfliktregler

**Rekommenderade bästa metoder:**

* Marketo Consulting rekommenderar att man efter importen av innehållsprogrammet flyttar formuläret från en lokal resurs till en global resurs i Design Studio i Marketo Engage.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger även flexibilitet i regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet för att använda de varumärkesanpassade mallarna eller att uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp och sidfotsinformation.

* Överväg vid behov att uppdatera namnkonventionen för den här programmallen så att den anpassas till namnkonventionen.

* Glöm inte att uppdatera My Token-värdena i programmallen och varje gång du använder programmet efter behov.

* Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontoteamet på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) sida.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;02-engagerad&quot; för att spåra framgångar! Gör detta INNAN formuläret är live och e-post skickas.

>[!NOTE]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
