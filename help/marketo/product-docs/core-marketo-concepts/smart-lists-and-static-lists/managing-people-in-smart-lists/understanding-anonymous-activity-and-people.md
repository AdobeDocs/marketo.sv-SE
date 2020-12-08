---
unique-page-id: 1147322
description: Förstå anonym aktivitet och människor - Marketo Docs - Produktdokumentation
title: Förstå anonym aktivitet och människor
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# Förstå anonym aktivitet och människor {#understanding-anonymous-activity-and-people}

Första gången någon besöker en Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (eller en sida på din webbplats som har [Munchkin Tracking Code](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) skapar Marketo en *anonym **aktivitet* och använder en webbläsar-cookie för att spåra den. När den har identifierats blir den en person och historiken som är kopplad till deras webbläsarcookie sammanfogas i.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

**En anonym** aktivitet skapas när någon:

* Besök din Markets landningssida första gången.

* Besöker en sida på webbplatsen som har [Munchkin-spårning](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).

* Klicka på länken [Visa som webbsida](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) i ett Marketo-e-postmeddelande.

>[!NOTE]
>
>Till skillnad från andra länkar i Marketo-e-postmeddelanden spåras inte [Visa som webbsida](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) som ett e-postklick.

En anonym aktivitet sammanfogas till en ny eller befintlig person när någon:

* Klicka på en [länk i ett Marketo-e-postmeddelande](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Fyller i ett Marketo- [formulär](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Använder Marketos [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) - eller [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) -API (för utvecklare) för att associera en anonym person med en känd post.

Ett namn i databasen kan vara knutet till många cookies eftersom användare ofta använder olika enheter och webbläsare för att besöka webbplatsen.

>[!NOTE]
>
>När anonyma poster sammanfogas till en ny eller befintlig personpost överförs **inte** anpassade fältvärden över.

