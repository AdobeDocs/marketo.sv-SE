---
description: Standardfältmappning för Dynamics - Marketo Docs - produktdokumentation
title: Fältmappning för standardDynamics
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# Fältmappning för standardDynamics {#default-dynamics-field-mapping}

När du först synkroniserar ditt Marketo Engage-konto med Microsoft skapar Marketo automatiskt dessa associationer mellan de inbyggda fälten i Dynamics och Marketo.  Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

## Leadfält {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo Field</th>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>hälsningsfras</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>förnamn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>efternamn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>e-postadress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job title]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Street 1]</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL City]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL State/Province]</td>
      <td>address1_stateorregion</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Country/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Source]</td>
      <td>[!UICONTROL Lead Source]</td>
      <td>leadsourccode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>statuskod</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemi</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Rating]</td>
      <td>[!UICONTROL Rating]</td>
      <td>leadqualityCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Do Not Allow Faxes]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>telefon2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method of Contact]</td>
      <td>preferredcontactMethodCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Topic]</td>
      <td>[!UICONTROL Topic]</td>
      <td>ämne</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterest_potens</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterest_potdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterest_potens</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastIntresseDriftstyp</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Company Name]</td>
      <td>företagsnamn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgent</td>
    </tr>
    <tr>
      <td>[!UICONTROL Subject]</td>
      <td>[!UICONTROL Topic]</td>
      <td>ämne</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>intäkt</td>
    </tr>
  </tbody>
</table>

Leadfälten nedan synkroniseras för internt bruk.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>skapad</td>
    </tr>
  </tbody>
</table>

## Kontaktfält {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo Field</th>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>[!UICONTROL Created On]</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>[!UICONTROL Salutation]</td>
      <td>[!UICONTROL Salutation]</td>
      <td>hälsningsfras</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL First Name]</td>
      <td>förnamn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL Middle Name]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last]</td>
      <td>[!UICONTROL Last Name]</td>
      <td>efternamn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>e-postadress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Job Title]</td>
      <td>[!UICONTROL Job Title]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobile Phone]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>[!UICONTROL City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL State]</td>
      <td>[!UICONTROL Address 1: State/Province]</td>
      <td>address1_stateorregion</td>
    </tr>
    <tr>
      <td>[!UICONTROL Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>statuskod</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do Not Call]</td>
      <td>[!UICONTROL Do Not Allow Phone Calls]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Unsubscribed]</td>
      <td>[!UICONTROL Do not bulk email]</td>
      <td>donotbulkemi</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Email]</td>
      <td>[!UICONTROL Do Not Allow Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Home Phone]</td>
      <td>telefon2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Preferred Method Of Contact]</td>
      <td>[!UICONTROL Preferred Method Of Contact]</td>
      <td>preferredcontactMethodCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>[!UICONTROL Last interesting moment date]</td>
      <td>mkt_lastinterest_potens</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>[!UICONTROL Last interesting moment type]</td>
      <td>mkt_lastIntresseDriftstyp</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>[!UICONTROL Last Interesting moment source]</td>
      <td>mkt_leadinterest_potens</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>[!UICONTROL Last Interesting moment desc]</td>
      <td>mkt_lastinterest_potdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Send Marketing Material]</td>
      <td>[!UICONTROL Marketing Material]</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Priority]</td>
      <td>[!UICONTROL Priority]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Urgency]</td>
      <td>[!UICONTROL Urgency]</td>
      <td>mkt_urgent</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Score]</td>
      <td>[!UICONTROL Relative Score]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>description </td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Score]</td>
      <td>[!UICONTROL Lead Score]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>description </td>
    </tr>
  </tbody>
</table>

Kontaktfälten nedan synkroniseras för internt bruk.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Name]</td>
      <td>parentcustomerid</td>
    </tr>
  </tbody>
</table>

## Kontofält {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo Field</th>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Account (a)]</td>
      <td>[!UICONTROL Account]</td>
      <td>kontotid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Address]</td>
      <td>[!UICONTROL Address 1: Street 1]</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing City]</td>
      <td>[!UICONTROL Address 1: City]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Country]</td>
      <td>[!UICONTROL Address 1: Country/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Billing Postal Code]</td>
      <td>[!UICONTROL Address 1: Zip/Postal Code]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 2]</td>
      <td>[!UICONTROL Address 1: Street 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Billing Address 3]</td>
      <td>[!UICONTROL Address 1: Street 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Main Phone]</td>
      <td>[!UICONTROL Main Phone]</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Business Type]</td>
      <td>[!UICONTROL Business Type]</td>
      <td>företag, ekosystem</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Account Number]</td>
      <td>[!UICONTROL Account Number]</td>
      <td>kontonummer</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Company Status]</td>
      <td>[!UICONTROL Status]</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>[!UICONTROL Annual Revenue]</td>
      <td>intäkt</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company Notes]</td>
      <td>[!UICONTROL Description]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL Industry]</td>
      <td>[!UICONTROL Industry]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Website]</td>
      <td>[!UICONTROL Website]</td>
      <td>webbplats</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>antal anställda</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC Code]</td>
      <td>[!UICONTROL SIC Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Company]</td>
      <td>[!UICONTROL Account Name]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Num Employees]</td>
      <td>[!UICONTROL Number of Employees]</td>
      <td>antal anställda</td>
    </tr>
  </tbody>
</table>

Kontofälten nedan synkroniseras för internt bruk.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Created On]</td>
      <td>skapad</td>
    </tr>
  </tbody>
</table>

## Fält för affärsmöjlighet {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo Field</th>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Close Probability]</td>
      <td>[!UICONTROL Probabliity]</td>
      <td>stängningssannolikhet</td>
    </tr>
    <tr>
      <td>[!UICONTROL Stage]</td>
      <td>[!UICONTROL Status]</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>[!UICONTROL Actual Close Date]</td>
      <td>aktualclosedat</td>
    </tr>
    <tr>
      <td>[!UICONTROL Name]</td>
      <td>[!UICONTROL Topic]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estimated Value]</td>
      <td>[!UICONTROL Est. Revenue]</td>
      <td>measuredValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Description]</td>
      <td>[!UICONTROL Description]</td>
      <td>description</td>
    </tr>
  </tbody>
</table>

Kontofälten nedan synkroniseras för internt bruk.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-fält</th>
      <th>API-namn för MS Dynamics</th>
    </tr>
    <tr>
      <td>[!UICONTROL Owner] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Opportunity]</td>
      <td>OpportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Potential Customer]</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Microsoft-relaterade systemfält i Marketo (skrivskyddade) {#microsoft-related-system-fields}

Fälten nedan skapas i Marketo men kan inte justeras av användare.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo Field</th>
      <th>Beskrivning</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Type]</td>
      <td>Lead eller kontakt. Om det är tomt finns leadet bara som en person i Marketo</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Created Date]</td>
      <td>Skapad i [!DNL MS Dynamics] (kan skilja sig från Skapad i Marketo)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft is Deleted]</td>
      <td>Tidigare var personen i Microsoft men togs bort och bor nu endast i Marketo</td>
    </tr>
  </tbody>
</table>
