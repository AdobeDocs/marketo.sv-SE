---
unique-page-id: 2951640
description: Använda intressanta stunder - Marketo Docs - Produktdokumentation
title: Använda intressanta stunder
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Använda intressanta stunder {#using-interesting-moments}

Intressanta ögonblick är nyckeln till att kommunicera med säljarna via Marketo Sales Insight-appen.

>[!AVAILABILITY]
>
>Dessa är endast tillgängliga för kunder som har Marketo Sales Insight och [Marketo Sales Connect](http://docs.marketo.com/x/fgTLAQ) .

## Vad är ett intressant ögonblick?  {#what-is-an-interesting-moment}

Det är upp till dig! Du bestämmer själv vilken information som är relevant för säljteamet. Säljteamet kanske vill veta när en lead:

* Besök prissidan på din webbplats
* Klicka på en länk i ett e-postmeddelande om en ny produkt
* Begär en produktdemo

## Hur skapar jag ett intressant ögonblick?  {#how-do-i-create-an-interesting-moment}

1. Välj en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), helst en som säljteamet skulle finna intressant om det utlöstes.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Dra över flödessteget **Intressanta** stunder.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Välj en **typ** (E-post, Milstolpe eller Webb).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Skriv ett meddelande till ditt säljteam i fältet **Beskrivning** som förklarar varför den här åtgärden är viktig.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo lägger också till datumet det inträffade och hur det intressanta ögonblicket lades till (dvs lead action > flow step, SOAP API).

## Hur kan det här bli ännu intressantare?  {#how-can-this-get-even-more-interesting}

Tokens! Lägg till dem i beskrivningsfältet för att ge säljteamet mer specifik information, som ämnesraden i det e-postmeddelande som leadet öppnade eller vem som skickade det. Ta reda på vilka variabler som är tillgängliga för användning i ordlistan [Tokens for Intresse Moments](tokens-for-interesting-moments.md) .

>[!TIP]
>
>Börja med fem intressanta ögonblick och samarbeta sedan med säljarna för att ta reda på vilken information de är intresserade av att se.

## Hur ser ett intressant ögonblick ut i Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Intressanta stunder visas i en [leads aktivitetslogg](../../../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Hur ser ett intressant ögonblick ut i Salesforce?  {#what-does-an-interesting-moment-look-like-in-salesforce}

När du har [installerat Marketo Sales Insight App](../../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)visas intressanta stunder på lead-, kontakt-, konto- eller affärsmöjlighetssidorna. De visas också på kontrollpanelen Sales Insight i Lead Feed, Best Bets och Watch List.

![](assets/six.png)

## Hur ser ett intressant ögonblick ut i Salesforce1? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

När du har installerat eller uppdaterat Marketo Sales Insight för Salesforce1 visas intressanta stunder under leadets relaterade länkar.

![](assets/seven.png)
