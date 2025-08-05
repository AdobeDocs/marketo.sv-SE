---
description: OP-Data Management - Marketo Docs - produktdokumentation
title: OP-Data Management
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# OP-Data Management {#op-data-management}

Det här är ett exempel på enkla arbetsflöden för datahantering med bästa praxis, med ett standardprogram, som hjälper dig att hantera datakonsekvens för poster i din Marketo Engage-databas.

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
   <td>Operativ</td>
   <td>01-medlem</td>
   <td>Operativ</td>
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
   <td>Smart Campaign</td>
   <td> </td>
   <td>Normalisera land - USA</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Normalisera land - Storbritannien</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ange Blocklist till Sant</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ange är partner till sant</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Listimport</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Live Event</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Online Advertising</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Trade Show</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Webbinnehåll</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Webbförfrågan</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Webbinarium</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från listimport</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från Live Event</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från Advertising online</td>
  </tr>
  <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från Trade Show</td>
  </tr>
   <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från webbinnehåll</td>
  </tr>
   <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från webbförfrågan</td>
  </tr>
   <tr>
   <td>Smart Campaign</td>
   <td> </td>
   <td>Ny person från webbinariet</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Person Source Nightly Batch (för högtrafikinstanser)</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Person Source Triggered (för lågtrafikinstanser)</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Capture Person Source</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Normalisering</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Posthantering</td>
  </tr>
  <tr>
   <td>Mapp</td>
   <td> </td>
   <td>Blockeringslista</td>
  </tr>
 </tbody>
</table>

![](assets/op-data-management-1.png)

## Konfliktregler {#conflict-rules}

* **Programtaggar**
   * Skapa taggar i den här prenumerationen - _Rekommenderas_
   * Ignorera

* **Landningssidmall med samma namn**
   * Kopiera ursprunglig mall - _Rekommenderad_
   * Använd målmall

* **Bilder med samma namn**
   * Behåll båda filerna - _Rekommenderas_
   * Ersätt artikel i den här prenumerationen

* **E-postmallar med samma namn**
   * Behåll båda mallarna - _Rekommenderas_
   * Ersätt befintlig mall

## Bästa praxis {#best-practices}

* Varje kampanj som byggs är tänkt att vara ett exempel på hur ni bygger de bästa metoderna och inte specifikt för era användningsfall. Kom ihåg att uppdatera smarta kampanjer för att hantera era specifika utmaningar och datamängder.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.
