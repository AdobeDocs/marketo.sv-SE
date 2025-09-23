---
unique-page-id: 42762519
description: Konfiguration för befintliga kunder - Marketo Docs - produktdokumentation
title: Konfiguration för befintliga kunder
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# Konfiguration för befintliga kunder {#configuration-for-existing-customers}

Ställ in följande konfiguration för att börja använda den nya instrumentpanelen för Insights.

>[!PREREQUISITES]
>
>Kontrollera att du har uppgraderat ditt [!DNL Salesforce]-paket till den senaste versionen

## Konfigurera [!DNL Sales Insight] i Marketo {#configure-sales-insight-in-marketo}

1. Öppna en ny flik i webbläsaren för att hämta inloggningsuppgifterna för [!DNL Marketo Sales Insights] från ditt Marketo-konto.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Klicka på **[!UICONTROL Sales Insight]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Klicka på **[!UICONTROL View]** för att fylla i Rest API-autentiseringsuppgifter.

   ![](assets/configuration-for-existing-customers-3.png)

1. En bekräftelse visas. Klicka på **[!UICONTROL OK]**.

## Konfigurera [!DNL Sales Insight] i [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Klicka på **[!UICONTROL Setup]** i Salesforce.

   ![](assets/configuration-for-existing-customers-4.png)

1. Sök efter och välj **[!UICONTROL Remote Site Settings]**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Klicka på **[!UICONTROL New Remote Site]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Ange [!UICONTROL Remote Site Name] (det kan vara något som MarketoRestAPI) och [!UICONTROL Remote Site URL] (din API-URL från Rest API Configuration-panelen i Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/configuration-for-existing-customers-8.png)

   Du har nu skapat fjärrplatsinställningar för Rest API.

## Öppna Marketo Sales Insight {#access-marketo-sales-insight}

1. Kopiera inloggningsuppgifterna från panelen Rest API på administratörssidan för [!DNL Marketo’s Sales Insight]. Klistra in dem i avsnittet Rest API på Salesforce [!DNL Sales Insight]-konfigurationssida.

1. Ange [!UICONTROL API Secret Key].

   ![](assets/configuration-for-existing-customers-9.png)
