---
description: Standardfältmappning för Dynamics - Marketo Docs - produktdokumentation
title: Fältmappning för standardDynamics
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
source-git-commit: d87809e12f153d025f8d013ea52e06c0b6530154
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 12%

---

# Fältmappning för standardDynamics {#default-dynamics-field-mapping}

När du först synkroniserar ditt Marketo-konto med Microsoft skapar Marketo automatiskt dessa associationer mellan de inbyggda fälten i Dynamics och Marketo.  Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

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
      <td>Skapad av Microsoft</td>
      <td>Skapad den</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>Titel</td>
      <td>Titel</td>
      <td>hälsning</td>
    </tr>
    <tr>
      <td>Första</td>
      <td>Förnamn</td>
      <td>förnamn</td>
    </tr>
    <tr>
      <td>Mitten</td>
      <td>Mellannamn</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Sista</td>
      <td>Efternamn</td>
      <td>efternamn</td>
    </tr>
    <tr>
      <td>E-post</td>
      <td>E-post</td>
      <td>e-postadress1</td>
    </tr>
    <tr>
      <td>Befattning</td>
      <td>Befattning</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Tel.</td>
      <td>Telefon, arbete</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>Mobil</td>
      <td>Mobiltelefon</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>Adress</td>
      <td>Gatuadress 1</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>Ort</td>
      <td>Ort</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stat</td>
      <td>Stat/provins</td>
      <td>address1_stateorregion</td>
    </tr>
    <tr>
      <td>Land</td>
      <td>Land/region</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Postnummer</td>
      <td>Postnummer</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Personkälla</td>
      <td>Leadkälla</td>
      <td>leadsourccode</td>
    </tr>
    <tr>
      <td>Personstatus</td>
      <td>Status</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Statusorsak</td>
      <td>Statusorsak</td>
      <td>statuskod</td>
    </tr>
    <tr>
      <td>Personanteckningar</td>
      <td>Beskrivning</td>
      <td>description</td>
    </tr>
    <tr>
      <td>Ring inte</td>
      <td>Tillåt inte telefonsamtal</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Avprenumererad</td>
      <td>Massinte e-post</td>
      <td>donotbulkemi</td>
    </tr>
    <tr>
      <td>Personklassificering</td>
      <td>Klassificering</td>
      <td>leadqualityCode</td>
    </tr>
    <tr>
      <td>Microsoft-adress 2</td>
      <td>Gatuadress 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft-adress 3</td>
      <td>Gatuadress 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft skickar ingen e-post</td>
      <td>Tillåt inte e-post</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Fax</td>
      <td>Tillåt inte fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft skickar inte marknadsföringsmaterial</td>
      <td>Marknadsföringsmaterial</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>Microsoft hemtelefon</td>
      <td>Telefon, hem</td>
      <td>telefon2</td>
    </tr>
    <tr>
      <td>Microsoft föredragen kontaktmetod</td>
      <td>Önskad kontaktmetod</td>
      <td>preferredcontactMethodCode</td>
    </tr>
    <tr>
      <td>Microsoft Topic</td>
      <td>Ämne</td>
      <td>ämne</td>
    </tr>
    <tr>
      <td>Senaste intressanta datum</td>
      <td>Senaste intressanta datum</td>
      <td>mkt_lastinterest_potens</td>
    </tr>
    <tr>
      <td>Senaste intressanta stund desc</td>
      <td>Senaste intressanta stund desc</td>
      <td>mkt_lastinterest_potdesc</td>
    </tr>
    <tr>
      <td>Källa för senaste intressanta stund</td>
      <td>Källa för senaste intressanta stund</td>
      <td>mkt_leadinterest_potens</td>
    </tr>
    <tr>
      <td>Senaste intressanta stund</td>
      <td>Senaste intressanta stund</td>
      <td>mkt_lastIntresseDriftstyp</td>
    </tr>
    <tr>
      <td>Företag</td>
      <td>Företagets namn</td>
      <td>företagsnamn</td>
    </tr>
    <tr>
      <td>Relativa poäng</td>
      <td>Relativa poäng</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Prioritet</td>
      <td>Prioritet</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Relativ brådskande situation</td>
      <td>brådska</td>
      <td>mkt_urgent</td>
    </tr>
    <tr>
      <td>Ämne</td>
      <td>Ämne</td>
      <td>ämne</td>
    </tr>
    <tr>
      <td>Årlig intäkt</td>
      <td>Årlig intäkt</td>
      <td>omsättning</td>
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
      <td>Ägare </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>skapad den</td>
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
      <td>Skapad av Microsoft</td>
      <td>Skapad den</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>Titel</td>
      <td>Titel</td>
      <td>hälsning</td>
    </tr>
    <tr>
      <td>Första</td>
      <td>Förnamn</td>
      <td>förnamn</td>
    </tr>
    <tr>
      <td>Mitten</td>
      <td>Mellannamn</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Sista</td>
      <td>Efternamn</td>
      <td>efternamn</td>
    </tr>
    <tr>
      <td>E-post</td>
      <td>E-post</td>
      <td>e-postadress1</td>
    </tr>
    <tr>
      <td>Befattning</td>
      <td>Befattning</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Tel.</td>
      <td>Telefon, arbete</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>Mobil</td>
      <td>Mobiltelefon</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>Adress</td>
      <td>Adress 1: Gatuadress 1</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>Ort</td>
      <td>Adress 1: Ort</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stat</td>
      <td>Adress 1: Stat/provins</td>
      <td>address1_stateorregion</td>
    </tr>
    <tr>
      <td>Land</td>
      <td>Adress 1: Land/region</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Postnummer</td>
      <td>Adress 1: Postnummer</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Personstatus</td>
      <td>Status</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Statusorsak</td>
      <td>Statusorsak</td>
      <td>statuskod</td>
    </tr>
    <tr>
      <td>Ring inte</td>
      <td>Tillåt inte telefonsamtal</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Avprenumererad</td>
      <td>Massinte e-post</td>
      <td>donotbulkemi</td>
    </tr>
    <tr>
      <td>Microsoft-adress 2</td>
      <td>Adress 1: Gatuadress 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft-adress 3</td>
      <td>Adress 1: Gatuadress 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft skickar ingen e-post</td>
      <td>Tillåt inte e-post</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft hemtelefon</td>
      <td>Telefon, hem</td>
      <td>telefon2</td>
    </tr>
    <tr>
      <td>Microsoft föredragen kontaktmetod</td>
      <td>Önskad kontaktmetod</td>
      <td>preferredcontactMethodCode</td>
    </tr>
    <tr>
      <td>Senaste intressanta datum</td>
      <td>Senaste intressanta datum</td>
      <td>mkt_lastinterest_potens</td>
    </tr>
    <tr>
      <td>Senaste intressanta stund</td>
      <td>Senaste intressanta stund</td>
      <td>mkt_lastIntresseDriftstyp</td>
    </tr>
    <tr>
      <td>Källa för senaste intressanta stund</td>
      <td>Källa för senaste intressanta stund</td>
      <td>mkt_leadinterest_potens</td>
    </tr>
    <tr>
      <td>Senaste intressanta stund desc</td>
      <td>Senaste intressanta stund desc</td>
      <td>mkt_lastinterest_potdesc</td>
    </tr>
    <tr>
      <td>Microsoft skickar inte marknadsföringsmaterial</td>
      <td>Marknadsföringsmaterial</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Fax</td>
      <td>Microsoft Do Not Fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Prioritet</td>
      <td>Prioritet</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Relativ brådskande situation</td>
      <td>brådska</td>
      <td>mkt_urgent</td>
    </tr>
    <tr>
      <td>Relativa poäng</td>
      <td>Relativa poäng</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Personanteckningar</td>
      <td>Beskrivning</td>
      <td>description </td>
    </tr>
    <tr>
      <td>Personpoäng</td>
      <td>Leadpoäng</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>Personanteckningar</td>
      <td>Beskrivning</td>
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
      <td>Ägare </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>skapad den</td>
      <td>skapad</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Företagets namn</td>
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
      <td>Konto (a)</td>
      <td>Konto</td>
      <td>konto</td>
    </tr>
    <tr>
      <td>Faktureringsadress</td>
      <td>Adress 1: Gatuadress 1</td>
      <td>adress1_rad1</td>
    </tr>
    <tr>
      <td>Faktureringsort</td>
      <td>Adress 1: Ort</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Faktureringsland</td>
      <td>Adress 1: Land/region</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Faktureringspostnummer</td>
      <td>Adress 1: Postnummer</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Microsoft faktureringsadress 2</td>
      <td>Adress 1: Gatuadress 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft faktureringsadress 3</td>
      <td>Adress 1: Gatuadress 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Telefon</td>
      <td>Telefon</td>
      <td>telefon1</td>
    </tr>
    <tr>
      <td>Affärstyp</td>
      <td>Affärstyp</td>
      <td>företag, ekosystem</td>
    </tr>
    <tr>
      <td>Microsoft-kontonummer</td>
      <td>Kontonummer</td>
      <td>kontonummer</td>
    </tr>
    <tr>
      <td>Microsoft företagsstatus</td>
      <td>Status</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Årlig intäkt</td>
      <td>Årlig intäkt</td>
      <td>omsättning</td>
    </tr>
    <tr>
      <td>Företagsanteckningar</td>
      <td>Beskrivning</td>
      <td>description</td>
    </tr>
    <tr>
      <td>Bransch</td>
      <td>Bransch</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>SNI-kod</td>
      <td>SNI-kod</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Webbplats</td>
      <td>Webbplats</td>
      <td>webbplats</td>
    </tr>
    <tr>
      <td>Antal anställda</td>
      <td>Antal anställda</td>
      <td>antal anställda</td>
    </tr>
    <tr>
      <td>SNI-kod</td>
      <td>SNI-kod</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Företag</td>
      <td>name</td>
      <td>Kontonamn</td>
    </tr>
    <tr>
      <td>Antal anställda</td>
      <td>Antal anställda</td>
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
      <td>Ägare </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>skapad den</td>
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
      <td>Nära sannolikhet</td>
      <td>Sannolikhet</td>
      <td>stängningssannolikhet</td>
    </tr>
    <tr>
      <td>Scen</td>
      <td>status</td>
      <td>statcode</td>
    </tr>
    <tr>
      <td>Faktiskt stängningsdatum</td>
      <td>Faktiskt stängningsdatum</td>
      <td>aktualclosedat</td>
    </tr>
    <tr>
      <td>Namn</td>
      <td>Ämne</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Beräknat värde</td>
      <td>Beräkna. Intäkter</td>
      <td>measuredValue</td>
    </tr>
    <tr>
      <td>Beskrivning</td>
      <td>Beskrivning</td>
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
      <td>Ägare </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Möjligheter</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>Potentiell kund</td>
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
      <td>Microsoft Type</td>
      <td>Lead eller kontakt. Om det är tomt finns leadet bara som en person i Marketo</td>
    </tr>
    <tr>
      <td>Skapad av Microsoft</td>
      <td>Skapad i MS Dynamics (kan vara ett annat datum än Skapad i Marketo)</td>
    </tr>
    <tr>
      <td>Microsoft tas bort</td>
      <td>Tidigare var personen i Microsoft men togs bort och bor nu endast i Marketo</td>
    </tr>
  </tbody>
</table>
