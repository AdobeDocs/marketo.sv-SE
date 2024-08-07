---
unique-page-id: 30082174
description: Intressanta ögonblick i Sales Connect - Marketo Docs - produktdokumentation
title: Intressanta stunder i Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 3a3287ed20962a052e0015161e34e33a95dd450a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Intressanta stunder i Sales Connect {#interesting-moments-in-sales-connect}

Intressanta ögonblick är nyckeln till att kommunicera med säljarna via Marketo Sales Connect.

>[!AVAILABILITY]
>
>Dessa är endast tillgängliga för [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md)- och Marketo Sales Connect-kunder.

>[!PREREQUISITES]
>
>* Du måste ha en [anslutning till Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Du måste vara lead- eller kontaktägare i Salesforce
>* Du måste ha åtkomst till [Bevilja åtkomst till anslutningen för Marketo Engage](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## Vad är ett intressant ögonblick? {#what-is-an-interesting-moment}

Det är upp till dig! Du bestämmer själv vilken information som är relevant för säljteamet. Säljteamet kanske vill veta när en lead:

* Besök prissidan på din webbplats
* Klicka på en länk i ett e-postmeddelande om en ny produkt
* Begär en produktdemo

## Hur skapar jag ett intressant ögonblick? {#how-do-i-create-an-interesting-moment}

1. Välj en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), helst en som ditt säljteam tycker är intressant om den aktiveras.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Dra över flödessteget **Intressanta stunder**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Välj en **typ** (e-post, milstolpe eller webb).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Skriv ett meddelande till ditt säljteam i fältet **Beskrivning** som förklarar varför den här åtgärden är viktig.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo lägger också till datumet som infaller och hur den intressanta stunden lades till (dvs lead-åtgärd > flödessteg, SOAP API).

## Hur ser ett intressant ögonblick ut i Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Intressanta stunder visas i aktivitetsloggen för en [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Hur ser en intressant stund ut i Sales Connect? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Intressanta ögonblick visas i realtid i en användares livefeed. Vi använder ID:t för lead-ägare i Salesforce för att visa användarnas intressanta ögonblick av relevanta leads som de är ägare av. Användare kan snabbt följa upp med leads via e-post/telefon/försäljningskampanj genom att klicka på listrutan bredvid leadets namn.

![](assets/engagement.jpg)
