---
unique-page-id: 5472615
description: Understanding System Managed Fields - Marketo Docs - Product Documentation
title: Förstå systemhanterade fält
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Förstå systemhanterade fält {#understanding-system-managed-fields}

Du kan ha lagt märke till att [personinformationssidan](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) innehåller en serie icke-redigerbara fält som skapats av Marketo. Dessa data kommer från olika källor och det finns otaliga värden som kan visas.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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
| Infört företag | Marketos bästa gissning (baserat på IP) för personens företag |
| Inaktuell ort | Marketos bästa gissning (baserat på IP) för personens ort |
| Ingångsregion | Marketos bästa gissning (baserat på IP) för personens stat eller region |
| Infört postnummer | Marketos bästa gissning (baserat på IP) av personens postnummer |
| Infört land | Marketos bästa gissning (baserat på IP) för personens land |
| Ingående metropolitområde | Marketos bästa gissning (baserat på IP) i personens storstadsområde |
| Riktnummer för inkommande telefon | Marketos bästa gissning (baserat på IP) för personens riktnummer |

## Möjliga värden för ursprungs- och registreringskälltyp {#possible-values-for-original-and-registration-source-type}

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
| Munchkin API | Personen upptäcktes av Marketos Munchkin API |
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
| Munchkin API | Bli en person via Marketos Munchkin API |
| Social app | Bli en person via en social widget |
| Evenemangspartner | Bli en person via en länkad webbinärtjänst |

