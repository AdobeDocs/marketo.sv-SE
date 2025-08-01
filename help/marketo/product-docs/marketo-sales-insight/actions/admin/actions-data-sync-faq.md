---
description: Actions Data Sync FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om synkronisering av funktionsmakron
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Vanliga frågor om synkronisering av funktionsmakron {#actions-data-sync-faq}

Fältsynkroniseringen för dataentifiering för [!DNL Sales Insight Actions] gör att systemet kan hämta personinformation från din Marketo Engage-databas till din [!DNL Sales Insight Actions]-databas.

Detta tillhandahåller aktuella persondata i webbappen [!DNL Sales Insight Actions] och gör att systemet kan samla unika ID:n för motsvarande personposter i Marketo och lead-/kontakt-/konto-/affärsmöjlighetsposter i [!DNL Salesforce], så att poster kan refereras korrekt för loggningsdata.

Synkroniseringen kan aktiveras från fliken [!DNL Sales Insight Actions] Config i administratörsavsnittet i Marketo Engage. Mer information finns i [Initiera datasynkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Diagrammet ovan visar hur personaktivitets- och aktivitetsdata kan synkroniseras mellan system. Några saker att notera:

* Personposter synkroniseras till [!DNL Sales Insight Actions] från Marketo Engage, vilket gör Marketo Engage till sanningskälla för [!DNL Sales Insight Actions] persondata
* Både Marketo Engage och [!DNL Sales Insight Actions] [har en mekanism](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) för att samla in och synkronisera status för att avbryta prenumerationen till [!DNL Salesforce]
* Avbeställningsstatus synkroniseras inte från försäljningsåtgärder till Marketo Engage, men [!DNL Sales Insight Actions] kan konfigureras för att kontrollera status för Marketo Unsubscribe på personer innan säljarna kan skicka ett e-postmeddelande med [Marketo Unsubscribe Check](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md) .

Nedan visas några vanliga frågor om hur synkroniseringen av data fungerar.

## Vilka leads/kontakter synkroniseras med [!DNL Sales Insight Actions]? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Leads och kontakter som har en försäljningsägare tilldelad till sig synkroniseras ned till Försäljningsåtgärder.

Du kan se om ett lead/en kontakt har en säljare i [!DNL Salesforce] genom att titta i standardägarfältet som finns.

Säljaren behöver inte vara synkroniseringsanvändare för Marketo eller någon specifik [!DNL Salesforce]- eller säljanvändare. Allt vi behöver är att det finns en användare i listan i fältet Lead-ägare och Kontaktägare i [!DNL Salesforce], så att vi kan identifiera den som ett säljtips och synkronisera den till [!DNL Sales Insight Actions]. Uppdateringar av fälten som vi synkroniserar med upptäcks och uppdateras även i [!DNL Sales Insight Actions].

## Var kommer aktivitetsdata som visas i Sales Insight Smart Grid ifrån? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Aktivitetsdata som e-post, samtal, intressanta ögonblick och webben kommer från Marketo Engage databas. Sales Insight Smart Grid skickar en begäran till Marketo Engage-instansen om att hämta detta varje gång en säljanvändare läser in panelen Sales Insight.

![](assets/actions-data-sync-faq-4.png)

[!DNL Sales Insight Actions] synkroniserar alla aktivitetsdata till Marketo Engage för att se till att alla aktivitetsdata kan hämtas från Marketo Engage.

## Vilka fält som är relaterade till personposter synkroniseras från Marketo Engage till [!DNL Sales Insight Actions]? {#what-fields-sync}

Det finns 11 fält som synkroniseras från Marketo Engage till [!DNL Sales Insight Actions]:

* Förnamn
* Efternamn
* [!DNL Salesforce] kontakt-ID
* [!DNL Salesforce] lead-ID
* Konto-ID för [!DNL Salesforce]
* [!DNL Salesforce] affärsmöjlighets-ID
* MARKETO ID
* Företag
* Titel
* E-post
* Telefonnummer
* URL för [!DNL Linkedin]
* Källa

## Kan fälten som synkroniseras mellan Marketo Engage och [!DNL Sales Insight Actions] konfigureras? {#are-the-fields-that-sync-configurable}

Det går inte att konfigurera vilka Marketo Engage-fält som ska synkroniseras till [!DNL Sales Insight Actions] och inte heller att mappa fält. Synkroniseringen från Marketo mappar automatiskt vanliga Marketo-fält till standardfält i din instans av försäljningsåtgärd.

## Varför har [!DNL Sales Insight Actions] en egen databas? {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] har ett eget webbprogram med en dedikerad person- och aktivitetsdatabas för att tillhandahålla en optimerad arbetsyta som har skapats och utformats för säljteam. På så sätt kan säljchefer och säljare skapa och hantera sin strategi för engagemang   utan att ge åtkomst till eller behörighet till den primära Marketo Engage-arbetsytan, som är optimerad för marknadsföringsspecialister.

## Hur hanteras dubbletter? {#how-are-duplicates-handled}

Din databas för försäljningsåtgärder är en kopia av de kvalificerade personer (leads/kontakter med en säljare) som finns i din Marketo Engage-databas. Det innebär att om det finns två poster med samma e-postadress som har skapats i Marketo, skapas en dubblettpost i Försäljningsåtgärder.

## Hur lång tid tar det innan den första synkroniseringen är klar? {#how-long-initial-sync}

Den inledande processen för synkronisering av alla dina säljleads-data till en ny [!DNL Sales Insight Actions]-instans behandlar normalt personer vid cirka 1 000 varannan minut. Det här är bara en uppskattning och kan variera.

När den första synkroniseringen har utförts och alla dina säljleads har fyllts i i din [!DNL Sales Insight Actions]-webbprograminstans, kommer en stegvis synkronisering att utföras varje gång det finns en uppdatering till ett av de fält som stöds som synkroniseras.

## Kan [!DNL Sales Insight Actions] användare redigera persondata från webbappen Åtgärder? {#can-actions-users-edit-people-data}

Nej, det går inte att skapa och redigera personposter i Åtgärder för både användare och administratörer av webbappen Åtgärder. Du måste skapa och redigera personer i [!DNL Salesforce] eller Marketo Engage. [!DNL Sales Insight Actions] använder Marketo som källa för sanning för persondata genom att kontinuerligt synkronisera nya data, så om en person uppdateras eller skapas i Marketo antingen från ett arbetsflöde i Marketo eller synkroniseras från [!DNL Salesforce], skickas dessa uppdateringar till webbprogramdatabasen [!DNL Sales Insight Actions].

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

## Loggar försäljningsaktiviteter till [!DNL Salesforce]? {#do-sales-activities-log-to-salesforce}

Ja, aktiviteter för försäljningsengagemang loggar till [!DNL Salesforce] som inbyggda uppgifter. De här uppgifterna kan sedan användas i [!DNL Salesforce]-rapporter för att underlätta för team-instrumentpaneler som spårar försäljningsaktiviteter.

[!DNL Sales Insight Actions] tillåter administratörer att konfigurera vilka försäljningsaktiviteter som är loggade till [!DNL Salesforce]. Dessa aktiviteter omfattar e-post, samtal och öppna påminnelseuppgifter.

![](assets/actions-data-sync-faq-6.png)

Diagrammet ovan visar vilken information som loggas till [!DNL Salesforce]. Aktiviteter som e-post och samtal loggas till [!DNL Salesforce] i en [enkelriktad synkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Avbeställningar](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) och [Påminnelseaktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) uppdateras med en tvåvägssynkronisering. Var och en av dessa datasynkroniseringar kan konfigureras från webbappsgränssnittet [!DNL Sales Insight Actions].

>[!MORELIKETHIS]
>
>* [Synkroniserar Avsluta prenumeration med [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Avbeställ Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] Synkronisera inställningar](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synkronisering av påminnelseaktivitet med [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Starta datasynkronisering](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
