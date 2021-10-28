---
description: Säljaktivitetsordlista - Marketo Docs - produktdokumentation
title: Ordlista för försäljningsaktivitet
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 0a1e913fd03415d3668c8a9d2200e2211bad5980
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 1%

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
  <th rowspan="9">Skicka e-postmeddelande</th>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <td>URL för försäljningsmall</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Namn på försäljningsmall</td>
 </tr>
 <tr>
  <td>E-postämne</td>
 </tr>
 <tr>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>Marketo-säljarens ID</td>
 </tr>
 <tr>
  <th rowspan="9">Open Sales Email</th>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
 <tr>
  <td>URL för försäljningsmall</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Namn på försäljningsmall</td>
 </tr>
 <tr>
  <td>E-postämne</td>
 </tr>
 <tr>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>Marketo-säljarens ID</td>
 </tr>
 <tr>
  <th rowspan="10">Klicka på E-postadress för försäljning</th>
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
  <td>URL för försäljningsmall</td>
 </tr>
 <tr>
  <td>URL för försäljningskampanj</td>
 </tr>
 <tr>
  <td>Namn på försäljningsmall</td>
 </tr>
 <tr>
  <td>E-postämne</td>
 </tr>
 <tr>
  <td>Namn på försäljningskampanj</td>
 </tr>
 <tr>
  <td>Marketo-säljarens ID</td>
 </tr>
<tr>
  <th rowspan="3">Svar på e-postadress</th>
  <td>Mottaget av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Marketo-säljarens ID</td>
 </tr>
 <tr>
  <th rowspan="11">Mottaget försäljningssamtal</th>
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
  <td>Försäljningssamtalets längd</td>
 </tr>
 <tr>
  <td>Inspelnings-URL för försäljningssamtal</td>
 </tr>
  <tr>
  <td>Försäljningssamtal besvarat av</td>
 </tr>
 <tr>
  <td>Marketo-säljarens ID</td>
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
   <td><strong>Detaljer</strong></td> 
   <td>Information om studsfelmeddelande.</td> 
  </tr> 
  <tr> 
   <td><strong>E-post</strong></td> 
   <td>E-postadress som studsade.</td> 
  </tr> 
  <tr> 
   <td><strong>Länk</strong></td> 
   <td>URL som användaren klickade på.</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo-säljarens ID</strong></td> 
   <td>Unikt ID för personpost i Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Mottaget av</strong></td> 
   <td>E-postadress till den person som skickade e-postmeddelandet.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningssamtal besvarat av</strong></td> 
   <td>Namn på den person som besvarade samtalet.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningssamtalets längd</strong></td> 
   <td>Anropets längd i sekunder.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningssamtal gjort av</strong></td> 
   <td>E-postadress till den säljare som ringde samtalet.</td> 
  </tr>
  <tr> 
   <td><strong>Inspelnings-URL för försäljningssamtal</strong></td> 
   <td>URL för samtalsinspelning.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningssamtalsstatus</strong></td> 
   <td>Sparar samtalets slutliga samtalsstatus, som omfattar: slutförd, inget svar, avbruten, misslyckades.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningssamtalets ämne</strong></td> 
   <td>Samtalsresultat som valts av en säljare i återförsäljaren.</td> 
  </tr>
  <tr> 
   <td><strong>Försäljningskampanj-ID</strong></td> 
   <td>Unikt ID för försäljningskampanjtillgång i Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Namn på försäljningskampanj</strong></td> 
   <td>Namn på försäljningskampanj.</td> 
  </tr>
  <tr> 
   <td><strong>URL för försäljningskampanj</strong></td> 
   <td>Sales Connect URL för Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>E-postämne för försäljning</strong></td> 
   <td>Ämnesrad för e-post.</td> 
  </tr>
  <tr> 
   <td><strong>Telefonnummer till försäljning har anropats</strong></td> 
   <td>Telefonnummer som anropas av Försäljning.</td> 
  </tr>
  <tr> 
   <td><strong>Namn på försäljningsmall</strong></td> 
   <td>Namn på e-postmall i Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>URL för försäljningsmall</strong></td> 
   <td>Sales Connect URL för e-postmall.</td> 
  </tr>
  <tr> 
   <td><strong>Skickat av</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td> 
  </tr> 
  <tr> 
   <td><strong>Källa</strong></td> 
   <td>Aktivitetens källa. Anges som "Tout" för Sales Connect-aktiviteter före Jan 22-utgåvan. Kommer att bli "Sales App" för Sales Connect-aktiviteter efter Jan 22-utgåvan.</td>
  </tr> 
  <tr> 
   <td><strong>Mall-ID</strong></td> 
   <td>När källan är Tout blir mall-ID:t Marketo Sales Connect Template ID. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td> 
  </tr> 
 </tbody> 
</table>
