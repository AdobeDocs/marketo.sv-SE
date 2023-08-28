---
description: OP-Acquisition-API - Marketo Docs - Produktdokumentation
title: OP-Acquisition-API
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# OP-Acquisition-API {#op-acquisition-api}

Det här exempelprogrammet är avsett för operativa processer för att spåra förvärv av poster från API-källor med hjälp av ett Marketo Engage-standardprogram.

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

## Programmet innehåller följande resurser {#program-contains-the-following-assets}

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
   <td>Ange anskaffning - batch</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Ange förvärv - utlösare</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Kampanjer (innehåller alla smarta kampanjer)</td>
  </tr>
 </tbody> 
</table>

SCREENSHOT OF PROGRAM

## Konfliktregler {#conflict-rules}

* **Programtaggar**
   * Skapa taggar i den här prenumerationen - _Rekommenderas_
   * Ignorera

* **Landningssidmall med samma namn**
   * Kopiera ursprunglig mall - _Rekommenderas_
   * Använd målmall

* **Bilder med samma namn**
   * Behåll båda filerna - _Rekommenderas_
   * Ersätt artikel i den här prenumerationen

* **E-postmallar med samma namn**
   * Behåll båda mallarna - _Rekommenderas_
   * Ersätt befintlig mall

SKÄRMBILD AV KONFLIKTREGLER

## Bästa praxis {#best-practices}

* Kör batchkampanjen först om du behöver komma ikapp i datahanteringen.

* Överväg att använda liknande program för att säkerställa anpassning till bästa praxis i alla indatakällor för att inkludera CRM- eller dataintegreringar.

* Inom kanalspecifika marknadsföringssatsningar måste ni se till att ni kan samla in förvärv vid behov.
