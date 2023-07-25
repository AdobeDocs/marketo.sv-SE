---
unique-page-id: 42762519
description: Konfiguration för befintliga kunder - Marketo Docs - produktdokumentation
title: Konfiguration för befintliga kunder
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Konfiguration för befintliga kunder {#configuration-for-existing-customers}

Ställ in följande konfiguration för att börja använda den nya instrumentpanelen för Insights.

>[!PREREQUISITES]
>
>Kontrollera att du har uppgraderat ditt Salesforce-paket till den senaste versionen

## Konfigurera Sales Insight i Marketo {#configure-sales-insight-in-marketo}

1. Öppna en ny flik i webbläsaren och hämta Marketo Sales Insights-autentiseringsuppgifterna från ditt Marketo-konto.

1. Gå till **Administratör** område.

   ![](assets/configuration-for-existing-customers-1.png)

1. Klicka **Försäljningsinsikter**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Klicka **Visa** för att fylla i Rest API-autentiseringsuppgifter.

   ![](assets/configuration-for-existing-customers-3.png)

1. Ett bekräftelsemeddelande visas. Klicka **OK**.

## Konfigurera säljinsikter i Salesforce {#configure-sales-insight-in-salesforce}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Sök efter och markera **Inställningar för fjärrplats**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Ange fjärrwebbplatsnamnet (det kan vara något som MarketoRestAPI) och URL:en för fjärrplatsen (din API-URL från konfigurationspanelen för Rest API i Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Klicka **Spara**.

   ![](assets/configuration-for-existing-customers-8.png)

   Du har nu skapat fjärrplatsinställningar för Rest API.

## Öppna Marketo Sales Insight {#access-marketo-sales-insight}

1. Kopiera inloggningsuppgifterna från panelen Rest API på Marketo Sales Insight Admin-sida. Klistra in dem i avsnittet Rest API på Salesforce konfigurationssida Sales Insight.

1. Ange API-hemlig nyckel.

   ![](assets/configuration-for-existing-customers-9.png)
