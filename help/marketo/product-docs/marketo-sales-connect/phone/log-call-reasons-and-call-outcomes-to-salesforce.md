---
description: Logga samtalsorsaker och samtalsresultat för Salesforce - Marketo Docs - produktdokumentation
title: Logga samtalsorsaker och samtalsresultat till Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Logga samtalsorsaker och samtalsresultat till Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Om du vill logga samtalsresultat och anropa orsaker till Salesforce för rapporterings- eller synlighetssyften kan du skapa ett anpassat aktivitetsfält för varje. Varje fält måste ha ett specifikt API-namn.

* API-namn för utanrop: mktosales_call_result
* Namn på API för anropsorsaker: mktosales_call_reason

Om du vill använda dessa fält måste du först skapa fältet som ett anpassat aktivitetsfält. För att göra den synlig för användarna måste du lägga till den i sidolayouten för uppgiftsobjektet.

## Skapa anpassat aktivitetsfält i Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Gå till Konfigurera i Salesforce.

PICC

1. Ange&quot;Aktiviteter&quot; i rutan Snabbsökning.

PICC

1. Klicka **Anpassade aktivitetsfält**.

PICC

1. Klicka **Nytt**.

PICC

## Skapa anpassat aktivitetsfält i Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Klicka på kugghjulsikonen uppe till höger i Salesforce.

PICC

1. Klicka **Inställningar**.

PICC

1. Klicka **Objektshanteraren**.

PICC

1. Ange Aktivitet i rutan Snabbsökning och klicka på aktivitetsetiketten för att öppna objektets inställningar.

PICC

1. Klicka på till vänster **Fält och relationer**.

PICC

1. Klicka **Nytt**.

PICC

## Lägg till anpassat aktivitetsfält till aktivitetssidlayout i Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

STEG

## Lägg till anpassat aktivitetsfält i aktivitetssidlayout i Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

STEG

>[!MORELIKETHIS]
>
>[Installera händelsefält för försäljningsanslutning i aktivitetshistorik](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
