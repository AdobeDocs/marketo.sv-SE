---
description: Standardfältmappning för Dynamics - Marketo Docs - Produktdokumentation
title: Fältmappning för standardDynamics
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Standardfältmappning för Dynamics {#default-dynamics-field-mapping}

När du först synkroniserar ditt Markto-konto med Microsoft skapar Marketo automatiskt dessa associationer mellan dina inbyggda Dynamics- och Marketo-fält.  Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

## Leadfält {#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-fält</th> 
   <th>MS Dynamics-fält</th> 
   <th>API-namn för MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Skapad av Microsoft</td> 
   <td>Skapad den</td> 
   <td>skapad</td> 
  </tr> 
  <tr> 
   <td>Hälsning</td> 
   <td>Hälsning</td> 
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
   <td>Telefon</td> 
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
   <td>Läge</td> 
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
   <td>Avbeställ</td> 
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
   <td>Microsoft Skicka inte e-post</td> 
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
   <td>Microsoft Home Phone</td> 
   <td>Telefon, hem</td> 
   <td>telefon2</td> 
  </tr> 
  <tr> 
   <td>Microsoft-kontaktmetod</td> 
   <td>Önskad kontaktmetod</td> 
   <td>preferredcontactMethodCode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-ämne</td> 
   <td>Ämne</td> 
   <td>ämne</td> 
  </tr> 
 </tbody> 
</table>

## Kontaktfält {#contact-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-fält</th> 
   <th>MS Dynamics-fält</th> 
   <th>API-namn för MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Skapad av Microsoft</td> 
   <td>Skapad den</td> 
   <td>skapad</td> 
  </tr> 
  <tr> 
   <td>Hälsning</td> 
   <td>Hälsning</td> 
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
   <td>Telefon</td> 
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
   <tr> 
   <td>Ort</td> 
   <td>Adress 1: Ort</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Läge</td> 
   <td>Adress 1: Stat/provins</td> 
   <td>address1_stateorregion</td> 
  </tr> 
  <tr> 
   <td>Land</td> 
   <td>Adress 1: Land/region</td> 
   <td>address1_country</td> 
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
   <td>Avbeställ</td> 
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
   <td>Microsoft Skicka inte e-post</td> 
   <td>Tillåt inte e-post</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>Telefon, hem</td> 
   <td>telefon2</td> 
  </tr> 
  <tr> 
   <td>Microsoft-kontaktmetod</td> 
   <td>Önskad kontaktmetod</td> 
   <td>preferredcontactMethodCode</td> 
  </tr> 
 </tbody> 
</table>

## Kontofält {#account-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-fält</th> 
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
   <td>Postnummer för fakturering</td> 
   <td>Adress 1: Postnummer</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsofts faktureringsadress 2</td> 
   <td>Adress 1: Gatuadress 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsofts faktureringsadress 3</td> 
   <td>Adress 1: Gatuadress 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Huvudtelefon</td> 
   <td>Huvudtelefon</td> 
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
   <td>Microsoft-företagsstatus</td> 
   <td>Status</td> 
   <td>statcode</td> 
  </tr> 
  <tr> 
   <td>Årsintäkt</td> 
   <td>Årsintäkt</td> 
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
   <td>SIC-kod</td> 
   <td>SIC-kod</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Webbplats</td> 
   <td>Webbplats</td> 
   <td>webbplats</td> 
  </tr> 
 </tbody> 
</table>

## Microsoft-relaterade systemfält i Marketo (skrivskyddat) {#microsoft-related-system-fields-in-marketo}

Dessa fält skapas i Marketo men kan inte justeras av kunder.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-fält</th> 
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
   <td>Microsoft har tagits bort</td> 
   <td>Personen brukade vara i Microsoft men togs bort och bor nu bara i Marketo</td> 
  </tr> 
 </tbody> 
</table>
