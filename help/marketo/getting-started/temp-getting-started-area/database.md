---
description: Konfigurera databasavsnittet för en ny Marketo Engage-instans.
title: NY AREA-DATABAS
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: a9d902bf40e6193838a931ecb96a080bae098d68
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# NYTT OMRÅDE: Databaskontrolllista {#new-area-database-checklist}

Lär dig hur du implementerar de nödvändiga stegen för databasavsnittet i din nya Marketo Engage-instans. Följ guiderna&quot;Implementera en ny instans&quot; och håll reda på pågående uppgifter för att hjälpa dig att konfigurera instansen för långsiktig effektivitet.

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
    <td><li>Definiera villkor för blockeringslista. Överväg att lägga till konkurrentens domäner i <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">blockeringslista</a> för att hindra dem från att ta emot e-postmeddelanden.</li></td>
  </tr>
  <tr>
    <td>Marknadsföring har pausats</td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank">Marknadsföring har pausats</a> kriterier.</li></td>
  </tr>
  <tr>
    <td>Avrundade e-postadresser </td>
    <td><li>Definiera villkor för studsade e-postadresser.</li>
    <li>Granska personerna i kategorin Email Invalid (E-post är ogiltig) och om deras e-postmeddelanden måste skickas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">manuellt återställa</a>.</li></td>
  </tr>
  <tr>
    <td>Möjliga dubbletter</td>
    <td><li>Granska personer i listan Möjliga dubbletter.</li> 
    <li>Definiera er strategi för hantering av dubbletter för att avgöra om ni vill <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">sammanfoga personer manuellt</a>.</li>  
    <li>Om du har en CRM-integrering kan du definiera en process och ett konto för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank">effekten av att sammanfoga leads i CRM</a>.</li></td>
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
