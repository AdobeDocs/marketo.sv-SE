---
unique-page-id: 1147322
description: Förstå anonym aktivitet och människor - Marketo Docs - produktdokumentation
title: Förstå anonym aktivitet och människor
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Förstå anonym aktivitet och människor {#understanding-anonymous-activity-and-people}

Första gången någon besöker en Marketo-landningssida (eller en sida på din webbplats som har [Munchkin Tracking Code](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}) skapar Marketo *anonym aktivitet* och använder en webbläsarcookie för att spåra den. När den har identifierats blir den en person och historiken som är kopplad till deras webbläsarcookie sammanfogas i.

>[!IMPORTANT]
>
>Aktivera betafunktionen **Munchkin V2 Anonym repriser på kända** säkerställer att kampanjer som triggas av anonyma kampanjer alltid spelas upp efter att det anonyma leadet har slagits samman till det kända registret. Därför behålls anpassade fält som ändrats genom steg för att ändra datavärde i alla återspelade kampanjer i den kända posten.

**En anonym person** aktiviteten skapas när någon:

* Besök Marketo startsida första gången.
* Besöker en sida på webbplatsen som har [Munchkin tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Klicka på [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} i ett Marketo-mejl.

>[!NOTE]
>
>Till skillnad från andra länkar i Marketo mejl [Visa som webbsida](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} spåras inte som ett e-postklick.

En anonym aktivitet sammanfogas till en ny eller befintlig person när någon:

* Klicka på en [länk i ett Marketo-mejl](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Fyller i en Marketo [Formulär](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}.
* Använder Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} or [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API (för utvecklare) för att associera en anonym person med en känd post.

Ett namn i databasen kan vara knutet till många cookies eftersom användare ofta använder olika enheter och webbläsare för att besöka webbplatsen.

>[!NOTE]
>
>När anonyma poster sammanfogas till en ny eller befintlig personpost, kommer anpassade fältvärden att *not* överflyttning.
