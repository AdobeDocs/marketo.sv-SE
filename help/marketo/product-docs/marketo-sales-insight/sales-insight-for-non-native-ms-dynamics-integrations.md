---
description: '[!DNL Sales Insight] för icke-ursprungliga MS [!DNL Dynamics] integrations - Marketo Docs - produktdokumentation'
title: '[!DNL Sales Insight] för icke-ursprungliga MS [!DNL Dynamics] integreringar'
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 0%

---

# [!DNL Sales Insight] för icke-ursprungliga MS [!DNL Dynamics]-integreringar {#sales-insight-for-non-native-ms-dynamics-integrations}

Om ditt Adobe Marketo Engage-konto är anslutet till MS [!DNL Dynamics] via en anpassad eller icke-inbyggd integrering använder du den här artikeln för att konfigurera [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* Funktionen &quot;MSI Non-Native&quot; (MSI utan inbyggt) aktiverad för din Marketo-instans innan du börjar konfigurera MSI. Om den inte är det och du redan har köpt funktionen kontaktar du [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Om du ännu inte har köpt den här funktionen kontaktar du Adobe Account Team (din kontoansvarige).
>* Hämta [MSI-paket för anpassad synkronisering](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* En MS Dynamics-prenumeration med MSI-installationsprogrammet (vi stöder endast [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} just nu).
>* Marketo REST API [har konfigurerats](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. De exponerade CRUD-API:erna kommer att utgöra grunden för den icke-ursprungliga synkroniseringen.
>* Läs [det här blogginlägget](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} för att få en förståelse för objektet och relationerna.

## Lyckad icke-inbyggd synkronisering för MSI kräver följande {#successful-non-native-sync-for-msi-requires-the-following}

1. Synkronisera MS [!DNL Dynamics]-säljanvändaren till Marketo.

   Försäljningsanvändaren [!DNL Dynamics] i MS är en extern användare som äger leads/kontakter i MS [!DNL Dynamics]. En Marketo-säljare måste uppgraderas för MS [!DNL Dynamics]-säljanvändaren. Fältet externalSalesPersonId är obligatoriskt för att överföra säljaren.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Fält för Marketo-säljare</strong></td> 
        <td><strong>Användarfält för MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span>, användarskiftlägeskänslig, globalt unik identifierare</td> 
      <td><p>Identifierar posten för Marketo-säljare till ett externt användarobjekt för MS <span class="dnl">Dynamics</span>.</p><p>Försäljaren måste synkroniseras först innan de andra objekten synkroniseras så att rätt relationer skapas.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [API-dokumentation för säljare](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [API-dokumentation för synkronisering av säljaren](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synkronisera MS [!DNL Dynamics]-konton till Marketo.

   Ett Marketo-företag måste uppgraderas för MS [!DNL Dynamics]-kontot. Fälten _externalCompanyId_ och _externalSalesPersonId_ är obligatoriska för företagets upsert.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo-företagsfält</strong></td> 
        <td><strong>Kontofält för MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span>, skiftlägeskänslig global unik identifierare</td> 
        <td>Identifierar en Marketo-företagspost till ett externt MS <span class="dnl">Dynamics</span>-kontoobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Säljanvändares skiftlägeskänsliga globalt unika identifierare</td> 
        <td>Identifierar en Marketo-företagspost för ett externt MS <span class="dnl">Dynamics</span>-försäljningsanvändarobjekt som är kontoägare.<br><br>Används också inom Marketo för att associera företaget med den säljare som äger företagsposten. Säljaren måste synkroniseras först innan du anger det här fältet.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för företag: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * API-dokumentation för synkronisering av företag: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Synkronisera MS [!DNL Dynamics] leads/kontakter till Marketo.

   Du måste ange en Marketo-lead för lead/kontakt för medlemsstaterna [!DNL Dynamics]. Fälten _externalPersonId_, _externalSalesPersonId_ och _externalCompanyId_ krävs för att ladda upp lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead Field</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> lead-/kontaktfält</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Lead/Contact skiftlägeskänslig global unik identifierare</td> 
        <td>Identifierar Marketo Lead-posten till ett externt MS <span class="dnl">Dynamics</span> Lead/Contact-objekt.<br><br>Det här är ett nytt fält som introduceras för MSI som inte är Native.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Säljanvändares skiftlägeskänsliga globalt unika identifierare</td> 
        <td>Identifierar det externa MS <span class="dnl">Dynamics</span>-försäljningsanvändarobjektet som äger denna lead/kontakt.<br><br>Relaterar även leadet med säljaren i Marketo. Säljaren måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span>, skiftlägeskänslig global unik identifierare</td> 
        <td>Identifierar det externa MS <span class="dnl">Dynamics</span>-kontoobjektet som lead/kontakt tillhör.<br><br>Relaterar även lead-posten till ett företag i Marketo. MS <span class="dnl">Dynamics</span>-kontot måste synkroniseras korrekt först.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för leads: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * API-dokumentation för synkronisering av leads: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. Synkronisera MS [!DNL Dynamics]-affärsmöjligheter till Marketo.

   Du måste bekräfta en Marketo-möjlighet för MS [!DNL Dynamics]-säljprojektet. Fälten _externalOpportunityId_, _externalCompanyId_ och _externalSalesPersonId_ krävs för att bekräfta affärsmöjligheten.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity Object Field</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span>-objektfält för affärsmöjlighet</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>MS <span class="dnl">Dynamics</span> Lead/Contact skiftlägeskänslig global unik identifierare</td> 
      <td>Identifierar Marketo-säljprojektsposten till ett externt MS <span class="dnl">Dynamics</span> -säljprojektsobjekt.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
        <td>MS <span class="dnl">Dynamics</span>, skiftlägeskänslig global unik identifierare</td> 
        <td>Identifierar det externa MS <span class="dnl">Dynamics</span>-kontoobjektet som affärsmöjligheten tillhör. <br><br>MS <span class="dnl">Dynamics</span>-kontot måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
        <td>MS <span class="dnl">Dynamics</span> Säljanvändares skiftlägeskänsliga globalt unika identifierare</td> 
        <td>Identifierar det externa MS <span class="dnl">Dynamics</span>-försäljningsanvändarobjektet som äger affärsmöjligheten. </td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljprojekt: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synkronisera MS [!DNL Dynamics]-kontaktroller till Marketo.

   Kontaktroller för MS [!DNL Dynamics] för ett MS [!DNL Dynamics]-säljprojekt kan sedan synkroniseras via Marketo-säljprojektsrollen. Posten för säljprojektsrollen anger fälten _externalOpportunityId_, _role_ och _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Rollfält för Marketo-säljprojekt</strong></td> 
        <td><strong>Fält för kontaktroll för MS <span class="dnl">Dynamics</span></strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
        <td>MS <span class="dnl">Dynamics</span> - skiftlägeskänslig global unik identifierare för affärsmöjlighet</td> 
      <td>Identifierar Marketo-säljprojektsrollen för ett externt MS <span class="dnl">Dynamics</span> -säljprojektsobjekt.<br><br>MS <span class="dnl">Dynamics</span>-affärsmöjligheten måste synkroniseras korrekt först.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>Ej tillämpligt. Detta är ett Marketo lead-ID</td> 
        <td>Detta är Marketo lead-ID för den synkroniserade MS <span class="dnl">Dynamics</span>-kontakten.<br><br>När kontakten har synkroniserats i Marketo kan du använda MS <span class="dnl">Dynamics</span> som är skiftlägeskänslig globalt unik identifierare som externalPersonId och fråga efter Marketo Lead med Marketo REST API.</td> 
     </tr> 
     <tr> 
      <td>roll</td> 
        <td>Rollfältet för MS <span class="dnl">Dynamics</span>-kontakten</td> 
      <td>Beskriver rollen för kontakten för den här affärsmöjligheten.</td> 
     </tr> 
    </tbody> 
   </table>

   * API-dokumentation för säljprojekt: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * API-dokumentation för synkroniseringsmöjligheter: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Synkronisera senast intressanta stund-/MSI-bedömningsfält till MS [!DNL Dynamics].

   När dina MS [!DNL Dynamics]-objekt har synkroniserats korrekt till Marketo kan du dra nytta av MSI-funktionerna. Fälten Senaste intressanta MSI-stund/poäng visas i REST API för leads. Dessa fält beräknas av MSI och är skrivskyddade.

   Fälten Senaste intressanta stund/poäng i en Marketo Lead måste synkroniseras regelbundet till MS [!DNL Dynamics] med REST API Lead-slutpunkten. Fråga den här slutpunkten efter en Marketo Lead med hjälp av _externalPersonId_ som filterType och skicka lead-GUID:t för MS [!DNL Dynamics] som filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Du kan sedan använda värdena för de här fälten för att synkronisera till ditt lead-/kontaktobjekt för MS [!DNL Dynamics].

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Lead Field</strong></td> 
        <td><strong>MS <span class="dnl">Dynamics</span> lead-/kontaktfält</strong></td> 
      <td><strong>Beskrivning</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastIntressantMomentType</td> 
      <td>Etikett: Senaste intressanta stund typ<br>Namn: Last_Intressant_stund_typ__c</td> 
      <td>Typ av det sista intressanta tillfället för leadet</td> 
     </tr> 
     <tr> 
      <td>msiLastIntressantMomentDate</td> 
      <td><p>Etikett: Senaste intressanta datum</p><p>Namn: Last_Intressant_Moment_Date__c</p></td> 
      <td>Datum för leadets sista intressanta stund</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Etikett: Beskrivning av Senaste intressanta stund</p><p>Namn: Last_Intressant_stund_Desc__c</p></td> 
      <td>Beskrivning av leadets sista intressanta stund</td> 
     </tr> 
     <tr> 
      <td>msiLastIntressantMomentSource</td> 
      <td><p>Etikett: Senaste intressanta stund Source</p><p>Namn: Last_Intressant_stund_Source__c</p></td> 
      <td>Source för ledningens sista intressanta ögonblick</td> 
     </tr> 
     <tr> 
      <td>prioritet</td> 
      <td><p>Etikett: Engagement</p><p>Namn: Prioritet__c</p></td> 
      <td>Leadens prioritet</td> 
     </tr> 
     <tr> 
      <td>relativeUrgent</td> 
      <td><p>Etikett: Relativt akutvärde</p><p>Namn: Emergency_Value__c</p></td> 
      <td>Leadens relativa brådskande situation</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Etikett: Relativt poängvärde</p><p>Namn: Relative_Score_Value__c</p></td> 
      <td>Relativ poängsättning av lead</td> 
     </tr> 
    </tbody> 
   </table>

   * Dokumentation för Lead REST API: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   Korrekt användning av de externa fälten är avgörande för en lyckad icke-inbyggd synkronisering. Om du inte ser data i vissa vyer är det troligt att ett visst fält inte synkroniserades korrekt. Om t.ex. en leads aktiviteter och intressanta stunder inte visas vid sökning i MSI-widgeten under deras konto, är det troligt att antingen lead-företagets företag eller kontot inte synkroniserades korrekt. Genom att utföra en GET-begäran för denna lead och ange externa fält kan du kontrollera om leadet synkroniserades korrekt. Dessutom måste e-postadressen till den externa säljaren i Marketo matcha e-postadressen för den användaren i MS Dynamics. Data kanske inte visas på fliken Marketo i MS Dynamics om e-postmeddelandena inte matchar.
