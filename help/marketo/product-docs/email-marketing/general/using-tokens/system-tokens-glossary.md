---
unique-page-id: 1147344
description: Systemtokens - ordlista - Marketo Docs - produktdokumentation
title: Ordlista för systemtoken
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Ordlista för systemtoken {#system-tokens-glossary}

Förutom persontokens kan du använda några riktigt coola systemtokens. Här är de.

>[!NOTE]
>
>Tidszonsinställningarna för kontot påverkar när tokens för datum och tid körs.

## system.date {#system-date}

The `{{system.date}}` token återger aktuellt datum vid körning på följande sätt: **8 aug 2013**

**Fungerar i:**

* [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} flödessteg
* [Intressant stund](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} flödessteg
* [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} flödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.time {#system-time}

The `{{system.time}}` token återger aktuell tid vid körning så här: **04:34 PM (GMT -0700)**

**Fungerar i:**

* [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} flödessteg
* [Intressant stund](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} flödessteg
* [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} flödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.dateTime {#system-datetime}

The `{{system.dateTime}}` token återger aktuellt datum och aktuell tid vid körning på följande sätt: **2013-08-08 16:36:13**

**Fungerar i:**

* [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} flödessteg
* [Intressant stund](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} flödessteg
* [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} flödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.forwardToFriendLink {#system-forwardtofriendlink}

The `{{system.forwardToFriendLink}}` kan du styra placeringen av [Vidarebefordra till en vänlänk i e-postmeddelanden](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Fungerar i:**

* [Lägg till en systemtoken som en länk i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} eller mall

## system.unsubscribeLink {#system-unsubscribelink}

The `{{system.unsubscribeLink}}` kan du styra placeringen av länken för att avbryta prenumerationen i ett e-postmeddelande.

**Fungerar i:**

* [Lägg till en systemtoken som en länk i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} eller mall

## system.viewAsWebpageLink {#system-viewaswebpagelink}

The `{{system.viewAsWebpageLink}}` kan du styra placeringen av länken Visa som webbsida i ett e-postmeddelande.

**Fungerar med:**

* [Lägg till en systemtoken som en länk i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} eller mall
