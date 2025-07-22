---
unique-page-id: 2951640
description: Använda intressanta stunder - Marketo Docs - produktdokumentation
title: Använda intressanta stunder
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Använda intressanta stunder {#using-interesting-moments}

Intressanta ögonblick är nyckeln till att kommunicera med ditt säljteam via appen [!DNL Marketo Sales Insight].

>[!AVAILABILITY]
>
>Dessa är endast tillgängliga för [!DNL Marketo Sales Insight]- och [[!DNL Marketo Sales Connect]](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md)-kunder.

## Vad är ett intressant ögonblick? {#what-is-an-interesting-moment}

Det är upp till dig! Du bestämmer själv vilken information som är relevant för säljteamet. Säljteamet kanske vill veta när en lead:

* Besök prissidan på din webbplats
* Klicka på en länk i ett e-postmeddelande om en ny produkt
* Begär en produktdemo

## Hur skapar jag ett intressant ögonblick?  {#how-do-i-create-an-interesting-moment}

1. Välj en [smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), helst en som ditt säljteam tycker är intressant om den aktiveras.

   ![](assets/using-interesting-moments-1.png)

1. Dra över flödessteget **[!UICONTROL Interesting Moments]**.

   ![](assets/using-interesting-moments-2.png)

1. Välj en **typ** ([!UICONTROL Email], [!UICONTROL Milestone] eller [!UICONTROL Web]).

   ![](assets/using-interesting-moments-3.png)

1. Skriv ett meddelande till ditt säljteam i fältet **[!UICONTROL Description]** som förklarar varför den här åtgärden är viktig.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo lägger också till datumet som infaller och hur den intressanta stunden lades till (dvs lead action > flow step, SOAP API).

## Hur kan det här bli ännu intressantare?  {#how-can-this-get-even-more-interesting}

Tokens! Lägg till dem i beskrivningsfältet för att ge säljteamet mer specifik information, som ämnesraden i det e-postmeddelande som leadet öppnade eller vem som skickade det. Ta reda på vilka tokens som är tillgängliga för användning i ordlistan [Tokens för intressanta stunder](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md).

>[!TIP]
>
>Börja med fem intressanta ögonblick och samarbeta sedan med säljarna för att ta reda på vilken information de är intresserade av att se.

## Hur ser ett intressant ögonblick ut i Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Intressanta stunder visas i aktivitetsloggen för en [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## Hur ser en intressant stund ut i [!DNL Salesforce]?  {#what-does-an-interesting-moment-look-like-in-salesforce}

När du har [installerat [!DNL Marketo Sales Insight] appen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) visas intressanta stunder på lead-, kontakt-, konto- eller affärsmöjlighetssidorna. De visas också på kontrollpanelen [!DNL Sales Insight] i Lead Feed, [!DNL Best Bets] och Watch List.

![](assets/using-interesting-moments-6.png)

## Hur ser en intressant stund ut i [!DNL Salesforce1]? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

När du har installerat eller uppdaterat [!DNL Marketo Sales Insight] för [!DNL Salesforce1] visas intressanta stunder under leadets relaterade länkar.

![](assets/using-interesting-moments-7.png)

## Prenumerera på intressanta ögonblick {#subscribe-to-interesting-moments}

Du kan prenumerera på ett intressant tillfälle genom att klicka på knappen [!UICONTROL Subscribe] på fliken Intressant stund eller i lead-flödet. Stegen nedan är desamma för båda.

1. Klicka på prenumerationsikonen. Du kommer sedan till fliken E-postprenumeration.

1. Du kan välja vilken typ av e-postavisering du vill få baserat på [!UICONTROL Name], [!UICONTROL Account], [!UICONTROL Type] eller [!UICONTROL Description].

1. Välj vilken eller vilka e-postadresser du vill skicka aviseringarna till (dig själv/teammedlemmar)

1. Klicka på **[!UICONTROL Subscribe]**.

>[!NOTE]
>
>När användaren prenumererar på Intressant stund-typer eller beskrivningar får användaren e-postmeddelanden till personer (leads/kontakter) som de äger när de utlöser ett intressant tillfälle som matchar den typen eller beskrivningen.

![](assets/using-interesting-moments-8.png)
