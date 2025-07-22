---
unique-page-id: 30082174
description: Intressanta ögonblick i Sales Connect - Marketo Docs - produktdokumentation
title: Intressanta stunder i Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Intressanta stunder i [!DNL Sales Connect] {#interesting-moments-in-sales-connect}

Intressanta stunder är nyckeln till att kommunicera med ditt säljteam via [!DNL Marketo Sales Connect].

>[!AVAILABILITY]
>
>Dessa är endast tillgängliga för [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md)- och [!DNL Marketo Sales Connect]-kunder.

>[!PREREQUISITES]
>
>* Du måste ha en [anslutning till Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Du måste vara lead- eller kontaktägare i Salesforce
>* Du måste ha åtkomst till [Bevilja åtkomst till Marketo Engage-anslutningen](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## Vad är ett intressant ögonblick? {#what-is-an-interesting-moment}

Det är upp till dig! Du bestämmer själv vilken information som är relevant för säljteamet. Säljteamet kanske vill veta när en lead:

* Besök prissidan på din webbplats
* Klicka på en länk i ett e-postmeddelande om en ny produkt
* Begär en produktdemo

## Hur skapar jag ett intressant ögonblick? {#how-do-i-create-an-interesting-moment}

1. Välj en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), helst en som ditt säljteam tycker är intressant om den aktiveras.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Dra över flödessteget **[!UICONTROL Interesting Moments]**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Välj en **typ** ([!UICONTROL Email], [!UICONTROL Milestone] eller [!UICONTROL Web]).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Skriv ett meddelande till ditt säljteam i fältet **[!UICONTROL Description]** som förklarar varför den här åtgärden är viktig.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo lägger också till datumet som infaller och hur den intressanta stunden lades till (dvs lead action > flow step, SOAP API).

## Hur ser ett intressant ögonblick ut i Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Intressanta stunder visas i aktivitetsloggen för en [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Hur ser en intressant stund ut i [!DNL Sales Connect]? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Intressanta ögonblick visas i realtid i en användares livefeed. Vi använder ID:t för lead-ägare i [!DNL Salesforce] för att visa användarnas intressanta ögonblick av relevanta leads som de är ägare av. Användare kan snabbt följa upp med leads via e-post/telefon/försäljningskampanj genom att klicka på listrutan bredvid leadets namn.

![](assets/engagement.jpg)
