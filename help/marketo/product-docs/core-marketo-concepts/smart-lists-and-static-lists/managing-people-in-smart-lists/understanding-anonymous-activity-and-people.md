---
unique-page-id: 1147322
description: Förstå anonym aktivitet och människor - Marketo Docs - Produktdokumentation
title: Förstå anonym aktivitet och människor
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Förstå anonym aktivitet och personer {#understanding-anonymous-activity-and-people}

Första gången någon besöker en Marketo-landningssida (eller en sida på din webbplats som har [Munchkin Tracking Code](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), skapar Marketo en _anonym aktivitet_ och använder en webbläsarcookie för att spåra den. När den har identifierats blir den en person och historiken som är kopplad till deras webbläsarcookie sammanfogas i.

**En** anonym aktivitet skapas när någon:

* Besök din Markets landningssida första gången.
* Besöker en sida på webbplatsen som har [Munchkin-spårning](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Klicka på länken [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) i ett Marketo-e-postmeddelande.

>[!NOTE]
>
>Till skillnad från andra länkar i Marketo-e-postmeddelanden spåras inte [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) som ett e-postklick.

En anonym aktivitet sammanfogas till en ny eller befintlig person när någon:

* Klicka på en [länk i ett Marketo-e-postmeddelande](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Fyller i ett Marketo [Formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Använder Marketos [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) eller [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (för utvecklare) för att associera en anonym person med en känd post.

Ett namn i databasen kan vara knutet till många cookies eftersom användare ofta använder olika enheter och webbläsare för att besöka webbplatsen.

>[!NOTE]
>
>När anonyma poster sammanfogas till en ny eller befintlig personpost kommer anpassade fältvärden att **inte** överföra över.
