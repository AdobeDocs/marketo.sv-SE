---
description: CT-YYY-MM-Content Non-Marketo Landing Page - Marketo Docs - Product Documentation
title: CT-YYY-MM-Content Non-Marketo Landing Page
feature: Programs
exl-id: b7cf8e52-4f3f-44d7-ab4c-ad10fa0badc9
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 1%

---

# CT-YYY-MM-Content Non-Marketo Landing Page {#ct-yyyy-mm-content-non-marketo-landing-page}

Det här är ett exempel på ett innehållsprogram med ett Marketo Engage-formulär för att hämta innehåll på en icke-Marketo Engage landningssida som använder ett Marketo Engage-standardprogram. Det här programmet är avsett att fungera med ett Marketo Engage-formulär som är inbäddat på din webbplats. Länken till erbjudandet/innehållet kan skickas i ett tackmeddelande.

Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du Adobe Account Team eller går till sidan [Adobe Professional Services](https://business.adobe.com/se/customers/consulting-services/main.html){target="_blank"} .

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

## Programmet innehåller följande Assets {#program-contains-the-following-assets}

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
   <td>Formulär</td>
   <td> </td>
   <td>FM-Content Registration Form (global tillgång i Design Studio)</td>
  </tr>
  <tr>
   <td>Lokal rapport</td>
   <td> </td>
   <td>E-postprestanda</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>00-Capture Acquisition Program</td>
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

![](assets/ct-yyyy-mm-content-non-marketo-landing-page-1.png)

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
 </tbody>
</table>

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

## Bästa praxis {#best-practices}

* När innehållsprogrammet har importerats flyttar du formuläret från en lokal resurs till en global resurs i Design Studio.
   * Genom att minska antalet formulär och använda mer globalt material från Design Studio får du större skalbarhet i programdesignen och den administrativa styrningen. Det ger också flexibilitet för regelbundna uppdateringar av regelefterlevnad för fält, anmälningsspråk osv.

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den anpassas till namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;02-engagerad&quot; för att spåra framgångar! Gör detta _innan_ ditt formulär är live och e-postmeddelanden skickas.
