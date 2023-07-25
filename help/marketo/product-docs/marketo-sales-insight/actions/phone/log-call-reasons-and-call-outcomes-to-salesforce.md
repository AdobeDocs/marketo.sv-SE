---
description: Logga samtalsorsaker och samtalsresultat för Salesforce - Marketo Docs - produktdokumentation
title: Logga samtalsorsaker och samtalsresultat till Salesforce
exl-id: cfe71388-282b-45e5-a817-45a951f613bc
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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

1. I Salesforce klickar du på **Inställningar**.

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
   >Se till att det anpassade fältet är synligt för den profil som dina användare av Sales Insight Actions använder, tillsammans med alla andra du vill att det ska vara synligt.

1. Välj vilka sidlayouter du vill lägga till fältet i och klicka på **Spara** (du kan också klicka **Spara och ny** och upprepa processen för fältet Anropsorsak).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Lägg till anpassat aktivitetsfält till aktivitetssidlayout i Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Du behöver bara följa dessa steg om du inte har valt önskad sidlayout i steg 9 ovan.

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Klicka **Sidlayout för aktivitet**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Klicka **Redigera** intill uppgiftssidans layout vill du lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Klicka **Spara**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Skapa anpassat aktivitetsfält i Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Klicka på kugghjulsikonen uppe till höger i Salesforce och välj **Inställningar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Klicka **Objektshanteraren**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Skriv&quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Klicka på **Aktivitet** label.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Klicka **Fält och relationer**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Klicka **Nytt**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Lägg till anpassat aktivitetsfält i aktivitetssidlayout i Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Klicka på kugghjulsikonen uppe till höger i Salesforce och välj **Inställningar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Klicka **Objektshanteraren**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Klicka på **Uppgift** label.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Klicka **Sidlayouter**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Klicka på Öppna den uppgiftssidlayout som du vill lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Klicka **Spara**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [Utfall för samtal](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [Samtalsorsaker](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)
