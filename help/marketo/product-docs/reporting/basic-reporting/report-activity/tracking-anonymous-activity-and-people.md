---
unique-page-id: 2360181
description: Spåra anonym aktivitet och människor - Marketo Docs - Produktdokumentation
title: Spåra anonym aktivitet och människor
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Spåra anonym aktivitet och personer {#tracking-anonymous-activity-and-people}

Första gången någon besöker en Marketo [landningssida](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (eller en sida på din webbplats som har [Munchkin-spårningskoden](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) skapar Marketo en _anonym aktivitet_ och använder en webbläsarcookie för att spåra den. När besökaren identifieras blir den en person och historiken som är kopplad till webbläsarens cookie sammanfogas.

1. En anonym aktivitet skapas när någon:

   * Besök din Marketo [landningssida](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) första gången.
   * Besöker en sida på webbplatsen som har [Munchkin-spårning](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Klicka på länken [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) i ett Marketo-e-postmeddelande.

   >[!NOTE]
   >
   >Till skillnad från andra länkar i Marketo-e-postmeddelanden spåras inte Visa som webbsida som ett e-postklick.

   En anonym aktivitet sammanfogas till en ny eller befintlig person när någon:

   * Klicka på en [länk i ett Marketo-e-postmeddelande](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Fyller i ett Marketo [formulär](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Använder Marketos [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) eller [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API (för utvecklare) för att associera en anonym aktivitet med en känd post.

   Ett namn i databasen kan vara knutet till många cookies eftersom användare ofta använder olika enheter och webbläsare för att besöka webbplatsen.

   >[!NOTE]
   >
   >När anonyma poster sammanfogas till en ny eller befintlig personpost kommer anpassade fältvärden att **inte** överföra över.

   >[!MORELIKETHIS]
   >
   >[Visa personer eller anonyma besökare i webbrapporter](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
