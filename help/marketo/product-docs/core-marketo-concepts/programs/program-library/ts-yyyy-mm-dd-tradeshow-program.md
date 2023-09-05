---
description: TS-YYYY-MM-DD-Tradeshow Program - Marketo Docs - Produktdokumentation
title: TS-YYYY-MM-DD Tradeshow Program
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 569f61f15a9bdeb31b3a60b237f0c19aad68800a
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# TS-YYYY-MM-DD Tradeshow Program {#ts-yyyy-mm-dd-tradeshow-program}

Detta är ett exempel på ett program för bildspel med inbjudningar och uppföljningsmejl som använder ett Marketo Engage Event Program.

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
   <br/>04-Besökta monter
   <br/>05-engagerad vid Show - lyckades
   <br/>06-engagerade vid postshow - lyckades</td>
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
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>E-postprestanda</td>
  </tr>
  <tr> 
   <td>Lokal rapport</td> 
   <td> </td>
   <td>Programprestanda</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>00 - Capture Acquisition Program</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>01 - Skicka inbjudan</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 - Skicka uppföljningsmejl</td>
  </tr>
   <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>03 - Engagerad av uppföljningsmejl (lyckades)</td>
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
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
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
   <td>Varumärke</td>
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

* När du har importerat webbinariet flyttar du formuläret från en lokal resurs till en global resurs som finns i Design Studio.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger även flexibilitet i regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;03 - Inaktiverad av uppföljningsmeddelande via e-post (programmet lyckades)&quot; för att spåra om det lyckades! Gör så här _före_ dina e-postmeddelanden skickas.

>[!IMPORTANT]
>
>Mina token som refererar till en URL kan inte innehålla http:// eller https://, annars fungerar inte länken korrekt i resursen.
