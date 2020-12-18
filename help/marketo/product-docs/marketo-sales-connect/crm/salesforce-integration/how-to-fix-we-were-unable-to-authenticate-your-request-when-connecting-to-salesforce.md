---
unique-page-id: 14352484
description: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Så här åtgärdar du&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; när du försöker ansluta Sales Connect till Salesforce kan det finnas en begränsning för din åtkomst till Salesforce-API:t. Kontakta din Salesforce-administratör för att kontrollera att följande saker finns på plats.

## Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta den profil som ToutApp-användarna befinner sig under och klicka på **Redigera**.
1. Bläddra nedåt till **Administrativa behörigheter** och kontrollera att **API Enabled** är markerat.

## Kontrollera om Salesforce blockerar Sales Connect från Anslutning {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera program**.
1. Välj **Anslutna appar OAuth-användning**.
1. Se till att Sales Connect visar &quot;Block&quot; bredvid det. Om du ser &quot;Avblockera&quot; klickar du på knappen för att avblockera Sales Connect-åtkomsten till Salesforce.

