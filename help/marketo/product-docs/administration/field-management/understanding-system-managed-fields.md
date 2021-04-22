---
unique-page-id: 5472615
description: Understanding System Managed Fields - Marketo Docs - Product Documentation
title: Förstå systemhanterade fält
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Om systemhanterade fält {#understanding-system-managed-fields}

Du kan ha lagt märke till att sidan [personinformation](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) innehåller en serie icke-redigerbara fält som skapats av Marketo. Dessa data kommer från olika källor och det finns otaliga värden som kan visas.

## Fälttyper {#field-types}

| **Fältnamn** | **Definition** |
|---|---|
| Ursprunglig källtyp | Den plats där en person eller en besökare på webbplatsen först upptäcktes (Exempel: List Import, Web Page Visit) |
| Ursprunglig källinformation | Specifikationer om den platsen (Exempel: Namn på listan, webbsidans URL) |
| Ursprunglig sökmotor | Om tillämpligt, sökmotorn som refererade personen till den ursprungliga källan |
| Ursprunglig sökfras | Om tillämpligt, det sökord som refererade personen till den ursprungliga inmatningskällan |
| Ursprunglig referens | URL som var värd för den ursprungliga inmatningskällan |
| Typ av registreringskälla | Den plats där en aktivitet först blev en person (Exempel: List Import, Web Page Visit) |
| Information om registreringskälla | Specifikationer om den platsen (Exempel: Namn på listan, webbsidans URL) |
| Anonym IP | Anger en persons IP-adress |
| Berört företag | Marketo bästa gissning (baserat på IP) för personens företag |
| Inaktuell ort | Marketo bästa gissning (baserat på IP) för personens ort |
| Ingångsregion | Marketo bästa gissning (baserat på IP) för personens stat eller region |
| Infört postnummer | Marketo bästa gissning (baserat på IP) för personens postnummer |
| Berört land | Marketo bästa gissning (baserat på IP) för personens land |
| Ingående metropolitområde | Marketo bästa gissning (baserat på IP) för personens storstadsområde |
| Riktnummer för inkommande telefon | Marketo bästa gissning (baserat på IP) för personens riktnummer |

## Möjliga värden för ursprunglig och registreringskälltyp {#possible-values-for-original-and-registration-source-type}

Nedan finns några möjliga värden och vad de betyder.

| **Ursprunglig källtyp** | **Definition** |
|---|---|
| Salesforce.com | Personen upptäcktes från en Salesforce-synkronisering |
| Webbsidesbesök | En person upptäcktes från en webbsida |
| Fylla i webbformulär | En person upptäcktes när ett formulär fylldes i |
| Importera lista | Personen upptäcktes från en listimport |
| Ny person | Personen har angetts manuellt i databasen |
| Klicka på webblänk | Personen upptäcktes efter att ha klickat på en länk |
| E-postadress | Personen fick ett e-postmeddelande via e-posttillägget Sales Insight |
| Person | Personen synkroniserades från Salesforce som en person |
| Kontakt | Personen synkroniserades från Salesforce som en kontakt |
| Munchkin API | En person upptäcktes av Marketo Munchkin API |
| Social app | Personen upptäcktes av en social widget |
| Webbtjänstens API | Personen upptäcktes av ett webbtjänste-API |
| Evenemangspartner | Personen upptäcktes via en synkroniserad webbinatjänst |
| Associera lead | Person som har slagits samman via Associate Lead API-anrop |

| **Typ av registreringskälla** | **Definition** |
|---|---|
| Importera lista | Bli en person genom en listimport |
| Salesforce.com | Bli en person via en Salesforce-synkronisering |
| Fylla i webbformulär | Bli en person efter att ha fyllt i ett formulär |
| E-postadress | Personen fick ett e-postmeddelande via e-posttillägget Sales Insight |
| Webbtjänstens API | Personen skapades via SOAP/REST API |
| Ny person | Personen har angetts manuellt i databasen |
| Munchkin API | Bli en person med Marketo Munchkins API |
| Social app | Bli en person via en social widget |
| Evenemangspartner | Bli en person via en länkad webbinärtjänst |
