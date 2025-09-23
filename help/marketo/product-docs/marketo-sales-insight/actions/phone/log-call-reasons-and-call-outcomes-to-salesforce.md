---
description: Log Call Reasons and Call Outcome to Salesforce - Marketo Docs - Product Documentation
title: Logga samtalsorsaker och samtalsresultat för Salesforce
exl-id: cfe71388-282b-45e5-a817-45a951f613bc
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Logga samtalsorsaker och samtalsresultat för Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Om du vill logga samtalsresultat och ringa skäl till Salesforce för rapportering eller synlighet kan du skapa ett anpassat aktivitetsfält för varje. Varje fält måste ha ett specifikt API-namn (kallas fältnamn i Salesforce).

* Namn på utdatafält för anrop: mktosales_call_result
* Fältnamn för anropsorsaker: mktosales_call_reason

Om du vill använda dessa fält måste du först skapa fältet som ett anpassat aktivitetsfält. För att göra den synlig för användarna måste du lägga till den i sidolayouten för uppgiftsobjektet.

## Salesforce Classic {#salesforce-classic}

### Skapa fält för anpassad aktivitet i Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Klicka på **Konfigurera** i Salesforce.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Skriv&quot;Aktiviteter&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Klicka på **Anpassade aktivitetsfält**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Klicka på **Ny**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Markera datatypen &quot;Text&quot; och klicka på **Nästa**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Ge det anpassade fältet fältnamnet enligt definitionen ovan. Fältlängden får innehålla högst 255 tecken. Fältetiketten är det fält som är synligt för säljteamet och kan anpassas efter teamets behov.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Resten av inställningarna är valfria. När du har slutfört konfigurationen klickar du på **Nästa**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Välj önskade säkerhetsinställningar på fältnivå för det här fältet och klicka på **Nästa** (bilden nedan är bara ett exempel).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Se till att det anpassade fältet är synligt för den profil som dina användare av Sales Insight Actions använder, tillsammans med alla andra du vill att det ska vara synligt.

1. Välj vilka sidlayouter du vill lägga till fältet i och klicka på **Spara** (du kan också klicka på **Spara och ny** och upprepa processen för fältet Anropsorsak).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Lägg till anpassat aktivitetsfält i aktivitetssidlayouten i Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Du behöver bara följa dessa steg om du inte har valt önskad sidlayout i steg 9 ovan.

1. Klicka på **Konfigurera** i Salesforce.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Klicka på **Sidlayouter för åtgärder**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Klicka på **Redigera** bredvid den uppgiftssidlayout du vill lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Klicka på **Spara**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Skapa anpassat aktivitetsfält i Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. I Salesforce klickar du på kugghjulsikonen längst upp till höger och väljer **Konfigurera**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Klicka på **Objektshanteraren**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Skriv&quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Klicka på etiketten **Aktivitet**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Klicka på **Fält och relationer**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Klicka på **Ny**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Lägg till anpassat aktivitetsfält i uppgiftssidlayouten i Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. I Salesforce klickar du på kugghjulsikonen längst upp till höger och väljer **Konfigurera**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Klicka på **Objektshanteraren**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Klicka på etiketten **Aktivitet**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Klicka på **Sidlayouter**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Klicka på Öppna den uppgiftssidlayout som du vill lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Klicka på **Spara**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [Utfall för samtal](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [Anropa orsaker](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)
