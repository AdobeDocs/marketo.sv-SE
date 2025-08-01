---
description: Sales Insight Actions Activity Glossary - Marketo Docs - Product Documentation
title: Aktivitetsordlista för Sales Insight Actions
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 3%

---

# [!DNL Sales Insight Actions] aktivitetsordlista {#sales-insight-actions-activity-glossary}

Om en säljare i [!DNL Sales Insight Actions] lägger till ett lead till en försäljningskampanj, skickar ett e-postmeddelande till dem eller gör ett utgående försäljningssamtal, loggas det under Marketo aktivitetshistorik för det leadet. När leadet dessutom interagerar med e-post, öppnar, klickar och svarar loggas det också.

Aktiviteterna nedan loggas till Marketo från [!DNL Sales Insight Actions].

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
  <th rowspan="9">[!UICONTROL Send Sales Email]</th>
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
  <th rowspan="9">[!UICONTROL Open Sales Email]</th>
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
  <th rowspan="10">[!UICONTROL Clicked Sales Email]</th>
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
  <th rowspan="3">[!UICONTROL Replied to Sales Email]</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>Källa</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">[!UICONTROL Received Sales Call]</th>
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
  <th rowspan="6">[!UICONTROL Add to Sales Campaign]</th>
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
  <th rowspan="6">[!UICONTROL Remove from Sales Campaign]</th>
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
   <td>Unikt ID för personpost i [!DNL Sales Insight Actions].</td>
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
   <td>Unikt ID för försäljningskampanjresurs i [!DNL Sales Insight Actions].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td>
   <td>Namn på säljkampanj.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td>
   <td>[!DNL Sales Insight Actions] URL för försäljningskampanj.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td>
   <td>Ärenderad e-postadress följd av ett unikt ID (t.ex. Min ärenderad (SIA-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td>
   <td>Telefonnummer som anropas av Försäljning.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template Name]</strong></td>
   <td>Namn på e-postmall i [!DNL Sales Insight Actions].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template URL]</strong></td>
   <td>[!DNL Sales Insight Actions] URL för e-postmall.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>E-postadress till den person som skickade e-postmeddelandet.</td>
  </tr>
  <tr>
   <td><strong>Källa</strong></td>
   <td>Source om aktiviteten. Anges som "Tout" för [!DNL Sales Insight Actions] aktiviteter före oktot 21-versionen. Kommer att vara "Sales App" för [!DNL Sales Insight Actions]-aktiviteter efter okt '21'-versionen.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Template ID]</strong></td>
   <td>När källan är Tout blir mall-ID:t [!DNL Marketo Sales Insight Actions] mall-ID. Använd det här alternativet om du vill ha en specifik mall i stället för en ämnesrad, som kan finnas i flera mallar.
</td>
  </tr>
 </tbody>
</table>
