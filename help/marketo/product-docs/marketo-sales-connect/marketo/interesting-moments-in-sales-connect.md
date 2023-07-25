---
unique-page-id: 30082174
description: Intressanta ögonblick i Sales Connect - Marketo Docs - produktdokumentation
title: Intressanta stunder i Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Intressanta stunder i Sales Connect {#interesting-moments-in-sales-connect}

Intressanta ögonblick är nyckeln till att kommunicera med säljarna via Marketo Sales Connect.

>[!AVAILABILITY]
>
>Dessa är tillgängliga för [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) och endast Marketo Sales Connect-kunder.

## Vad är ett intressant ögonblick? {#what-is-an-interesting-moment}

Det är upp till dig! Du bestämmer själv vilken information som är relevant för säljteamet. Säljteamet kanske vill veta när en lead:

* Besök prissidan på din webbplats
* Klicka på en länk i ett e-postmeddelande om en ny produkt
* Begär en produktdemo

## Hur skapar jag ett intressant ögonblick? {#how-do-i-create-an-interesting-moment}

1. Välj en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), helst en som ditt säljteam tycker är intressant om det utlöses.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Dra över **Intressanta ögonblick** flödessteg.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Välj en **type** (E-post, Milstolpe eller Webb).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Skriv ett meddelande till ditt säljteam i **Beskrivning** fält som förklarar varför den här åtgärden är viktig.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo lägger också till datumet det inträffade och hur det intressanta ögonblicket lades till (dvs lead action > flow step, SOAP API).

## Hur ser ett intressant ögonblick ut i Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Intressanta stunder visas i en [Lead-aktivitetsloggen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Hur ser en intressant stund ut i Sales Connect? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Intressanta ögonblick visas i realtid i en användares livefeed. Vi använder ID:t för lead-ägare i Salesforce för att visa användarnas intressanta ögonblick av relevanta leads som de är ägare av. Användare kan snabbt följa upp med leads via e-post/telefon/försäljningskampanj genom att klicka på listrutan bredvid leadets namn.

![](assets/engagement.jpg)
