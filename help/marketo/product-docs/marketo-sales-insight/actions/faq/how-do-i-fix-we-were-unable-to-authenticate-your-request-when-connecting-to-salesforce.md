---
description: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Hur korrigerar jag&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till [!DNL Salesforce]? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du försöker ansluta din Marketo Sales-instans till Salesforce och du ser felet&quot;Vi kan inte autentisera din begäran&quot;, är det troligen relaterat till hur din Salesforce-instans är konfigurerad.

Det finns två typer av fel som kan leda till den här felaktiga autentiseringssidan.

* Inloggningsfel - begränsad domän
* Oauth-appen har blockerats

Du kan identifiera vilken typ du får genom att kontrollera URL-adressen.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Åtgärda inloggningsfel begränsad domän {#resolve-login-error-restricted-domain}

Det här felet indikerar vanligtvis att du har en anpassad domän som vi inte kan dirigera till. Du kan åtgärda det här felet genom att försöka logga in på den Salesforce-instans som du vill ansluta till först. Gå sedan igenom stegen för att ansluta till Salesforce.

Om instansen som du försöker ansluta till är en Salesforce Sandbox-domän och du får ett felmeddelande, måste du gå igenom ytterligare steg för att uppdatera instansen så att den blir Salesforce Sandbox-kompatibel. [Läs mer](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Lös OAuth-appen blockerad {#resolve-oauth-app-blocked}

Om du fick felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; med feltypen Oauth App Blocked (eller en annan typ) i URL:en kan det finnas en begränsning för din åtkomst till Salesforce API. Kontakta din Salesforce-administratör för att kontrollera att nedanstående saker är på plats.

### Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in på Salesforce.
1. Välj **Konfigurera**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta den profil som ToutApp-användarna befinner sig under och klicka på **Redigera**.
1. Bläddra ned till **Administrativa behörigheter** och kontrollera att **API-aktivering** är markerat.

### Kontrollera om Salesforce blockerar Sales Insight-åtgärder från Connecting {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Låt en Salesforce-administratör logga in på Salesforce.
1. Välj **Konfigurera**.
1. Välj **Hantera program**.
1. Välj **Anslutna appar för OAuth-användning**.
1. Se till att Sales Insight Actions visar &quot;Block&quot; bredvid den. Om du ser &quot;Lås upp&quot; klickar du på knappen för att häva blockeringen av Sales Insight Actions&#39; åtkomst till Salesforce.
