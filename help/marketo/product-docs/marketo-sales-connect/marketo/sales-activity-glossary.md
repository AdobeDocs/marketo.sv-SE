---
description: Säljaktivitetsordlista - Marketo Docs - produktdokumentation
title: Säljaktivitetsordlista
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---

# Säljaktivitetsordlista {#sales-activity-glossary}

När en säljare i Sales Connect lägger till ett lead till en säljkonferens, skickar ett e-postmeddelande till dem eller ringer en aktivitet loggas det under Marketo aktivitetshistorik. När leadet dessutom interagerar med e-post loggas även öppningar, klickningar och svar.

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
  <td>Marketo-säljares person-ID</td>
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
  <td>Marketo-säljares person-ID</td>
 </tr>
 <tr>
  <th rowspan="10">Klicka på E-postadress</th>
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
  <td>Marketo-säljares person-ID</td>
 </tr>
<tr>
  <th rowspan="3">Svar på e-postadress</th>
  <td>Mottaget av</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>Marketo-säljares person-ID</td>
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
  <td>Marketo-säljares person-ID</td>
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
 <tr>
  <th rowspan="5">E-postutfall för försäljning</th>
  <td>Information</td>
 </tr>
 <tr>
  <td>E-post</td>
 </tr>
 <tr>
  <td>Skickat av</td>
 </tr>
 <tr>
  <td>Marketo-säljares person-ID</td>
 </tr>
 <tr>
  <td>Mall-ID</td>
 </tr>
</table>

## Beskrivning {#descriptions}

<table> 
 <tr>
  <th>Attribut</th>
  <th>Beskrivning</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>Information</strong></td> 
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
   <td><strong>Marketo-säljares person-ID</strong></td> 
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
   <td>Unikt ID för tillgång till säljkampanj i försäljningsanslutning.</td> 
  </tr>
  <tr> 
   <td><strong>Namn på försäljningskampanj</strong></td> 
   <td>Namn på säljkampanj.</td> 
  </tr>
  <tr> 
   <td><strong>URL för försäljningskampanj</strong></td> 
   <td>Sales Connect URL för Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>E-postämne för försäljning</strong></td> 
   <td>Ärenderad e-postadress följd av ett unikt ID (t.ex. Min ärenderad (MSC-12345678)</td> 
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
   <td>Source om aktiviteten. Anger som "Tout" för Sales Connect-aktiviteter före oktot 21-versionen. Kommer att bli "Sales App" för Sales Connect-aktiviteter efter okt. 21-versionen.</td>
  </tr> 
  <tr> 
   <td><strong>Mall-ID</strong></td> 
   <td>När källan är Tout blir mall-ID:t Marketo Sales Connect Template ID. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td> 
  </tr> 
 </tbody> 
</table>
