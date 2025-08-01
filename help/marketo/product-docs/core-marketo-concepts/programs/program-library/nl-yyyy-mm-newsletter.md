---
description: NL-YYYY-MM-Newsletter - Marketo Docs - Produktdokumentation
title: NL-ÅÅÅ-MM-Newsletter
feature: Programs
exl-id: bce05e0f-e288-4614-9d05-c14844615454
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---

# NL-ÅÅÅ-MM-Newsletter {#nl-yyyy-mm-newsletter}

I det här exemplet skickas ett nyhetsbrev via e-post med Marketo Engage e-postprogram. E-postmeddelandet kan innehålla ett A/B-test eller inte.

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
   <td>Nyhetsbrev</td>
   <td>01-medlem
<br/>02-Engaged-Success</td>
   <td>Inkluderande</td>
   <td>E-post</td>
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
   <td>01 - E-post</td>
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
   <td>01 - Aktiverat (programmet lyckades)</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Assets - Alla kreativa resurser
<br/>(undermappar för e-post)  </td>
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

![](assets/nl-yyyy-mm-newsletter-1.png)

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
   * Använd målmall - _Rekommenderad_

* **Bilder med samma namn**
   * Behåll båda filerna
   * Ersätt objekt i den här prenumerationen - _Rekommenderas_

* **E-postmallar med samma namn**
   * Behåll båda mallarna
   * Ersätt befintlig mall - _Rekommenderas_

## Bästa praxis {#best-practices}

* Överväg att uppdatera mallarna i det importerade programmet så att de använder de varumärkesanpassade mallarna, eller uppdatera den importerade mallen så att den återspeglar ert varumärke genom att lägga till ett fragment eller lämplig logotyp/sidfotsinformation.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.

>[!NOTE]
>
>Kom ihåg att uppdatera My Token-värdena i programmallen och vid behov varje gång du använder programmet.

>[!TIP]
>
>Glöm inte att aktivera kampanjen&quot;10-engagerad&quot; för att spåra framgångar! Gör detta _innan_ ditt formulär är live och e-postmeddelanden skickas.
