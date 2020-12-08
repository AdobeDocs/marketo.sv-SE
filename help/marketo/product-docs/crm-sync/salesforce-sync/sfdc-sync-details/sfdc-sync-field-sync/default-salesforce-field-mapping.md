---
unique-page-id: 4719314
description: Standardfältmappning i Salesforce - Marketo Docs - Produktdokumentation
title: Standardfältmappning för Salesforce
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Standardfältmappning för Salesforce {#default-salesforce-field-mapping}

När du först synkroniserar ditt Marketto-konto med Salesforce skapar Marketo automatiskt dessa associationer mellan dina inbyggda Salesforce- och Marketo-fält. Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

## Leadfält {#lead-fields}

| SFDC-fält | Marketo-fält |
|---|---|
| Årsintäkt | Årsintäkt |
| Ort | Ort |
| Företag | Företag |
| Konverterat den | SFDC-konverteringsdatum |
| Land | Land |
| Skapad den | Skapad SFDC |
| Beskrivning | Personanteckningar |
| E-post | E-postadress |
| Fax | Faxnummer |
| Förnamn | Förnamn |
| Avanmäl dig via e-post | Avbeställ |
| Bransch | Bransch |
| Konverterad | SFDC är konverterat |
| Borttagen | SFDC tas bort |
| Efternamn | Efternamn |
| Leadkälla | Källa |
| Leadpoäng | Poäng |
| Mobiltelefon | Mobiltelefonnummer |
| Anställda | Antal anställda |
| Telefon | Telefonnummer |
| Postnummer | Postnummer |
| Klassificering | Klassificering |
| Hälsning | Hälsning |
| Stat/provins | Läge |
| Status | Status |
| Gata | Adress |
| Titel | Befattning |
| Webbplats | Webbplats |

## Kontaktfält {#contact-fields}

| SFDC-fält | Marketo-fält |
|---|---|
| Födelsedatum | Födelsedatum |
| Skapad den | Skapad SFDC |
| Kontaktbeskrivning | Personanteckningar |
| E-post | E-postadress |
| Fax, arbete | Faxnummer |
| Förnamn | Förnamn |
| Avanmäl dig via e-post | Avbeställ |
| Borttagen | SFDC tas bort |
| Efternamn | Efternamn |
| Leadkälla | Källa |
| Leadpoäng | Poäng |
| MailingCity | Ort |
| MailingCountry | Land |
| MailingPostalCode | Postnummer |
| MailingState | Läge |
| MailingStreet | Adress |
| Mobiltelefon | Mobiltelefonnummer |
| Telefon, arbete | Telefonnummer |
| Hälsning | Hälsning |
| Titel | Befattning |

## Kontofält {#account-fields}

| SFDC-fält | Marketo-fält |
|---|---|
| Årsintäkt | Årsintäkt |
| Faktureringsort | Faktureringsort |
| Faktureringsland | Faktureringsland |
| Postnummer för fakturering | Postnummer för fakturering |
| Faktureringsstat/provins | Faktureringsläge |
| Faktureringsgatan | Faktureringsadress |
| Kontobeskrivning | Företagsanteckningar |
| Bransch | Bransch |
| Borttagen | SFDC tas bort |
| Kontonamn | Företag |
| Anställda | Antal anställda |
| Telefon till konto | Huvudtelefon |
| SIC-kod | SIC-kod |
| Kontowebbplats | Plats |
| Kontotyp | SFDC-typ |
| Webbplats | Webbplats |

## Salesforce-relaterade systemfält i Marketo (skrivskyddat) {#salesforce-related-system-fields-in-marketo-read-only}

Dessa fält skapas i Marketo men kan inte justeras av kunder.

| Fält | Beskrivning |
|---|---|
| SFDC-ID | Salesforce-ID med 18 tecken |
| SFDC-typ | Lead eller kontakt. Om det är tomt finns leadet bara som en person i Marketo |
| Skapad SFDC | Skapad i SFDC (kan vara ett annat datum än Skapad i Marketo) |
| SFDC tas bort | Personen brukade vara i SFDC men togs bort och bor nu bara i Marketo |
