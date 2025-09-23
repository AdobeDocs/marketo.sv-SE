---
description: Ärvd checklista för instansdatabas - Marketo Docs - produktdokumentation
title: Ärvd checklista för instansdatabas
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Ärvd instans: Databaskontrolllista {#inherited-instance-database-checklist}

Förstå det totala antalet personer, säljbara personer och de främsta leverantörerna i prenumerationen. Kom ihåg att [hämta checklistorna](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) och spåra dina framsteg.

## Systemets smarta listor {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr>
  <tr>
   <td>Alla personer</td>
   <td><li>Hur många personer finns i <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">databasen</a>?</li>
<li>Om databasen är nästan full, rekommenderar din företagspolicy att du utökar databasstorleken eller rensar bort historiska data?</li>
<li>Är er övergripande databas minst 85 % marknadsmässig?
<br/>     Om ditt värde ligger under det här tröskelvärdet kan du titta på de andra systemsmarta listorna (Blockeringslista, Marketing Suspended, Duplicates, Unsubscribe) med större kontroll.</li></td>
  </tr>
  <tr>
   <td>Avbeställ</td>
   <td><li>Vilka villkor gäller för <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">personer som inte har prenumererat</a>? Finns det för många personer som inte har prenumererat?</li>
<li>Anpassar era avanmälningsmetoder er efter era sekretessbestämmelser?</li>
<li>Är din inställning för att avbryta prenumerationen uppdaterad? Hur länge finns det kvar poster i din databas som icke-marknadsförbara?</li></td>
  </tr>
  <tr>
   <td>Marknadsföring har pausats</td>
   <td><li>Vilka villkor gäller för <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marknadsföringen har pausats</a>? Finns det för många personer som är avstängda från marknadsföring?</li>
<li>Hur länge finns det kvar uppgifter om statusen för Marketing Suspended?</li>
<p>Exempel på uppskjuten användning av marknadsföring: personposter som aktivt deltar i försäljning i sista-minuten-möjligheter som du vill undertrycka marknadskommunikation för.</td>
  </tr>
   <tr>
   <td>Blockeringslista</td>
   <td><li>Vilka villkor gäller för <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">blockeringslistning av poster</a>? Finns det för många blocklist?</li></td>
  </tr>
  <tr>
   <td>Avrundade e-postadresser</td>
   <td><li>Har du många <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">personer som studsade</a> i din databas?
   <br/>     I så fall bör du överväga varför.</li></td></li></td>
  </tr>
  <tr>
   <td>Möjliga dubbletter</td>
   <td><li>Hur många <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">poster </a> som kan dupliceras finns det?
   <br/>     Överväg att ta bort eller sammanfoga dem.</li></td>
  </tr>
   <tr>
   <td>Inget förvärvsprogram</td>
   <td><li>Hur många personer har inte ett <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">förvärvsprogram</a>?
   <br/>     Om det är mycket, överväg att undersöka varför.</li></td>
  </tr>
 </tbody>
</table>

## Smarta listor {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr>
  <tr>
   <td>Smarta listor</td>
   <td><li>Hur många <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">smarta listor</a> finns det? Hur används de i den här instansen?</li>
   <p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! I avsnittet Databas genereras gruppsmarta listor av användare och systemsmarta listor är standardlistor som skapas av Marketo Engage.
<li>Är listorna ordnade i en sammanhängande mappstruktur?
<br/>     Om du har överblivna listor bör du överväga att ordna trädet så att det blir enkelt att hitta resurser.</li>
<p><img src="assets/tip-icon.png" alt="ikonen för tips">TIPS: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Arkivering</a> Smarta listor som inte längre behövs hjälper till med organisation och prestanda.</td>
  </tr>
 </tbody>
</table>

## Statiska listor {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr>
  <tr>
   <td>Statiska listor</td>
   <td><li>Hur många <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">statiska listor</a> finns det? Hur används de i den här instansen?</li>
   <p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Grupplistor är statiska listor i databasavsnittet.</td>
  </tr>
 </tbody>
</table>

## Segmenteringar {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr>
  <tr>
   <td>Segmenteringar</td>
   <td><li>Vilka <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segment</a> finns det? Hur används de?</li>
<li>Är för många personer i <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">standardsegmenten</a>?</li>
<li>Finns det någon segmentering för den marknadsföringsbara publiken?
<br/>     Om inte kan du skapa en.</li></td>
  </tr>
 </tbody>
</table>
