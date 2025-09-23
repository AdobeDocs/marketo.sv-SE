---
description: Log Call Reasons and Call Outcome to Salesforce - Marketo Docs - Product Documentation
title: Logga samtalsorsaker och samtalsresultat för Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 2%

---

# Logga samtalsorsaker och samtalsresultat till [!DNL Salesforce] {#log-call-reasons-and-call-outcomes-to-salesforce}

Om du vill logga samtalsresultat och anropa orsaker till [!DNL Salesforce] i rapporterings- eller synlighetssyfte kan du skapa ett anpassat aktivitetsfält för varje. Varje fält måste ha ett specifikt API-namn (kallas fältnamn i [!DNL Salesforce]).

* Namn på utdatafält för anrop: mktosales_call_result
* Fältnamn för anropsorsaker: mktosales_call_reason

Om du vill använda dessa fält måste du först skapa fältet som ett anpassat aktivitetsfält. För att göra den synlig för användarna måste du lägga till den i sidolayouten för uppgiftsobjektet.

## [!DNL Salesforce] Classic {#salesforce-classic}

### Skapa anpassat aktivitetsfält i [!DNL Salesforce] Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Klicka på [!DNL Salesforce] i **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Skriv&quot;Aktiviteter&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Klicka på **[!UICONTROL Activity Custom Fields]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Markera datatypen [!UICONTROL Text] och klicka på **[!UICONTROL Next]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Ge det anpassade fältet fältnamnet enligt definitionen ovan. Fältlängden får innehålla högst 255 tecken. Fältetiketten är det fält som är synligt för säljteamet och kan anpassas efter teamets behov.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Resten av inställningarna är valfria. När du har slutfört konfigurationen klickar du på **[!UICONTROL Next]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Välj önskade säkerhetsinställningar på fältnivå för det här fältet och klicka på **[!UICONTROL Next]** (bilden nedan är bara ett exempel).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Kontrollera att det anpassade fältet är synligt för den profil som dina [!DNL Sales Connect]-användare använder, tillsammans med alla andra som du vill att det ska vara synligt.

1. Välj vilka sidlayouter du vill lägga till fältet i och klicka på **[!UICONTROL Save]** (du kan också klicka på **[!UICONTROL Save & New]** och upprepa processen för fältet Anropsorsak).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Lägg till anpassat aktivitetsfält i aktivitetssidlayouten i [!DNL Salesforce] Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Du behöver bara följa dessa steg om du inte har valt önskad sidlayout i steg 9 ovan.

1. Klicka på [!DNL Salesforce] i **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Skriv &quot;Aktivitet&quot; i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Klicka på **[!UICONTROL Task Page Layouts]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Klicka på **[!UICONTROL Edit]** bredvid den uppgiftssidlayout du vill lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce] Lightning {#salesforce-lightning}

### Skapa anpassat aktivitetsfält i [!DNL Salesforce] Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. I [!DNL Salesforce] klickar du på kugghjulsikonen uppe till höger och väljer **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Klicka på **[!UICONTROL Object Manager]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Skriv [!UICONTROL Activity] i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Klicka på etiketten **[!UICONTROL Activity]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Klicka på **[!UICONTROL Fields & Relationships]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Lägg till anpassat aktivitetsfält i aktivitetssidlayout i [!DNL Salesforce] Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. I [!DNL Salesforce] klickar du på kugghjulsikonen uppe till höger och väljer **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Klicka på **[!UICONTROL Object Manager]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Skriv [!UICONTROL Task] i rutan Snabbsökning.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Klicka på etiketten **[!UICONTROL Task]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Klicka på **[!UICONTROL Page Layouts]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Klicka på den uppgiftssidlayout som du vill lägga till det här fältet i.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Dra och släpp fältet till önskat avsnitt på sidan Uppgift.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Installera händelserefält för anslutning av försäljning på aktivitetshistorik](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
