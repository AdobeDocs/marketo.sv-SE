---
description: Läs mer om försäljningsaktivitetsvillkor för Sales Connect. Använd den här ordlistan för aktivitetstyper som synkroniseras med Marketo och Salesforce.
title: Säljaktivitetsordlista
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 3%

---

# Säljaktivitetsordlista {#sales-activity-glossary}

När en säljare i Sales Connect lägger till ett lead till en säljkonferens, skickar ett e-postmeddelande till dem eller ringer en aktivitet loggas det under Marketo aktivitetshistorik. När leadet dessutom interagerar med e-post loggas även öppningar, klickningar och svar.

Aktiviteterna nedan loggas till Marketo från [!DNL Sales Connect].

>[!NOTE]
>
>Dessa aktiviteter och attribut är tillgängliga för användning från våra REST- och Bulk-API:er.

## Aktiviteter {#activities}

<table>
 <tr>
  <th>Försäljningsaktivitet</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="9">Skicka e-postmeddelande</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] Namn</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="9"> Open Sales Email</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="10">Klicka på E-postadress</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
<tr>
  <th rowspan="3">Svar på e-postadress</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">Mottaget försäljningssamtal</th>
  <td>[!UICONTROL Sales Call Made By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Phone Number Called]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Duration]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Recording URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Sales Call Answered By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Lägg till i försäljningskampanj</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Ta bort från försäljningskampanj</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
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
   <td><strong>[!UICONTROL Details]</strong></td>
   <td>Information om studsfelmeddelande.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Email]</strong></td>
   <td>E-postadress som studsade.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Link]</strong></td>
   <td>URL som användaren klickade på.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Marketo Sales Person ID]</strong></td>
   <td>Unikt ID för personpost i [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Received By]</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Answered By]</strong></td>
   <td>Namn på den person som besvarade samtalet.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Duration]</strong></td>
   <td>Anropets längd i sekunder.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Made By]</strong></td>
   <td>E-postadress till den säljare som ringde samtalet.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Recording URL]</strong></td>
   <td>URL för samtalsinspelning.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Status]</strong></td>
   <td>Sparar samtalets slutliga samtalsstatus, som omfattar: slutförd, inget svar, avbruten, misslyckades.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Subject]</strong></td>
   <td>Samtalsresultat som valts av en säljare i återförsäljaren.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign ID]</strong></td>
   <td>Unikt ID för försäljningskampanjresurs i [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td>
   <td>Namn på säljkampanj.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td>
   <td>[!DNL Sales Connect] URL för försäljningskampanj.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td>
   <td>Ärenderad e-postadress följd av ett unikt ID (t.ex. Min ärenderad (MSC-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td>
   <td>Telefonnummer som anropas av Försäljning.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template Name]</strong></td>
   <td>Namn på e-postmall i [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template URL]</strong></td>
   <td>[!DNL Sales Connect] URL för e-postmall.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td>Source om aktiviteten. Anges som "Tout" för [!DNL Sales Connect] aktiviteter före oktot 21-versionen. Kommer att vara "Sales App" för [!DNL Sales Connect]-aktiviteter efter okt '21'-versionen.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Template ID]</strong></td>
   <td>När källan är Tout blir mall-ID:t [!DNL Marketo Sales Connect] mall-ID. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td>
  </tr>
 </tbody>
</table>
