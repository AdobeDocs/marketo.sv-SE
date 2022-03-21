---
description: Actions Data Sync FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om synkronisering av funktionsmakron
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Vanliga frågor om synkronisering av funktionsmakron {#actions-data-sync-faq}

Synkroniseringen av datafältet för Sales Insight-åtgärder gör att systemet kan hämta personinformation från din Marketo Engage-databas till din databas för Sales Insight-åtgärder.

Detta tillhandahåller aktuella persondata i webbappen Sales Insight Actions och gör det möjligt för systemet att samla in unika ID:n för motsvarande personposter i Marketo och lead-/kontakt-/konto-/affärsmöjlighetsposter i Salesforce, så att poster kan refereras till korrekt för loggningsdata.

Synkroniseringen kan aktiveras på fliken Sales Insight Actions Config i administratörsavsnittet i Marketo Engage. Mer information finns på [Initiera datasynkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Diagrammet ovan visar hur personaktivitets- och aktivitetsdata kan synkroniseras mellan system. Några saker att notera:

* Personposter synkroniseras till Sales Insight Actions från Marketo Engage, vilket gör Marketo Engage till källan för uppgifter om säljare i Sales Insight Actions
* Både Marketo Engage och Sales Insight [har en mekanism](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) för att samla in och synkronisera avbeställningsstatus till Salesforce
* Avbeställningsstatus synkroniseras inte från försäljningsåtgärder till Marketo Engage, men Sales Insight Actions kan konfigureras för att kontrollera status för Marketo Unsubscribe på personer innan säljarna kan skicka ett e-postmeddelande med [Avbeställ Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Nedan visas några vanliga frågor om hur synkroniseringen av data fungerar.

## Vilka leads/kontakter synkroniseras med Sales Insight Actions? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Leads och kontakter som har en försäljningsägare tilldelad till sig synkroniseras ned till Försäljningsåtgärder.

Du kan se om ett lead/en kontakt har en säljare i Salesforce genom att titta i det standardägarfält som finns.

Säljaren behöver inte vara synkroniseringsanvändare för Marketo eller någon specifik Salesforce- eller säljanvändare. Det enda vi behöver är att det finns en användare listad i fältet Lead-ägare och Kontaktägare i Salesforce, så att vi kan identifiera den som ett säljtips och synkronisera den med Sales Insight-åtgärder. Alla uppdateringar av fälten som vi synkroniserar med kommer också att identifieras och uppdateras i Sales Insight Actions.

## Var kommer aktivitetsdata som visas i Sales Insight Smart Grid ifrån? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Aktivitetsdata som e-post, samtal, intressanta ögonblick och webben hämtas från Marketo Engage databas. Sales Insight Smart Grid skickar en begäran till Marketo Engage-instansen om att hämta detta varje gång en säljanvändare läser in panelen Sales Insight.

![](assets/actions-data-sync-faq-4.png)

För att alla aktivitetsdata ska kunna hämtas från Marketo Engage synkroniseras alla aktivitetsdata till Marketo Engage.

## Vilka fält för personposter synkroniseras från Marketo Engage till Sales Insight-åtgärder? {#what-fields-sync}

Det finns 11 fält som synkroniseras från Marketo Engage till Sales Insight-åtgärder:

* Förnamn
* Efternamn
* Salesforce-kontakt-ID
* Salesforce lead-ID
* Marketo ID
* Företag
* Titel
* E-post
* Telefonnummer
* Linkedin-URL
* Källa

## Kan fälten som synkroniseras mellan Marketo Engage och Sales Insight Actions konfigureras? {#are-the-fields-that-sync-configurable}

Det går inte att konfigurera vilka Marketo Engage-fält som ska synkroniseras till åtgärder för försäljningsinsikter, och inte heller möjligheten att mappa fält. Synkroniseringen från Marketo mappar automatiskt vanliga Marketo-fält till standardfält i din instans av försäljningsåtgärd.

## Varför har Sales Insight Actions en egen databas? {#why-does-actions-have-its-own-database}

Sales Insight Actions har ett eget webbprogram med en dedikerad person- och aktivitetsdatabas som ger en optimerad arbetsyta som är framtagen och utformad för säljteam. På så sätt kan säljchefer och säljare få plats att bygga ut och hantera sin engagemangsstrategi utan att ge åtkomst till eller behörigheter för den primära arbetsytan i Marketo Engage, som är optimerad för marknadsföringsspecialister.

## Hur hanteras dubbletter? {#how-are-duplicates-handled}

Din databas för försäljningsåtgärder är en kopia av de kvalificerade personer (leads/kontakter med en säljare) som finns i din Marketo Engage-databas. Det innebär att om det finns två poster med samma e-postadress som har skapats i Marketo, skapas en dubblettpost i Försäljningsåtgärder.

## Hur lång tid tar det innan den första synkroniseringen är klar? {#how-long-initial-sync}

Den inledande processen för synkronisering av alla dina säljleads-data till en ny instans av Sales Insight Actions behandlar normalt personer vid cirka 1 000 varannan minut. Det här är bara en uppskattning och kan variera.

När den första synkroniseringen har utförts och alla säljleads har fyllts i i instansen av webbappen Sales Insight Actions, kommer det att finnas en stegvis synkronisering som körs varje gång ett av de fält som stöds uppdateras.

## Kan användare av Sales Insight Actions redigera persondata från webbappen Actions? {#can-actions-users-edit-people-data}

Nej, det går inte att skapa och redigera personposter i Åtgärder för både användare och administratörer av webbappen Åtgärder. Du måste skapa och redigera personer i Salesforce eller Marketo Engage. Sales Insight Actions använder Marketo som källa för persondata genom att kontinuerligt synkronisera nya data, så om en person uppdateras eller skapas i Marketo antingen från ett arbetsflöde i Marketo eller synkroniseras från Salesforce, skickas dessa uppdateringar till webbappsdatabasen för Sales Insight Actions.

## Loggar säljaktiviteterna till Marketo? {#do-sales-activities-log-to-marketo}

Ja, försäljningsaktiviteter loggar in på Marketo som inbyggda aktiviteter. De här aktiviteterna innehåller också inbyggda filter som kan användas med begränsningar för att rikta leads baserat på attribut för försäljningsaktivitet.

![](assets/actions-data-sync-faq-5.png)

Nedan finns en lista över de aktiviteter som loggar till Marketo:

* Skicka e-postmeddelande
* Open Sales Email
* Klicka på E-postadress
* Svar på e-postadress
* E-postförsäljning studsade
* Mottaget försäljningssamtal
* Lägg till i försäljningskampanj
* Borttagen från försäljningskampanj

## Loggar försäljningsaktiviteter till Salesforce? {#do-sales-activities-log-to-salesforce}

Ja, försäljningsinteraktionsaktiviteter loggar till Salesforce som inbyggda uppgifter. Dessa uppgifter kan sedan användas i Salesforce-rapporter för att underlätta för teamets kontrollpaneler som spårar försäljningsaktiviteter.

Med Sales Insight Actions kan administratörer konfigurera vilka försäljningsaktiviteter som loggas till Salesforce. Dessa aktiviteter omfattar e-post, samtal och öppna påminnelseuppgifter.

![](assets/actions-data-sync-faq-6.png)

Diagrammet ovan visar vilken information som loggas till Salesforce. Aktiviteter som e-post och samtal loggas till Salesforce i en [enkelriktad synkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Avbeställ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) och [Påminnelseaktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) hålls uppdaterade med tvåvägssynkronisering. Var och en av dessa datasynkroniseringar kan konfigureras från webbappen Sales Insight Actions.

>[!MORELIKETHIS]
>
>* [Synkronisera avbeställningar med Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Avbeställ Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Synkroniseringsinställningar för Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synkronisering av påminnelseaktivitet med Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Initiera datasynkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-guide.md#initiate-data-sync)

