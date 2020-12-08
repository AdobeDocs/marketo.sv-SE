---
unique-page-id: 42762519
description: Konfiguration för befintliga kunder - Marketo Docs - Produktdokumentation
title: Konfiguration för befintliga kunder
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Konfiguration för befintliga kunder {#configuration-for-existing-customers}

Ställ in följande konfiguration för att börja använda den nya instrumentpanelen för Insights.

>[!NOTE]
>
>**Förutsättningar**
>
>Kontrollera att du har uppgraderat ditt Salesforce-paket till den senaste versionen

## Konfigurera Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Öppna en ny flik i webbläsaren för att hämta Marketo Sales Insights-autentiseringsuppgifterna från ditt Marketo-konto.
1. Gå till området **Admin** .

   ![](assets/configure-1.png)

1. Klicka på **Sales Insight**.

   ![](assets/configure-2.png)

1. Klicka på **Visa** för att fylla i Rest API-autentiseringsuppgifter.

   ![](assets/configure-3.png)

1. Ett bekräftelsemeddelande visas. Klicka på **OK**.

## Konfigurera säljinsikter i Salesforce {#configure-sales-insight-in-salesforce}

1. Klicka på **Konfigurera** i Salesforce.

   ![](assets/sfdc-1.png)

1. Sök efter och välj **Fjärrplatsinställningar**.

   ![](assets/sfdc-2.png)

1. Klicka på **Ny fjärrplats**.

   ![](assets/sfdc-3.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoRestAPI&quot;) och URL:en för fjärrplatsen (din API-URL från panelen för konfiguration av Rest API i Marketo).

   ![](assets/sfdc-4.png)

1. Klicka på **Spara**.

   ![](assets/sfdc-5.png)

   Du har nu skapat fjärrplatsinställningar för Rest API.

## Access Marketo Sales Insight {#access-marketo-sales-insight}

1. Kopiera inloggningsuppgifterna från panelen Rest API på Marketos Sales Insight Admin-sida. Klistra in dem i avsnittet Rest API på Salesforce konfigurationssida Sales Insight.
1. Ange API-hemlig nyckel.

   ![](assets/config.png)

