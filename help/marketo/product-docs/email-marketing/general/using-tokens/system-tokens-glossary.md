---
unique-page-id: 1147344
description: System Tokens Glossary - Marketo Docs - Produktdokumentation
title: Ordlista för systemtoken
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
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

`{{system.date}}`-token kommer att återge aktuellt datum vid körning så här: **8 aug 2013**

**Fungerar i:**

* [Ändra ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) datavärdessteg
* [Intressant ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) steg för Momentflow
* [Skapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) uppgiftsflödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.time {#system-time}

Token `{{system.time}}` återger aktuell tid vid körning så här: **04:34 PM (GMT -0700)**

**Fungerar i:**

* [Ändra ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) datavärdessteg
* [Intressant ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) steg för Momentflow
* [Skapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) uppgiftsflödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.dateTime {#system-datetime}

Token `{{system.dateTime}}` återger aktuellt datum och aktuell tid vid körning så här: **2013-08-08 16:36:13**

**Fungerar i:**

* [Ändra ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) datavärdessteg
* [Intressant ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) steg för Momentflow
* [Skapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) uppgiftsflödessteg
* Innehållet i ett e-postmeddelande eller en mall

## system.forwardToFriendLink {#system-forwardtofriendlink}

Med `{{system.forwardToFriendLink}}`-token kan du styra placeringen av [&#39;Forward to a Friend Link&#39; i e-postmeddelanden](../../../../product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md).

**Fungerar i:**

* [Lägg till en systemtoken som en länk i en ](add-a-system-token-as-a-link-in-an-email.md) e-postmall

## system.unsubscribeLink {#system-unsubscribelink}

Med `{{system.unsubscribLink}}`-token kan du styra placeringen av länken för att avbryta prenumerationen i ett e-postmeddelande.

**Fungerar i:**

* [Lägg till en systemtoken som en länk i en ](add-a-system-token-as-a-link-in-an-email.md) e-postmall

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Med `{{system.viewAsWebpageLink}}`-token kan du styra placeringen av länken Visa som webbsida i ett e-postmeddelande.

**Fungerar med:**

* [Lägg till en systemtoken som en länk i en ](add-a-system-token-as-a-link-in-an-email.md) e-postmall
