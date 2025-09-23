---
unique-page-id: 2360301
description: Ange poängfält som ska användas för staplar och flamma i Sales Insight - Marketo Docs - produktdokumentation
title: Ange poängfält som ska användas för staplar och flamma i Sales Insight
exl-id: 640f6d53-71ee-4a6d-b28a-82f3825b8f8e
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Ange poängfält som ska användas för [!UICONTROL Stars] och [!UICONTROL Flames] i [!DNL Sales Insight] {#set-score-fields-to-be-used-for-stars-and-flames-in-sales-insight}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Som standard använder [!DNL Marketo Sales Insight] fältet **[!UICONTROL Lead Score]** för att beräkna stjärnor och lågor. Men om du vill välja ett annat fält, så här:

>[!TIP]
>
>Om du inte redan har dina anpassade poängfält, så här [skapar](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) dem.

>[!NOTE]
>
>**Definition**
>
>* **[!UICONTROL Stars]**: Stjärnor representerar det totala antalet leads jämfört med andra leads.
>* **[!UICONTROL Flames]**: Lågor representerar ett brådskande ärende - hur mycket ett leadets poäng har ändrats nyligen.
>

1. Klicka på **[!UICONTROL Admin]** under **[!UICONTROL Sales Insight]**.

   ![](assets/image2014-9-16-13-3a27-3a19.png)

1. Klicka på **[!UICONTROL Lead Scoring Settings]** under **[!UICONTROL Edit]**.

   ![](assets/image2014-9-16-13-3a27-3a33.png)

1. Markera fältet som du vill använda för **[!UICONTROL Stars]**.

   ![](assets/image2014-9-16-13-3a27-3a45.png)

1. Markera fältet som du vill använda för **[!UICONTROL Flames]**.

   ![](assets/image2014-9-16-13-3a28-3a1.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-16-13-3a28-3a18.png)

   >[!NOTE]
   >
   >[!DNL Sales insight] tar lite tid att omberäkna. Du kan kontrollera CRM senare för att se stjärnorna och lågor.

   >[!MORELIKETHIS]
   >
   >[Prioritet, brådskande, Relativ poäng och Bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
