---
unique-page-id: 2953461
description: SFDC Sync -Field Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - fältsynkronisering
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# SFDC-synkronisering: Fältsynkronisering {#sfdc-sync-field-sync}

Marketo synkroniserar fältinformation från Salesforce. Här är detaljerna.

## Vilka fält synkroniseras? {#which-fields-are-synced}

Vi synkroniserar de flesta standardfält i SFDC och alla anpassade fält som synkroniseringsanvändaren har behörighet att se.

## Hur avgör du om en post i Marketo är en lead eller en kontakt i Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Vi har ett fält i Marketo som kallas SFDC-typ. Den har tre möjliga värden: lead, contact, or it is empty. Om den är tom betyder det att denna Marketo-lead inte finns i SFDC.

## Hur avgör du om en lead eller kontakt tas bort i SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Vi har ett fält i Marketo som kallas SFDC isDeleted. Om värdet är true togs leadet bort i SFDC.

## Hur ser jag till att ett nytt fält som jag lägger till i SFDC också läggs till i Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Om du vill ha ett fält i båda systemen skapar du det först i SFDC och synkroniserar automatiskt ned till Marketo.

Om du lägger till ett nytt fält i SFDC och synkroniseringsanvändaren har behörighet att se det, läggs det automatiskt till i Marketo.

## Vad händer om jag ändrar en fältetikett i SFDC? {#what-if-i-change-a-field-label-in-sfdc}

Om du ändrar fältetiketten i SFDC påverkas inte fältetiketten i Marketo.

## Vad händer om jag ändrar en fälttyp i SFDC? {#what-if-i-change-a-field-type-in-sfdc}

När du ändrar en fälttyp tas data i fälten bort om de inte matchar (men först visas en varning). Om du vill bevara data måste du exportera dem och importera dem igen när du har ändrat fälttypen.

## Vad händer om jag ändrar ett API-namn i SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Om du ändrar API-namnet för ett fält i SFDC skapas ett nytt fält i Marketo.

## Vad händer om jag lägger till ett nytt listvärde i SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Om ett nytt listvärde läggs till i SFDC till ett fält, skickar Marketo ett meddelande till dig.

## Vad gäller för anpassade SFDC-sökfält? {#what-about-custom-sfdc-lookup-fields}

Sökfält i SFDC synkroniserar ID:t men inte det refererade namnet.

## SFDC-formelfält då? {#what-about-sfdc-formula-fields}

Formelfält synkroniseras, men uppdateringar av referenserna i formeln synkroniseras inte förrän det finns en uppdatering av en [systemstämpel](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## Vad händer när jag tar bort ett fält från Salesforce som tidigare synkroniserades med Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Om du tar bort ett fält i SFDC tas inte fältet i Marketo bort automatiskt, utan synkroniseringen avbryts.
