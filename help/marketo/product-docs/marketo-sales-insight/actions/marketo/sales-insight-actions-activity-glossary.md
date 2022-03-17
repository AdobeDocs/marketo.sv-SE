---
description: Sales Insight Actions Activity Glossary - Marketo Docs - Product Documentation
title: Aktivitetsordlista för Sales Insight Actions
hide: true
hidefromtoc: true
source-git-commit: a0cfc190e00ea6f8a9f5ef717566651423638b7d
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Aktivitetsordlista för Sales Insight Actions {#sales-insight-actions-activity-glossary}

I Sales Insight Actions, when a seller: lägger till ett lead till en försäljningskampanj, skickar ett e-postmeddelande till dem eller gör ett utgående försäljningssamtal, loggas det under Marketo aktivitetshistorik för det leadet. När leadet dessutom interagerar med e-post, öppnar, klickar och svarar loggas det också.

Aktiviteterna nedan loggas till Marketo från Sales Insight Actions.

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
   <td>Unikt ID för personpost i Säljinformationsåtgärder.</td> 
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
   <td>Unikt ID för tillgång till säljkampanj i åtgärder för försäljningsinsikter.</td> 
  </tr>
  <tr> 
   <td><strong>Namn på försäljningskampanj</strong></td> 
   <td>Namn på försäljningskampanj.</td> 
  </tr>
  <tr> 
   <td><strong>URL för försäljningskampanj</strong></td> 
   <td>Säljannonsering - Insight Actions URL for Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>E-postämne för försäljning</strong></td> 
   <td>Ärenderad e-postadress följd av ett unikt ID (t.ex.: Min ämnesrad (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>Telefonnummer till försäljning har anropats</strong></td> 
   <td>Telefonnummer som anropas av Försäljning.</td> 
  </tr>
  <tr> 
   <td><strong>Namn på försäljningsmall</strong></td> 
   <td>Namn på e-postmall i Sales Insight Actions.</td> 
  </tr>
  <tr> 
   <td><strong>URL för försäljningsmall</strong></td> 
   <td>Sales Insight Actions URL for email template.</td> 
  </tr>
  <tr> 
   <td><strong>Skickat av</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td> 
  </tr> 
  <tr> 
   <td><strong>Källa</strong></td> 
   <td>Aktivitetens källa. Anger som "Tout" för aktiviteter inom Sales Insight före oktoberversionen 21. Kommer att bli "Sales App" för Sales Insight Actions-aktiviteter efter okt 21-versionen.</td>
  </tr> 
  <tr> 
   <td><strong>Mall-ID</strong></td> 
   <td>När källan är Tout blir mall-ID Marketo mall-ID:t för försäljningsåtgärder. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td> 
  </tr> 
 </tbody> 
</table>
