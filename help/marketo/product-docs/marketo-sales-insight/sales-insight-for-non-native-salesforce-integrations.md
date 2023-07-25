---
unique-page-id: 45417125
description: Sales Insight for Non-Native Salesforce Integrations - Marketo Docs - Product Documentation
title: Sales Insight for Non-Native Salesforce Integrations
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Sales Insight for Non-Native Salesforce Integrations {#sales-insight-for-non-native-salesforce-integrations}

Om ditt Adobe Marketo Engage-konto är anslutet till Salesforce via en anpassad eller icke-inbyggd integrering använder du den här artikeln för att konfigurera Sales Insight.

>[!PREREQUISITES]
>
>* Funktionen &quot;MSI Non-Native&quot; (MSI utan inbyggt) aktiverad för din Marketo-instans innan du börjar konfigurera MSI. Om den inte är det och du redan har köpt funktionen kontaktar du [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Om du ännu inte har köpt den här funktionen kontaktar du kontoteamet på Adobe (din kontoansvarige).
>* Ett Salesforce-konto med [Installation av MSI-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* Marketo REST API [har konfigurerats](https://developers.marketo.com/rest-api/){target="_blank"}. De exponerade CRUD-API:erna kommer att utgöra grunden för den icke-ursprungliga synkroniseringen.
>* Läs [det här blogginlägget](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} för att förstå objektet och relationerna.
>* Ställ in Salesforce-objekt för att visa den globalt unika identifieraren som inte är skiftlägeskänslig för 18 tecken i stället för den globalt unika identifieraren för 15 tecken.

>[!NOTE]
>
>Det går inte att använda REST API-konfigurationen i administratörspanelen för Marketo MSI för icke-inbyggd synkronisering.

## Lyckad icke-inbyggd synkronisering för MSI kräver följande {#successful-non-native-sync-for-msi-requires-the-following}

1. Synkronisera Salesforce-säljanvändaren till Marketo.

   Salesforce-användaren är en extern användare som äger lead/kontakt i Salesforce. En Marketo-säljare måste uppgraderas för Salesforce-säljanvändaren. The *externalSalesPersonId* ska fyllas i av säljaren.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Fält för Marketo-säljare</strong></td> 
      <td><strong>Användarfält för Salesforce-försäljning</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce Sales User case-insensitive global unique identifier</td> 
      <td><p>Identifierar posten för Marketo-säljare till ett externt Salesforce-försäljningsanvändarobjekt.</p><p>Försäljaren måste synkroniseras först innan de andra objekten synkroniseras så att rätt relationer skapas.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljare: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * API-dokumentation för synkronisering av säljaren: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST){target="_blank"}

1. Synkronisera Salesforce-konton med Marketo.

   Ett Marketo-företag måste uppdateras för Salesforce-kontot. The _externalCompanyId_ och _externalSalesPersonId_ fält är obligatoriska för att bekräfta företaget.

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
      <td>Identifierar en företagspost för Marketo till ett externt Salesforce-användarobjekt som är kontoägare.<br><br>Används också inom Marketo för att associera företaget med den säljare som äger företagsposten. Säljaren måste synkroniseras först innan du anger det här fältet.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för företag: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * API-dokumentation för synkronisering av företag: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. Synkronisera Salesforce-leads/kontakter till Marketo.

   Du måste ange en Marketo-lead för Salesforce-lead/kontakt. The _externalPersonId_, _externalSalesPersonId_ och _externalCompanyId_ fält är obligatoriska för att lägga upp lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead Field</strong></td> 
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
      <td>Identifierar det externa Salesforce-objektet Försäljningsanvändare som äger denna lead/kontakt.<br><br>Kopplar även lead till säljaren i Marketo. Säljaren måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce-kontots skiftlägeskänsliga globalt unika identifierare</td> 
      <td>Identifierar det externa Salesforce-kontoobjektet som lead/kontakt tillhör.<br><br>Även relaterar lead-posten till ett företag i Marketo. Salesforce-kontot måste först synkroniseras korrekt.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för leads: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * API-dokumentation för synkronisering av leads: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Synkronisera Salesforce-affärsmöjligheter med Marketo.

   Du måste bekräfta en Marketo-möjlighet för Salesforce-säljprojektet. The _externalOpportunityId_, _externalCompanyId_ och _externalSalesPersonId_ fält är obligatoriska för att bekräfta säljprojektet.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity Object Field</strong></td> 
      <td><strong>Salesforce-objektfält för affärsmöjlighet</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce Lead/Contact case-insensitive global unique identifier</td> 
      <td>Identifierar posten för Marketo-säljprojekt till ett externt Salesforce-objekt för säljprojekt.</td> 
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

   * API-dokumentation för säljprojekt: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST){target="_blank"}

1. Synkronisera Salesforce-kontaktroller till Marketo.

   Salesforce-kontaktroller för en Salesforce-affärsmöjlighet kan sedan synkroniseras via Marketo-säljprojektsrollen. Posten för säljprojektsrollen anger att _externalOpportunityId_, _roll_ och _leadId_ fält.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Rollfält för Marketo-säljprojekt</strong></td> 
      <td><strong>Salesforce-kontaktrollfält</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce-ärendeokänslig global unik identifierare</td> 
      <td>Identifierar Marketo-säljprojektsrollen för ett externt Salesforce-säljprojektsobjekt.<br><br>Salesforce-säljprojektet måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Ej tillämpligt, det här skulle vara ett Marketo lead-ID</td> 
      <td>Detta är Marketo lead-ID för den synkroniserade Salesforce-kontakten.<br><br>När kontakten har synkroniserats i Marketo kan du använda den globalt unika identifieraren, som inte är skiftlägeskänslig för Salesforce, som externalPersonId och fråga för Marketo Lead med hjälp av Marketo REST API.</td> 
     </tr> 
     <tr> 
      <td>roll</td> 
      <td>Rollfältet för Salesforce-kontakten</td> 
      <td>Beskriver rollen för kontakten för den här affärsmöjligheten.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljprojekt: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST){target="_blank"}

1. Synkronisera senast intressanta stund-/MSI-bedömningsfält till SFDC.

   När dina Salesforce-objekt har synkroniserats korrekt till Marketo kan du dra nytta av MSI-funktionerna. Fälten Senaste intressanta MSI-stund/poäng visas i REST API för leads. Dessa fält beräknas av MSI och är skrivskyddade.

   Fälten Senaste intressanta stund/poäng i en Marketo Lead måste synkroniseras regelbundet till Salesforce med REST API Lead-slutpunkten. Fråga den här slutpunkten efter en Marketo-lead med _externalPersonId_ som filterType och som skickas i Salesforce Lead GUID som filterValue.

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
      <td><strong>Marketo Lead Field</strong></td> 
      <td><strong>Lead-/kontaktfält för Salesforce</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastIntressantMomentType</td> 
      <td>Etikett: Typ av senaste intressanta stund<br>Namn: Sista_intressanta_stund_typ__c</td> 
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

   Dokumentation för Lead REST API: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   Korrekt användning av de externa fälten är avgörande för en lyckad icke-inbyggd synkronisering. Om du inte ser data i vissa vyer är det troligt att ett visst fält inte synkroniserades korrekt. Om t.ex. en leads aktiviteter och intressanta stunder inte visas vid sökning i MSI-widgeten under deras konto, är det troligt att antingen lead-företagets företag eller kontot inte synkroniserades korrekt. Om du utför en GET-begäran för denna lead samtidigt som du anger externa fält kan du kontrollera om leadet synkroniserades korrekt. E-postmeddelandet för den externa säljaren i Marketo måste dessutom matcha e-postmeddelandet för den användaren i Salesforce. Data kanske inte visas på fliken Marketo i Salesforce om e-postmeddelandena inte matchar.
