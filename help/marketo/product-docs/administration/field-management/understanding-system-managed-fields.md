---
unique-page-id: 5472615
description: Om systemhanterade fält - Marketo Docs - produktdokumentation
title: Förstå systemhanterade fält
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Förstå systemhanterade fält {#understanding-system-managed-fields}

Du kan ha lagt märke till att [personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} innehåller en serie fält som inte kan redigeras och som har skapats av Marketo. Dessa data kommer från olika källor och det finns otaliga värden som kan visas.

## Fälttyper {#field-types}

| **Fältnamn** | **Definition** |
|---|---|
| Ursprunglig Source-typ | Den plats där en person eller en besökare på webbplatsen först upptäcktes (Exempel: Listimport, Webbsidesbesök) |
| Ursprunglig Source-information | Specifikationer om den platsen (Exempel: listans namn, webbsidans URL) |
| Ursprunglig sökmotor | Om tillämpligt, sökmotorn som refererade personen till den ursprungliga källan |
| Ursprunglig sökfras | Om tillämpligt, det sökord som refererade personen till den ursprungliga inmatningskällan |
| Ursprunglig referens | URL som var värd för den ursprungliga inmatningskällan |
| Registrera Source Type | Den plats där en aktivitet först blev en person (Exempel: Listimport, Webbsidesbesök) |
| Registrera Source Info | Specifikationer om den platsen (Exempel: listans namn, webbsidans URL) |
| Anonym IP | Anger en persons IP-adress |
| Berört företag | Marketo bästa gissning (baserat på IP) för personens företag |
| Inaktuell ort | Marketo bästa gissning (baserat på IP) för personens ort |
| Ingångsregion | Marketo bästa gissning (baserat på IP) för personens stat eller region |
| Infört postnummer | Marketo bästa gissning (baserat på IP) för personens postnummer |
| Berört land | Marketo bästa gissning (baserat på IP) för personens land |
| Ingående metropolitområde | Marketo bästa gissning (baserat på IP) för personens storstadsområde |
| Riktnummer för inkommande telefon | Marketo bästa gissning (baserat på IP) för personens riktnummer |

## Möjliga värden för Source-typen Original och Registration {#possible-values-for-original-and-registration-source-type}

Nedan finns några möjliga värden och vad de betyder.

| **Ursprunglig Source-typ** | **Definition** |
|---|---|
| Salesforce.com | Personen upptäcktes från en [!DNL Webhook]-synkronisering |
| Webbsidesbesök | En person upptäcktes från en webbsida |
| Fylla i webbformulär | En person upptäcktes när ett formulär fylldes i |
| Listimport | Personen upptäcktes från en listimport |
| Ny person | Personen har angetts manuellt i databasen |
| Klicka på webblänk | Personen upptäcktes efter att ha klickat på en länk |
| E-postadress | Personen fick ett e-postmeddelande via [!DNL Sales Insight] e-posttillägg |
| Person | Personen synkroniserades från [!DNL Salesforce] som en person |
| Kontakt | Personen synkroniserades från [!DNL Webhook] som en kontakt |
| API för [!DNL Munchkin] | Personen upptäcktes av Marketo Engage [!DNL Munchkin] API |
| Social app | Personen upptäcktes av en social widget |
| Webbtjänstens API | Personen upptäcktes av ett webbtjänste-API |
| Evenemangspartner | Personen upptäcktes via en synkroniserad webbinatjänst |
| Associera lead | Person som har slagits samman via Associate Lead API-anrop |

| **Registrera Source Type** | **Definition** |
|---|---|
| Listimport | Bli en person genom en listimport |
| Salesforce.com | Blev en person via en [!DNL Webhook]-synkronisering |
| Fylla i webbformulär | Bli en person efter att ha fyllt i ett formulär |
| E-postadress | Personen fick ett e-postmeddelande via [!DNL Webhook] e-posttillägg |
| Webbtjänstens API | Personen skapades via SOAP/REST API |
| Ny person | Personen har angetts manuellt i databasen |
| API för [!DNL Munchkin] | Bli en person via Marketo [!DNL Munchkin] API |
| Social app | Bli en person via en social widget |
| Evenemangspartner | Bli en person via en länkad webbinatjänst |
