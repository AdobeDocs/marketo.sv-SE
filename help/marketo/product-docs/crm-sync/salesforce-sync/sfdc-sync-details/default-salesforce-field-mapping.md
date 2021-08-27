---
unique-page-id: 4719314
description: Standardfältmappning för Salesforce - Marketo Docs - produktdokumentation
title: Standardfältmappning för Salesforce
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 34%

---

# Standardfältmappning för Salesforce {#default-salesforce-field-mapping}

När du först synkroniserar ditt Marketo-konto med Salesforce skapar Marketo automatiskt dessa associationer mellan dina inbyggda Salesforce- och Marketo-fält. Marketo synkroniserar även dina anpassade fält på leads, konton, säljprojekt och kontakter.

## Leadfält {#lead-fields}

| SFDC-fält | Marketo |
|---|---|
| Årlig intäkt | Årlig intäkt |
| Ort | Ort |
| Företag | Företagets namn |
| Konverterat den | SFDC-konverteringsdatum |
| Land | Land |
| Skapad den | Skapad SFDC |
| Beskrivning | Personanteckningar |
| E-post | E-postadress |
| Fax | Faxnummer |
| Förnamn | Förnamn |
| Avanmäl dig via e-post | Avprenumererad |
| Bransch | Bransch |
| Konverterad | SFDC är konverterat |
| Borttagen | SFDC tas bort |
| Efternamn | Efternamn |
| Leadkälla | Källa |
| Leadpoäng | Poäng |
| Mobiltelefon | Mobiltelefon |
| Anställda | Antal anställda |
| Tel. | Telefonnummer |
| Postnummer | Postnummer |
| Klassificering | Klassificering |
| Titel | Titel |
| Stat/provins | Stat |
| Status | Status |
| Gata | Adress |
| Titel | Befattning |
| Webbplats | Webbplats |

## Kontaktfält {#contact-fields}

| SFDC-fält | Marketo |
|---|---|
| Födelsadatum | Födelsedatum |
| Skapad den | Skapad SFDC |
| Kontaktbeskrivning | Personanteckningar |
| E-post | E-postadress |
| Fax, arbete | Faxnummer |
| Förnamn | Förnamn |
| Avanmäl dig via e-post | Avprenumererad |
| Borttagen | SFDC tas bort |
| Efternamn | Efternamn |
| Leadkälla | Källa |
| Leadpoäng | Poäng |
| MailingCity | Ort |
| MailingCountry | Land |
| MailingPostalCode | Postnummer |
| MailingState | Stat |
| MailingStreet | Adress |
| Mobiltelefon | Mobiltelefon |
| Telefon, arbete | Telefonnummer |
| Titel | Titel |
| Titel | Befattning |

## Kontofält {#account-fields}

| SFDC-fält | Marketo |
|---|---|
| Årlig intäkt | Årlig intäkt |
| Faktureringsort | Faktureringsort |
| Faktureringsland | Faktureringsland |
| Postnummer för fakturering | Faktureringspostnummer |
| Faktureringsstat/provins | Faktureringsstat |
| Faktureringsgatan | Faktureringsadress |
| Kontobeskrivning | Företagsanteckningar |
| Bransch | Bransch |
| Borttagen | SFDC tas bort |
| Kontonamn | Företagets namn |
| Anställda | Antal anställda |
| Telefon till konto | Telefon |
| SNI-kod | SNI-kod |
| Kontowebbplats | Plats |
| Kontotyp | SFDC-typ |
| Webbplats | Webbplats |

## Salesforce-relaterade systemfält i Marketo (skrivskyddade) {#salesforce-related-system-fields-in-marketo-read-only}

Dessa fält skapas i Marketo men kan inte justeras av kunder.

| Fält | Beskrivning |
|---|---|
| SFDC-ID | Salesforce-ID med 18 tecken |
| SFDC-typ | Lead eller kontakt. Om det är tomt finns leadet bara som en person i Marketo |
| Skapad SFDC | Skapad i SFDC (kan vara ett annat datum än Skapad i Marketo) |
| SFDC tas bort | Personen brukade befinna sig i SFDC men togs bort och bor nu bara i Marketo |
