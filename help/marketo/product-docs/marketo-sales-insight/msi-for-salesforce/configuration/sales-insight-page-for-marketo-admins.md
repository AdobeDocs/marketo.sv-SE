---
unique-page-id: 42762409
description: Sales Insight Page for Marketo Admins - Marketo Docs - produktdokumentation
title: Sales Insight Page for Marketo Admins
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# [!DNL Sales Insight]-sida för Marketo-administratörer {#sales-insight-page-for-marketo-admins}

Marketo-administratörer har vissa behörigheter i [!DNL Sales Insight]. Läs vad de är nedan.

## Konfiguration av Soap API {#soap-api-configuration}

Dessa autentiseringsuppgifter används för att ansluta ditt [!DNL Salesforce]-konto till din Marketo-instans för att kunna använda MSI i [!DNL Salesforce].

![](assets/one-1.png)

## Återstående API-konfiguration {#rest-api-configuration}

De här autentiseringsuppgifterna används för att ansluta ditt [!DNL Salesforce]-konto till din Marketo-instans för att kunna använda MSI Insights Dashboard i [!DNL Salesforce].

![](assets/two-1.png)

## Inställningar för personpoäng {#person-score-settings}

* **[!UICONTROL Stars]**: Stjärnor representerar totalt antal leads jämfört med andra leads.
* **[!UICONTROL Flames]**: Flammen är brådskande - hur mycket ett leads poäng har ändrats nyligen.

Som standard använder [!DNL Marketo Sales Insight] fältet Leadpoäng för att beräkna stjärnor och lågor. Men om du vill välja ett annat fält, så här:

1. Klicka på **[!UICONTROL Admin]** i området **[!UICONTROL Sales Insight]** i Marketo.

   ![](assets/four.png)

1. Klicka på [!UICONTROL Lead Scoring Settings] under **[!UICONTROL Edit]**.

   ![](assets/five.png)

1. Markera det fält som du vill använda för stjärnor.

   ![](assets/six.png)

1. Markera det fält som du vill använda för lågor.

   ![](assets/seven.png)

1. Klicka på **[!UICONTROL Save]**. Försäljningsinsikter kan ta lite tid att omberäkna. Du kan kontrollera CRM senare för att se stjärnorna och lågor.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Om du inte redan har dina anpassade poängfält gör du så här för att [skapa dem](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Stjärnor och flamma](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Inställningar {#settings}

![](assets/nine.png)

**Inställningar för att avbryta prenumerationen:**

Du kan välja bland följande inställningar för att avbryta prenumerationen för [!UICONTROL No Template], [!UICONTROL Standard Emails] &amp; [!UICONTROL Operational emails]

* [!UICONTROL Respect Unsubscribe Setting]
* [!UICONTROL Respect Unsubscribe Settings when more than 1 recipient]
* [!UICONTROL Respect Unsubscribe Settings when more than 5 recipients]
* [!UICONTROL Ignore Unsubscribe Settings]

**Aktivera möjligheten att låsa mallar:**

När det här alternativet är aktiverat kan MSI-användare inte redigera mallar när de skickar e-post från [!DNL Salesforce]

**Aktivera RSS-feed:**

När det här alternativet är aktiverat kan MSI-användare visa sin lead-feed i en RSS-feed (utöver lead-feed i [!DNL Salesforce]). RSS-feed fungerar bara om funktionen [!UICONTROL Token Expiration] är inaktiverad.

**Giltig token:**

Förfallotid för token styrs i Funktionshanteraren. Om du vill aktivera/inaktivera den kan du kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support). När det här alternativet är aktiverat upphör alla Marketo-tokens att gälla inom 10 minuter. När funktionen är inaktiverad upphör inte Marketo-tokens att gälla.

Token som genererats innan Token Expiration aktiverades har ingen förfallotid att validera mot, så de upphör inte att gälla även om funktionen är aktiverad.

Token som genereras efter att Token Expiration aktiverats har en förfallotid på 10 minuter, så de går fortfarande ut om 10 minuter även efter att funktionen har inaktiverats.

Tokenbeteendet baseras på när det genererades (när funktionen för förfallodatum för token aktiverades/inaktiverades, i stället för på dess nuvarande funktionsstatus).
