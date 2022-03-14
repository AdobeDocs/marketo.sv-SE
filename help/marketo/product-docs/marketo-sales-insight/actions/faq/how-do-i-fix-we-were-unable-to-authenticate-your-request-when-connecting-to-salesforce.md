---
description: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Hur korrigerar jag"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce?
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Hur korrigerar jag&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till Salesforce? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; när du försöker ansluta Sales Insight-åtgärder till Salesforce kan det finnas en begränsning för din åtkomst till Salesforce-API:t. Kontrollera med din Salesforce-administratör att följande saker finns på plats.

## Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta profilen som ToutApp-användarna är under och klicka på **Redigera**.
1. Bläddra nedåt till **Administrativa behörigheter** och se till att **API aktiverat** är markerad.

## Kontrollera om Salesforce blockerar åtgärder för försäljningsinsikter från anslutning {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Inställningar**.
1. Välj **Hantera program**.
1. Välj **OAuth-användning för anslutna appar**.
1. Se till att Sales Insight Actions visar &quot;Block&quot; bredvid den. Om du ser &quot;Lås upp&quot; klickar du på knappen för att häva blockeringen av Sales Insight Actions&#39; åtkomst till Salesforce.
