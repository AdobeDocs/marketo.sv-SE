---
description: Använda massutskick av e-post för försäljning i Salesforce - Marketo Docs - produktdokumentation
title: Använda massutskick av e-post för försäljning i Salesforce
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Använda massutskick av e-post för försäljning i Salesforce {#using-bulk-send-sales-email-in-salesforce}

Lär dig hur du skickar massutskick i Salesforce för att skala din utgående kommunikation med hjälp av försäljningsåtgärder.

>[!NOTE]
>
>Salesforce har en begränsning på 200 poster som kan väljas samtidigt.

>[!PREREQUISITES]
>
>Kontrollera att du har installerat [senaste Sales Insight-paketet](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} i dina kontakt- och leadlistor i Salesforce.

## Skicka massutskick via e-post i Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. I Salesforce navigerar du till hemsidan Leads/Kontakter genom att klicka på **Leads/kontakter** -fliken.

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. I listrutan Visa väljer du den vy med leads/kontakter som du vill skicka e-post till.

   >[!TIP]
   >
   >Du kan skapa en ny vy genom att klicka på kodikonen till höger och välja **Nytt**. När du har gett vyn ett nytt namn och sparat det kan du klicka på filterikonen till höger för att filtrera ner till den önskade uppsättningen leads/kontakter som du vill skicka med e-post.

1. Välj önskad lead- eller kontaktlista och klicka på **Skicka e-postmeddelande** -knappen.

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Du kommer att navigeras till fönstret för funktionsmakron med de personer du har valt tillagda.

1. Välj den mall som du vill infoga i redigeraren i åtgärdsdispositionsfönstret eller skriv ett eget e-postmeddelande.

   >[!TIP]
   >
   >Använd [Fasta kategorier](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} för att ge enklare åtkomst till dina e-postmallar.

   **VALFRITT STEG**: Förhandsgranska personalisering av dynamiska fält genom att klicka på **Förhandsgranska dynamiska fält** -knappen.

   >[!TIP]
   >
   >Om du vill anpassa en mall för alla mottagare kan du redigera alla mottagares e-postmeddelanden samtidigt genom att klicka på alternativet Alla mottagare i sidofältet Gruppera disposition. Om du vill ändra ett visst e-postmeddelande klickar du på mottagarens namn eller e-postadress i sidofältet Gruppera disposition. Observera att om du ändrar ett enskilt e-postmeddelande och sedan gör ändringar när du markerar Alla mottagare, kommer ändringarna som gjorts för Alla mottagare att skriva över ändringarna som gjorts för det enskilda e-postmeddelandet.

1. Välj **Skicka** att skicka e-postmeddelandet omedelbart, eller **Ange schema** för att ange ett datum och en tid för när e-postmeddelandet ska skickas.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Skicka massutskick i Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. I Salesforce klickar du på **Leads/kontakter** -fliken.

1. I listrutan Visa väljer du önskad vy med leads/kontakter som du vill skicka e-post till och klickar på **Gå**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Du kan skapa en ny vy genom att klicka på Skapa ny vy och konfigurera de tillgängliga filtren för att begränsa listan över vilka du lägger till i en försäljningskampanj.

1. Välj önskade leads eller kontaktlistor och klicka på **Skicka e-postmeddelande** -knappen.

1. Du kommer att navigeras till fönstret Åtgärder och disposition med de mottagare som du har valt i dispositionsfönstret.

1. Välj den mall som du vill infoga i redigeraren för åtgärdsdispositionsfönstret eller skriv ett eget e-postmeddelande.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Använd [Fasta kategorier](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} för att ge enklare åtkomst till dina e-postmallar.

   **VALFRITT STEG**: Förhandsgranska personalisering av dynamiska fält genom att klicka på **Förhandsgranska dynamiska fält** -knappen.

   >[!TIP]
   >
   >Om du vill anpassa en mall för alla mottagare kan du redigera alla mottagares e-postmeddelanden samtidigt genom att klicka på alternativet Alla mottagare i sidofältet Gruppera disposition. Om du vill ändra ett visst e-postmeddelande klickar du på mottagarens namn eller e-postadress i sidofältet Gruppera disposition. Observera att om du ändrar ett enskilt e-postmeddelande och sedan gör ändringar när du markerar Alla mottagare, kommer ändringarna som gjorts för Alla mottagare att skriva över ändringarna som gjorts för det enskilda e-postmeddelandet.

1. Välj **Skicka** att skicka e-postmeddelandet omedelbart, eller **Ange schema** för att ange ett datum och en tid för när e-postmeddelandet ska skickas.
