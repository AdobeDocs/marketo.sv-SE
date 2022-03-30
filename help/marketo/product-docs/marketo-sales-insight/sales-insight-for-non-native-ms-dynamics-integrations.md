---
description: Sales Insight for Non-Native MS Dynamics Integrations - Marketo Docs - produktdokumentation
title: Sales Insight for Non-Native MS Dynamics Integrations
source-git-commit: fb663ddf4c0021f258317636fbc7794e8172ab7e
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# Sales Insight for Non-Native MS Dynamics Integrations {#sales-insight-for-non-native-ms-dynamics-integrations}

Om ditt Adobe Marketo Engage-konto är anslutet till MS Dynamics via en anpassad eller icke-inbyggd integrering använder du den här artikeln för att konfigurera Sales Insight.

>[!PREREQUISITES]
>
>* Funktionen&quot;MSI Non-Native&quot; aktiverad för din Marketo-instans innan du börjar konfigurera MSI (om den inte redan är aktiverad och du redan har köpt funktionen kontaktar du [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} - kontakta din Customer Success Manager om du inte har köpt den här funktionen än.)
>* En MS Dynamics-prenumeration med MSI-installation ([Lokalt](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-365.md){target=&quot;_blank&quot;}, [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target=&quot;_blank&quot;}).
>* Marketo REST API [har konfigurerats](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}. De exponerade CRUD-API:erna kommer att utgöra grunden för den icke-ursprungliga synkroniseringen.
>* Läs [det här blogginlägget](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;} för att förstå objektet och relationerna.


## Lyckad icke-inbyggd synkronisering för MSI kräver följande {#successful-non-native-sync-for-msi-requires-the-following}

1. Synkronisera MS Dynamics-försäljningsanvändaren till Marketo.

   Försäljningsanvändaren för MS Dynamics är en extern användare som äger lead/kontakt i MS Dynamics. En Marketo-säljare måste uppgraderas för MS Dynamics-säljanvändaren. Fältet externalSalesPersonId är obligatoriskt för att överföra säljaren.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Fält för Marketo-säljare</strong></td> 
      <td><strong>Användarfält för MS Dynamics</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-användare</td> 
      <td><p>Identifierar posten för Marketo-säljare till ett externt användarobjekt för MS Dynamics.</p><p>Försäljaren måste synkroniseras först innan de andra objekten synkroniseras så att rätt relationer skapas.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljare: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * API-dokumentation för synkronisering av säljaren: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST){target=&quot;_blank&quot;}

1. Synkronisera MS Dynamics-konton med Marketo.

   Ett Marketo-företag måste uppdateras för MS Dynamics-kontot. The _externalCompanyId_ och _externalSalesPersonId_ fält är obligatoriska för att bekräfta företaget.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-företagsfält</strong></td> 
      <td><strong>Kontofält för MS Dynamics</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-konto</td> 
      <td>Identifierar en Marketo-företagspost till ett externt MS Dynamics-kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-försäljning</td> 
      <td>Identifierar en Marketo-företagspost för ett externt MS Dynamics-försäljningsanvändarobjekt som är kontoägare.<br><br>Används också inom Marketo för att associera företaget med den säljare som äger företagsposten. Säljaren måste synkroniseras först innan du anger det här fältet.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för företag: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * API-dokumentation för synkronisering av företag: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target=&quot;_blank&quot;}

1. Synkronisera MS Dynamics Leads/Contacts till Marketo.

   Du måste infoga en Marketo-lead för MS Dynamics-lead/kontakt. The _externalPersonId_, _externalSalesPersonId_ och _externalCompanyId_ fält är obligatoriska för att lägga upp lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead Field</strong></td> 
      <td><strong>Lead-/kontaktfält för MS Dynamics</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Lead/kontakt-skiftlägeskänslig global unik identifierare för MS Dynamics</td> 
      <td>Identifierar Marketo Lead-posten till ett externt lead-/kontaktobjekt för MS Dynamics.<br><br>Det här är ett nytt fält som introduceras för MSI som inte är Native.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-försäljning</td> 
      <td>Identifierar det externa användarobjektet för MS Dynamics-försäljning som äger denna lead/kontakt.<br><br>Kopplar även lead till säljaren i Marketo. Säljaren måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-konto</td> 
      <td>Identifierar det externa MS Dynamics-kontoobjektet som lead/kontakt tillhör.<br><br>Även relaterar lead-posten till ett företag i Marketo. MS Dynamics-kontot måste först synkroniseras korrekt.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för leads: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target=&quot;_blank&quot;}
   * API-dokumentation för synkronisering av leads: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target=&quot;_blank&quot;}

1. Synkronisera MS Dynamics-affärsmöjligheter med Marketo.

   Du måste bekräfta en Marketo-möjlighet för MS Dynamics-säljprojektet. The _externalOpportunityId_, _externalCompanyId_ och _externalSalesPersonId_ fält är obligatoriska för att bekräfta säljprojektet.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity Object Field</strong></td> 
      <td><strong>Objektfält för MS Dynamics-affärsmöjlighet</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Lead/kontakt-skiftlägeskänslig global unik identifierare för MS Dynamics</td> 
      <td>Identifierar Marketo-säljprojektsposten till ett externt MS Dynamics-säljprojektsobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-konto</td> 
      <td>Identifierar det externa MS Dynamics-kontoobjektet som affärsmöjligheten tillhör. <br><br>MS Dynamics-kontot måste först synkroniseras korrekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-försäljning</td> 
      <td>Identifierar det externa användarobjektet för MS Dynamics-försäljning som äger affärsmöjligheten. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljprojekt: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST){target=&quot;_blank&quot;}

1. Synkronisera kontaktroller för MS Dynamics till Marketo.

   Kontaktroller för MS Dynamics för ett MS Dynamics-säljprojekt kan sedan synkroniseras via Marketo-säljprojektsrollen. Posten för säljprojektsrollen anger att _externalOpportunityId_, _roll_ och _leadId_ fält.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Rollfält för Marketo-säljprojekt</strong></td> 
      <td><strong>Fält för kontaktroll för MS Dynamics</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Versalokänslig global unik identifierare för MS Dynamics-affärsmöjlighet</td> 
      <td>Identifierar Marketo-säljprojektsrollen för ett externt MS Dynamics-säljprojektsobjekt.<br><br>MS Dynamics-säljprojektet måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Ej tillämpligt, det här skulle vara ett Marketo lead-ID</td> 
      <td>Detta är Marketo lead-ID för den synkroniserade MS Dynamics-kontakten.<br><br>När kontakten har synkroniserats i Marketo kan du använda den skiftlägeskänsliga globala unika identifieraren för MS Dynamics som externalPersonId och fråga för Marketo Lead med Marketo REST API.</td> 
     </tr> 
     <tr> 
      <td>roll</td> 
      <td>Rollfältet för MS Dynamics-kontakten</td> 
      <td>Beskriver rollen för kontakten för den här affärsmöjligheten.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljprojekt: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunity/syncOpportzationsUsingPOST){target=&quot;_blank&quot;}

1. Synkronisera senast intressanta stund-/MSI-bedömningsfält till MS Dynamics.

   När MS Dynamics-objekten har synkroniserats korrekt till Marketo kan du dra nytta av MSI-funktionerna. Fälten Senaste intressanta MSI-stund/poäng visas i REST API för leads. Dessa fält beräknas av MSI och är skrivskyddade.

   Fälten Senaste intressanta stund/poäng i en Marketo Lead måste synkroniseras regelbundet till MS Dynamics med REST API Lead-slutpunkten. Fråga den här slutpunkten efter en Marketo-lead med _externalPersonId_ som filterType och skickar MS Dynamics Lead GUID som filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Du kan sedan använda värdena för de här fälten för att synkronisera med ditt lead-/kontaktobjekt för MS Dynamics.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead Field</strong></td> 
      <td><strong>Lead-/kontaktfält för MS Dynamics</strong></td> 
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

   * Dokumentation för Lead REST API: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}.
   Korrekt användning av de externa fälten är avgörande för en lyckad icke-inbyggd synkronisering. Om du inte ser data i vissa vyer är det troligt att ett visst fält inte synkroniserades korrekt. Om t.ex. en leads aktiviteter och intressanta stunder inte visas när du tittar i MSI-widgeten under deras konto, är det troligt att antingen lead-företagets företag eller kontot inte synkroniserades korrekt. Om du utför en GET-begäran för denna lead samtidigt som du anger externa fält kan du kontrollera om leadet synkroniserades korrekt. Dessutom måste e-postadressen till den externa säljaren i Marketo matcha e-postadressen för den användaren i MS Dynamics. Data kanske inte visas på fliken Marketo i MS Dynamics om e-postmeddelandena inte matchar.
