---
description: Personhantering - Marketo Docs - produktdokumentation
title: Personhantering
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Personhantering {#person-management}

Det här är ett exempel på referens för arbetsflöden för personhantering med bästa praxis, med ett standardprogram för Marketo Engage, som hjälper dig att hantera personrörelser för poster i din Marketo-databas till din CRM. &quot;FRÅN&quot; ÄR DU I STÄLLET FÖR DIN??

INFOGA ANTECKNING HÄR - person/lead

Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontogruppen på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) sida.

**Kanalsammanfattning:**

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
   <td>01-medlem</td>
   <td>Inkluderande</td>
   <td>Standard</td>
  </tr>
 </tbody> 
</table>

Programmet innehåller följande resurser:

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
   <td>01-Synkronisera nya personer till CRM</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>02-Marknadsföringskvalificerad</td>
  </tr>
  <tr> 
   <td>E-post</td> 
   <td>E-postmall för snabbstart</td>
   <td>01- E-post - VARNING - MQL</td>
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
   * Skapa taggar i den här prenumerationen (standard) - _Rekommenderas_
   * Ignorera

* **Landningssidmall med samma namn**
   * Kopiera ursprunglig mall (standard) - _Rekommenderas_
   * Använd målmall

* **Bilder med samma namn**
   * Behåll båda filerna (standard) - _Rekommenderas_
   * Ersätt artikel i den här prenumerationen

* **E-postmallar med samma namn**
   * Behåll båda mallarna (standard) - _Rekommenderas_
   * Ersätt befintlig mall

SKÄRMBILD AV KONFLIKTREGLER

>[!TIP]
>
>Om du vill använda programmet som det är ska du behålla standardkonfliktreglerna markerade.

## Bästa praxis {#best-practices}

* Överväg att lägga till ytterligare smarta kampanjer för att hantera alla livscykelstatusbehov som ni kanske håller på att spåra i organisationen. Varje kampanj som byggs i det här programmet ska vara ett exempel på hur man bygger bästa praxis och inte specifik för alla användningsfall. Kom ihåg att uppdatera smarta kampanjer för att hantera din specifika process för livscykelhantering.

* Överväg att uppdatera namnkonventionen för det här programexemplet så att den överensstämmer med din.

* Om du vill ha mer hjälp eller hjälp med att anpassa ett program kontaktar du kontoteamet på Adobe eller går till [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) sida.
