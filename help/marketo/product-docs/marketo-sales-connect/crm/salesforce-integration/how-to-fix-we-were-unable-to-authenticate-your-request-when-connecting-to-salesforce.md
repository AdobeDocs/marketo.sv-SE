---
unique-page-id: 14352484
description: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Så här åtgärdar du&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; när du försöker ansluta Sales Connect till Salesforce kan det finnas en begränsning för din åtkomst till Salesforce-API:t. Kontrollera med din Salesforce-administratör att följande saker finns på plats.

## Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta profilen som ToutApp-användarna är under och klicka på **Redigera**.
1. Bläddra nedåt till **Administrativa behörigheter** och se till att **API aktiverat** är markerad.

## Kontrollera om Salesforce blockerar Sales Connect från Connecting {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera program**.
1. Välj **OAuth-användning för anslutna appar**.
1. Se till att Sales Connect visar &quot;Block&quot; bredvid det. Om du ser &quot;Avblockera&quot; klickar du på knappen för att avblockera Sales Connect-åtkomsten till Salesforce.
