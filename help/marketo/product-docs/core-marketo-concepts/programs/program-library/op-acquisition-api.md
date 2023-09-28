---
description: OP-Acquisition-API - Marketo Docs - Produktdokumentation
title: OP-Acquisition-API
feature: Programs
exl-id: 1d6ec686-af0b-46a9-b428-1520b671ca24
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '171'
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

![](assets/op-acquisition-api-1.png)

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

## Bästa praxis {#best-practices}

* Kör batchkampanjen först om du behöver komma ikapp i datahanteringen.

* Överväg att använda liknande program för att säkerställa anpassning till bästa praxis i alla indatakällor för att inkludera CRM- eller dataintegreringar.

* Inom kanalspecifika marknadsföringssatsningar måste ni se till att ni kan samla in förvärv vid behov.
