---
description: Logga samtalsorsaker och samtalsresultat för Salesforce - Marketo Docs - produktdokumentation
title: Logga samtalsorsaker och samtalsresultat till Salesforce
hide: true
hidefromtoc: true
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
source-git-commit: 0fc2551ffc85260a282b64995c698098846eb10c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Logga samtalsorsaker och samtalsresultat till Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Om du vill logga samtalsresultat och anropa orsaker till Salesforce för rapporterings- eller synlighetssyften kan du skapa ett anpassat aktivitetsfält för varje. Varje fält måste ha ett specifikt API-namn (kallas fältnamn i Salesforce).

* Namn på utdatafält för samtal: mktosales_call_result
* Fältnamn för samtalsorsaker: mktosales_call_reason

Om du vill använda dessa fält måste du först skapa fältet som ett anpassat aktivitetsfält. För att göra den synlig för användarna måste du lägga till den i sidolayouten för uppgiftsobjektet.

## Salesforce Classic {#salesforce-classic}

### Skapa anpassat aktivitetsfält i Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Skriv&quot;Aktiviteter&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Klicka **Anpassade aktivitetsfält**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Klicka **Nytt**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Markera datatypen &quot;Text&quot; och klicka på **Nästa**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Ge det anpassade fältet fältnamnet enligt definitionen ovan. Fältlängden får innehålla högst 255 tecken. Fältetiketten är det fält som är synligt för säljteamet och kan anpassas efter teamets behov.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Resten av inställningarna är valfria. När du är klar med konfigurationen klickar du på **Nästa**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Välj önskade säkerhetsinställningar på fältnivå för det här fältet och klicka på **Nästa** (bilden nedan är bara ett exempel).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Se till att det anpassade fältet är synligt för den profil som dina Sales Connect-användare använder, tillsammans med alla andra som du vill att det ska vara synligt.

1. Välj vilka sidlayouter du vill lägga till fältet i och klicka på **Spara** (du kan också klicka **Spara och ny** och upprepa processen för fältet Anropsorsak).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Lägg till anpassat aktivitetsfält till aktivitetssidlayout i Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Klicka **Sidlayout för aktivitet**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Klicka **Redigera** intill uppgiftssidans layout vill du lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Dra och släpp fältet till sidlayouten Uppgift.

   PICC

1. Klicka **Spara**.

   PICC

## Salesforce Lightning {#salesforce-lightning}

### Skapa anpassat aktivitetsfält i Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. I Salesforce klickar du på kugghjulsikonen längst upp till höger.

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

## Lägg till anpassat aktivitetsfält i aktivitetssidlayout i Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. I Salesforce klickar du på kugghjulsikonen längst upp till höger.

PICC

1. Klicka **Inställningar**.

PICC

1. Gå till Konfigurera????????????

PICC

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

PICC

1. Klicka på Aktivitet.

PICC

1. Klicka på Sidlayouter.

PICC

1. Klicka på Öppna den uppgiftssidlayout som du vill lägga till det här fältet i.

PICC

1. Dra och släpp fältet till sidlayouten Uppgift.

PICC

1. Klicka på Spara.

PICC

>[!MORELIKETHIS]
>
>[Installera händelsefält för försäljningsanslutning i aktivitetshistorik](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
