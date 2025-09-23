---
unique-page-id: 2360181
description: Spåra anonym aktivitet och människor - Marketo Docs - produktdokumentation
title: Spåra anonym aktivitet och människor
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Spåra anonym aktivitet och människor {#tracking-anonymous-activity-and-people}

Första gången någon besöker en [landningssida](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) för Marketo (eller en sida på din webbplats som har [Munchkin spårningskod](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) skapar Marketo en _anonym aktivitet_ och använder en webbläsarcookie för att spåra den. När besökaren identifieras blir den en person och historiken som är kopplad till webbläsarens cookie sammanfogas.

1. En anonym aktivitet skapas när någon:

   * Besök Marketo [landningssida](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) första gången.
   * Besöker en sida på webbplatsen som har [Munchkin tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Klicka på länken [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) i ett Marketo-e-postmeddelande.

   >[!NOTE]
   >
   >Till skillnad från andra länkar i Marketo e-postmeddelanden spåras inte Visa som webbsida som ett e-postklick.

   En anonym aktivitet sammanfogas till en ny eller befintlig person när någon:

   * Klicka på en [länk i ett Marketo-mejl](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Fyller i ett [formulär](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) från Marketo.
   * Använder Marketo [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/lead-database/leads) eller [Munchkin](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) API (för utvecklare) för att associera en anonym aktivitet med en känd post.

   Ett namn i databasen kan vara knutet till många cookies eftersom användare ofta använder olika enheter och webbläsare för att besöka webbplatsen.

   >[!NOTE]
   >
   >När anonyma poster sammanfogas till en ny eller befintlig personpost, kommer anpassade fältvärden **inte** att överföras över.

   >[!MORELIKETHIS]
   >
   >[Visa personer eller anonyma besökare i webbrapporter](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
