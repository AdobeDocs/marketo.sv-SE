---
description: Konfigurera databasavsnittet för den nya instansen Marketo Engage.
title: Nya bästa metoder för instanser - Databaskontrolllista
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 7805983cdaff0b99a38aefc2c2467b53f3386da3
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# God praxis för nya instanser: Databaskontrolllista {#new-instance-best-practices-database-checklist}

I avsnittet Databas hittar du nyckelattributen för personerna i instansen. Lär dig mer om de nödvändiga stegen för att navigera i olika listor och segmenteringar i din databas samt för att hantera personposter.

Kom ihåg [ladda ned checklistor](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) och spåra dina framsteg.

## Systemets smarta listor {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Alla personer</td>
    <td><li>Bestäm hur du implementerar en 1:1-synkronisering med CRM eller använd filter för att begränsa vem som ska flytta från system till system och när.</li> 
    <li>Granska det totala antalet personer och marknadsföringsbara personer i din <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank">Marketo Engage-databas</a>.</li></td>
  </tr>
  <tr>
    <td>Blockeringslista</td>
    <td><li>Definiera villkor för blockeringslista. Överväg att lägga till konkurrentens domäner i din <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">blockeringslista</a> för att hindra dem från att ta emot e-postmeddelanden.</li></td>
  </tr>
  <tr>
    <td>Marknadsföring har pausats</td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marknadsföring har pausats</a> kriterier.</li></td>
  </tr>
  <tr>
    <td>Avrundade e-postadresser </td>
    <td><li>Definiera villkor för studsade e-postadresser.</li>
    <li>Granska personerna i kategorin"E-post ogiltig" och kontrollera om deras e-postmeddelanden behöver skickas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">manuellt återställa</a>.</li></td>
  </tr>
  <tr>
    <td>Möjliga dubbletter</td>
    <td><li>Granska personer i listan Möjliga dubbletter.</li> 
    <li>Definiera er strategi för hantering av dubbletter för att avgöra om ni vill <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">sammanfoga personer manuellt</a>.</li>  
    <li>Om du har en CRM-integrering kan du definiera en process och ett konto för <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">effekten av att sammanfoga leads i CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Inget förvärvsprogram</td>
    <td><li>Skapa kampanjer i era programmallar som skapar ett inköpsprogram, särskilt om ni använder globala formulär.</li></td>
  </tr>
  <tr>
    <td>Avbeställ</td>
    <td><li>Granska villkoren för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank">Avbeställ</a>.</li></td>
  </tr>
</tbody>
</table>

## Gruppera smarta listor {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gruppera smarta listor</td>
    <td><li>Var medveten om att du har skapat smarta grupplistor så att det inte finns dubblettlistor.</li>
    <li>Håll reda på huvudlistorna i databasen.</li></td>
  </tr>
</tbody>
</table>

## Segmentering {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentering</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank">Skapa segmenteringar</a> baserat på era affärsbehov. Varje prenumeration är begränsad till 20 segmenteringar och 100 segment inom varje segmentering.</li></td>
  </tr>
</tbody>
</table>