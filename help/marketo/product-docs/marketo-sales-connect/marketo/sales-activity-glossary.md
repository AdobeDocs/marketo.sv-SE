---
description: Säljaktivitetsordlista - Marketo Docs - produktdokumentation
title: Ordlista för försäljningsaktivitet
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 3%

---

# Ordlista för försäljningsaktivitet {#sales-activity-glossary}

I Sales Connect, när en säljare: lägger till ett lead till en säljkonferens, skickar ett e-postmeddelande till dem eller ringer en aktivitet. Den loggas under Marketo aktivitetshistorik. När leadet dessutom interagerar med e-post loggas även öppningar, klickningar och svar.

Aktiviteterna nedan loggas till Marketo från Sales Connect.

>[!NOTE]
>
>Dessa aktiviteter och attribut är tillgängliga för användning från våra REST- och Bulk-API:er.

## Verksamhet {#activities}

<table>
 <tr>
  <th>Försäljningsaktivitet</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="3">Skicka e-postmeddelande</th>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <th rowspan="3">Open Sales Email</th>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <th rowspan="4">Klicka på E-postadress för försäljning</th>
  <td>Länk</td>
 </tr>
 <tr>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <th rowspan="2">Mottaget e-postmeddelande</th>
  <td>Mottaget av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <th rowspan="4">E-postförsäljning studsade</th>
  <td>Detaljer</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <td>E-post</td>
 </tr>
 <tr>
  <td>Skickat av</td>
 </tr>
 <tr>
  <th rowspan="7">Mottaget försäljningssamtal</th>
  <td>Försäljningssamtal gjort av</td>
 </tr>
 <tr>
  <td>Försäljningssamtalsstatus</td>
 </tr>
 <tr>
  <td>Försäljningssamtalets ämne</td>
 </tr>
 <tr>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Telefonnummer till försäljning har anropats</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <th rowspan="6">Lägg till i försäljningskampanj</th>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>Försäljningssamtalsstatus</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Försäljningskampanj-ID</td>
 </tr>
 <tr>
  <th rowspan="6">Ta bort från försäljningskampanj</th>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>Försäljningssamtalsstatus</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Försäljningskampanj-ID</td>
 </tr>
</table>

## Beskrivningar {#descriptions}

<table> 
 <tr>
  <th>Attribut</th>
  <th>Beskrivning</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>Skickat av</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td> 
  </tr> 
  <tr> 
   <td><strong>Källa</strong></td> 
   <td>Aktivitetens källa. Anger som "Tout" för Sales Connect-aktiviteter.</td> 
  </tr> 
  <tr> 
   <td><strong>Mall-ID</strong></td> 
   <td>När källan är Tout blir mall-ID:t Marketo Sales Connect Template ID. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td> 
  </tr> 
  <tr> 
   <td><strong>Mottaget av</strong></td> 
   <td>E-postadress till den person som skickade e-postmeddelandet.</td> 
  </tr> 
  <tr> 
   <td><strong>Detaljer</strong></td> 
   <td>Information om studsfelmeddelande.</td> 
  </tr> 
  <tr> 
   <td><strong>E-post</strong></td> 
   <td>E-postadress som studsade.</td> 
  </tr> 
 </tbody> 
</table>