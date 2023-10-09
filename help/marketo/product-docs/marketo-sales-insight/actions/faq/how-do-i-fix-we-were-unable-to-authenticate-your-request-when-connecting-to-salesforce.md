---
description: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: b09bff5fe72e5cce86ab4664e264edb181fa3e5c
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Hur korrigerar jag&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till Salesforce? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du försöker ansluta din Marketo Sales-instans till Salesforce och du ser felet&quot;Vi kan inte autentisera din begäran&quot;, är det troligen relaterat till hur Salesforce-instansen är konfigurerad.

Det finns två typer av fel som kan leda till den här felaktiga autentiseringssidan.

* Inloggningsfel - begränsad domän
* Oauth-appen har blockerats

Du kan identifiera vilken typ du får genom att kontrollera URL-adressen.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Åtgärda inloggningsfel begränsad domän {#resolve-login-error-restricted-domain}

Det här felet indikerar vanligtvis att du har en anpassad domän som vi inte kan dirigera till. Du kan lösa det här felet genom att försöka logga in på Salesforce-instansen som du vill ansluta till först. Gå sedan igenom stegen för att ansluta till Salesforce.

Om instansen som du försöker ansluta till är en Salesforce-sandlådedomän och du får ett fel, måste du gå igenom ytterligare steg för att uppdatera instansen så att den blir Salesforce-sandlådekompatibel. [Läs mer](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Lös OAuth-appen blockerad och andra feltyper {#resolve-oauth-app-blocked-and-other-error-types}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; med feltypen Oauth App Blocked eller en annan typ i URL:en, kan det finnas en begränsning för din åtkomst till Salesforce API. Kontakta din Salesforce-administratör för att kontrollera att följande saker finns på plats.

### Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in i Salesforce.
1. Välj **Inställningar**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta profilen som ToutApp-användarna är under och klicka på **Redigera**.
1. Bläddra nedåt till **Administrativa behörigheter** och se till att **API aktiverat** är markerad.

### Kontrollera om Salesforce blockerar åtgärder för försäljningsinsikter från anslutning {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Låt en Salesforce-administratör logga in i Salesforce.
1. Välj **Inställningar**.
1. Välj **Hantera program**.
1. Välj **OAuth-användning för anslutna appar**.
1. Se till att Sales Insight Actions visar &quot;Block&quot; bredvid den. Om du ser Upphäv blockering klickar du på knappen för att häva blockeringen av Sales Insight Actions åtkomst till Salesforce.
