---
unique-page-id: 42762409
description: Sales Insight Page for Marketo Admins - Marketo Docs - produktdokumentation
title: Sales Insight Page for Marketo Admins
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Sales Insight Page for Marketo Admins {#sales-insight-page-for-marketo-admins}

Marketo-administratörer har vissa privilegier i Sales Insight. Läs vad de är nedan.

## Konfiguration av Soap API {#soap-api-configuration}

De här inloggningsuppgifterna används för att ansluta ditt Salesforce-konto till din Marketo-instans för att använda MSI i Salesforce.

![](assets/one-1.png)

## Återstående API-konfiguration {#rest-api-configuration}

De här inloggningsuppgifterna används för att ansluta ditt Salesforce-konto till din Marketo-instans för att använda MSI Insights Dashboard i Salesforce.

![](assets/two-1.png)

Du kan välja att ta bort Rest API-autentiseringsuppgifter i SFDC och endast använda Soap API:er. Detta inaktiverar Insikt-instrumentpanelen

![](assets/three-1.png)

## Inställningar för personpoäng {#person-score-settings}

| **Stjärnor:** | Stjärnor representerar totalt antal leads jämfört med andra leads. |
|---|---|
| **Lågor:** | Lågor är brådskande - hur mycket en leads poäng har ändrats nyligen. |

Som standard använder Marketo Sales Insight fältet Lead Score för att beräkna stjärnor och lågor. Men om du vill välja ett annat fält, så här:

1. Klicka på **Sales Insight** under **Admin** i Marketo.

   ![](assets/four.png)

1. Klicka på **Redigera** under Inställningar för leadpoäng.

   ![](assets/five.png)

1. Markera det fält som du vill använda för stjärnor.

   ![](assets/six.png)

1. Markera det fält som du vill använda för lågor.

   ![](assets/seven.png)

1. Klicka på **Spara**. Försäljningsinsikter kan ta lite tid att omberäkna. Du kan kontrollera CRM senare för att se stjärnorna och lågor.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Om du inte redan har dina anpassade poängfält så här [skapar du dem](http://docs.marketo.com/x/3wMk).

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >
   >[Stjärnor och flamman](http://docs.marketo.com/x/qgU6Ag)

## Inställningar {#settings}

![](assets/nine.png)

**Avbeställ prenumerationsinställningar: **

Du kan välja bland följande inställningar för att avbryta prenumerationen för Ingen mall, Standardmeddelanden och operativa e-postmeddelanden

* Respektera inställningen för att avbryta prenumerationen
* Respektera inställningarna för att avbryta prenumerationen när fler än en mottagare
* Uppfyll inställningarna för att avbryta prenumerationen när fler än fem mottagare har
* Ignorera inställningar för att avbryta prenumerationen

**Möjlighet att låsa mallar: **

När det här alternativet är aktiverat kan MSI-användare inte redigera mallar när de skickar e-post från Salesforce

**Aktivera RSS-feed:**

När det här alternativet är aktiverat kan MSI-användare visa sin lead-feed i en RSS-feed (utöver lead-feed i Salesforce)**.**
