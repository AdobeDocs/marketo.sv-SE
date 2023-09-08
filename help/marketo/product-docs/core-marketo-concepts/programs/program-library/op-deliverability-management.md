---
description: OP-Deliverability Management - Marketo Docs - produktdokumentation
title: OP-Deliverability Management
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# OP-Deliverability Management {#op-deliverability-management}

Det här är ett exempel på arbetsflöden för hantering av bästa praxis för leverans med ett standardprogram för Marketo Engage, för att granska ditt nuvarande e-postleveranstillstånd och hantera kroniska studsar och andra som inte svarar.

>[!NOTE]
>
>Kräver det anpassade strängfältet&quot;Orsak till pausad marknadsföring&quot; för import. [Läs mer](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

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
   <td>Operativ</td> 
   <td>01-medlem</td>
   <td>Operativ</td>
   <td>Standard</td>
  </tr>
 </tbody> 
</table>

## Obligatoriska fält {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Typ</th> 
   <th>Eget namn</th>
   <th>API Name</th>
  </tr>
  <tr> 
   <td>Sträng</td> 
   <td>Orsak till pausad marknadsföring</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Pausa kroniska svar på marknadsföring</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Marknadsföring Pausa kroniskt studsade e-postmeddelanden</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Återställ E-post ogiltig efter e-postuppdatering</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Återställ"Marknadsföring pausad" efter e-postuppdatering</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Hantera</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Granska</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

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

* Varje kampanj som byggs är tänkt att vara ett exempel på hur ni bygger de bästa metoderna och inte specifikt för era användningsfall. Kom ihåg att uppdatera smarta kampanjer för att hantera era specifika utmaningar och datamängder.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med namnkonventionen.
