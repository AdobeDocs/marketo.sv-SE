---
description: OP-Lead Management - Marketo Docs - produktdokumentation
title: OP-Lead Management
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: ea276734b6d277f4a3548a9a697e1c7ed4c30e2d
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# OP-Lead Management {#op-lead-management}

Det här är ett exempel på arbetsflöden för bästa praxis för leadhantering, med ett Marketo Engage-standardprogram, som hjälper dig att hantera poster i din Marketo Engage-databas till din CRM.

>[!NOTE]
>
>I Marketo Engage kallas poster i din databas personer/person. Leadhanteringen i det här exemplet gäller posterna i CRM.

Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontogruppen på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) sida.

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
   <td>01 - Synkronisera nya personer till CRM</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02 - Kvalificerad marknadsföring</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td>E-postmall för snabbstart</td>
   <td>01 - E-post - VARNING - MQL</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>Kampanjer</td>
  </tr>
  <tr> 
   <td>Mapp</td> 
   <td> </td>
   <td>E-postavisering</td>
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

* Överväg att lägga till ytterligare smarta kampanjer för att hantera alla livscykelstatusbehov som ni kanske håller på att spåra i organisationen. Varje kampanj som byggs i det här programmet ska vara ett exempel på hur man bygger bästa praxis och inte specifik för alla användningsfall. Kom ihåg att uppdatera smarta kampanjer för att hantera era specifika livscykelhanteringsprocesser.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med din.
