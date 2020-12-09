---
unique-page-id: 45417125
description: Sales Insight for Non-Native Salesforce Integrations - Marketo Docs - Produktdokumentation
title: Sales Insight for Non-Native Salesforce Integrations
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Sales Insight for Non-Native Salesforce Integrations {#sales-insight-for-non-native-salesforce-integrations}

Om ditt Marketo-konto är anslutet till Salesforce via en anpassad eller icke-inbyggd integrering använder du det här dokumentet för att konfigurera Sales Insight.

>[!PREREQUISITES]
>
>* Kontakta er Customer Success Manager för att aktivera funktionen&quot;MSI Non-Native&quot; för er Marketo-instans.
>* Ett Salesforce-konto med konfiguration av MSI-paket.
>* Marketo REST API [har konfigurerats](http://developers.marketo.com/rest-api/). De exponerade CRUD-API:erna kommer att utgöra grunden för den icke-ursprungliga synkroniseringen.
>* Läs [det här blogginlägget](http://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) för att få en förståelse för objektet och relationerna.
>* Ställ in Salesforce-objekt för att visa den globalt unika identifieraren som inte är skiftlägeskänslig för 18 tecken i stället för den globalt unika identifieraren för 15 tecken.

>



>[!NOTE]
>
>Det går inte att använda REST API-konfigurationen i Marketo MSI Admin Panel för icke-inbyggd synkronisering.

## Lyckad icke-inbyggd synkronisering för MSI kräver följande {#successful-non-native-sync-for-msi-requires-the-following}

1. Synkronisera Salesforce-säljanvändaren till Marketo.

   Salesforce-användaren är en extern användare som äger lead/kontakt i Salesforce. En Marketo-säljare måste uppgraderas för Salesforce-säljanvändaren. Fältet *externalSalesPersonId* är obligatoriskt för att överföra säljaren.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Sales Person Field</strong></td> 
   <td><strong>Användarfält för Salesforce-försäljning</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User case-insensitive global unique identifier</td> 
   <td><p>Identifierar Marketo-säljpersonsposten till ett externt Salesforce-försäljningsanvändarobjekt.</p><p>Försäljaren måste synkroniseras först innan de andra objekten synkroniseras så att rätt relationer skapas.</p></td> 
  </tr> 
 </tbody> 
</table>

API-dokumentation för säljare: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](http://developers.marketo.com/rest-api/lead-database/sales-persons/)\
API-dokumentation för synkronisering av säljaren: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST)

1. Synkronisera Salesforce-konton med Marketo.

   Ett Marketo-företag måste uppdateras för Salesforce-kontot. Fälten *externalCompanyId* och *externalSalesPersonId* är obligatoriska för företagets upsert.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo-företagsfält</strong></td> 
   <td><strong>Salesforce-kontofält</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce-kontots skiftlägeskänsliga globalt unika identifierare</td> 
   <td>Identifierar en Marketo-företagspost till ett externt Salesforce-kontoobjekt.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User case-insensitive global unique identifier</td> 
   <td>Identifierar en Marketo-företagspost till ett externt Salesforce-användarobjekt som är kontoägare.<br><br>Används även inom Marketo för att associera företaget med den säljare som äger företagsposten. Säljaren måste synkroniseras först innan du anger det här fältet.</td> 
  </tr> 
 </tbody> 
</table>

API-dokumentation för företag: [https://developers.marketo.com/rest-api/lead-database/companies/](http://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Synkronisera Salesforce-leads/kontakter till Marketo.

   Du måste infoga en Marketo Lead för Salesforce Lead/Contact. Fälten *externalPersonId*, *externalSalesPersonId* och *externalCompanyId* krävs för att ladda upp leadet.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Lead-fält</strong></td> 
   <td><strong>Lead-/kontaktfält för Salesforce</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforce Lead/Contact case-insensitive global unique identifier</td> 
   <td>Identifierar Marketo Lead-posten till ett externt Salesforce Lead/Contact-objekt.<br><br>Det här är ett nytt fält som introduceras för MSI som inte är Native.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User case-insensitive global unique identifier</td> 
   <td>Identifierar det externa Salesforce-objektet Försäljningsanvändare som äger denna lead/kontakt.<br><br>Relaterar även leadet till säljaren i Marketo. Säljaren måste synkroniseras korrekt först.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce-kontots skiftlägeskänsliga globalt unika identifierare</td> 
   <td>Identifierar det externa Salesforce-kontoobjektet som lead/kontakt tillhör.<br><br>Relaterar även lead-posten till ett företag i Marketo. Salesforce-kontot måste först synkroniseras korrekt.</td> 
  </tr> 
 </tbody> 
</table>

API-dokumentation för leads: [`https://developers.marketo.com/rest-api/lead-database/leads/`](http://developers.marketo.com/rest-api/lead-database/leads/)\
API-dokumentation för synkronisering av leads:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Synkronisera Salesforce-affärsmöjligheter med Marketo.

   Du måste infoga en marknadsföringsmöjlighet för Salesforce-affärsmöjligheten. Fälten *externalOpportunityId*, *externalCompanyId* och *externalSalesPersonId* krävs för att bekräfta säljprojektet.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo-säljprojektsobjektfält</strong></td> 
   <td><strong>Salesforce-objektfält för affärsmöjlighet</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce Lead/Contact case-insensitive global unique identifier</td> 
   <td>Identifierar Marketo-säljprojektsposten till ett externt Salesforce-säljprojektsobjekt.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce-kontots skiftlägeskänsliga globalt unika identifierare</td> 
   <td>Identifierar det externa Salesforce-kontoobjektet som affärsmöjligheten tillhör. <br><br>Salesforce-kontot måste först synkroniseras korrekt.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales User case-insensitive global unique identifier</td> 
   <td>Identifierar det externa Salesforce-försäljningsanvändarobjektet som äger affärsmöjligheten. </td> 
  </tr> 
 </tbody> 
</table>

API-dokumentation för säljprojekt: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synkronisera Salesforce-kontaktroller till Marketo.

   Salesforce-kontaktroller för en Salesforce-affärsmöjlighet kan sedan synkroniseras via Marketo-säljprojektsrollen. Posten för säljprojektsrollen anger *fälten externalOpportunityId*, *role* och *leadId* .

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo-säljprojektsrollfält</strong></td> 
   <td><strong>Salesforce-kontaktrollfält</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce-ärendeokänslig global unik identifierare</td> 
   <td>Identifierar Marketo-säljprojektsrollen till ett externt Salesforce-säljprojektsobjekt.<br><br>Salesforce-säljprojektet måste synkroniseras korrekt först.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>Ej tillämpligt, detta skulle vara ett Marketo Lead ID</td> 
   <td>Detta är Marketo Lead ID för den synkroniserade Salesforce-kontakten.<br><br>När kontakten har synkroniserats i Marketo kan du använda den globalt unika identifieraren, som inte är skiftlägeskänslig för Salesforce, som externalPersonId och frågan för Marketo Lead med hjälp av Marketo REST API.</td> 
  </tr> 
  <tr> 
   <td>roll</td> 
   <td>Rollfältet för Salesforce-kontakten</td> 
   <td>Beskriver rollen för kontakten för den här affärsmöjligheten.</td> 
  </tr> 
 </tbody> 
</table>

API-dokumentation för säljprojekt: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Synkronisera senast intressanta stund-/MSI-bedömningsfält till SFDC.

   När Salesforce-objekten har synkroniserats korrekt till Marketo kan du sedan utnyttja MSI-funktionerna. Fälten Senaste intressanta MSI-stund/poäng visas i REST API för leads. Dessa fält beräknas av MSI och är skrivskyddade.

   Fälten Senaste intressanta stund/poäng i en Marketo Lead måste synkroniseras regelbundet till Salesforce med REST API Lead-slutpunkten. Fråga den här slutpunkten efter en Marketo Lead med *externalPersonId* som filterType och skicka Salesforce Lead GUID som filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Du kan sedan använda värdena för dessa fält för att synkronisera med Salesforce-objektet Lead/Contact.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Lead-fält</strong></td> 
   <td><strong>Lead-/kontaktfält för Salesforce</strong></td> 
   <td><strong>Beskrivning</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastIntressantMomentType</td> 
   <td>Etikett: Senaste intressanta<br>stund TypeName: Sista_intressanta_stund_typ__c</td> 
   <td>Typ av det sista intressanta tillfället för leadet</td> 
  </tr> 
  <tr> 
   <td>msiLastIntressantMomentDate</td> 
   <td><p>Etikett: Senaste intressanta datum</p><p>Namn: Last_Intrescing_Moment_Date__c</p></td> 
   <td>Datum för leadets sista intressanta stund</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>Etikett: Senaste intressanta stund - beskrivning</p><p>Namn: Sista_intressanta_stund_Desc_c</p></td> 
   <td>Beskrivning av leadets sista intressanta stund</td> 
  </tr> 
  <tr> 
   <td>msiLastIntressantMomentSource</td> 
   <td><p>Etikett: Källa för senaste intressanta stund</p><p>Namn: Last_Intrescing_Moment_Source__c</p></td> 
   <td>Källa till leadets sista intressanta tillfälle</td> 
  </tr> 
  <tr> 
   <td>prioritet</td> 
   <td><p>Etikett: Engagemang</p><p>Namn: Prioritet__c</p></td> 
   <td>Leadens prioritet</td> 
  </tr> 
  <tr> 
   <td>relativeUrgent</td> 
   <td><p>Etikett: Relativt brådskande värde</p><p>Namn: Emergency_Value__c</p></td> 
   <td>Leadens relativa brådskande situation</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Etikett: Relativt poängvärde</p><p>Namn: Relative_Score_Value__c</p></td> 
   <td>Relativ poängsättning av lead</td> 
  </tr> 
 </tbody> 
</table>

Dokumentation för Lead REST API:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

Korrekt användning av de externa fälten är avgörande för en lyckad icke-inbyggd synkronisering. Om du inte ser data i vissa vyer är det troligt att ett visst fält inte synkroniserades korrekt. Om t.ex. en leads aktiviteter och intressanta stunder inte visas när du tittar i MSI-widgeten under deras konto, är det troligt att antingen lead-företagets företag eller kontot inte synkroniserades korrekt. Om du utför en GET-begäran för denna lead samtidigt som du anger externa fält kan du kontrollera om leadet synkroniserades korrekt. E-postmeddelandet för den externa säljaren i Marketo måste dessutom matcha e-postmeddelandet för den användaren i Salesforce. Data kanske inte visas på Marketo-fliken i Salesforce om e-postmeddelandena inte matchar.

