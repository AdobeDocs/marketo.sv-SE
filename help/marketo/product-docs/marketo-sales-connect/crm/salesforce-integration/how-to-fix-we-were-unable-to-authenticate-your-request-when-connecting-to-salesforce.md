---
unique-page-id: 14352484
description: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce - Marketo Docs - produktdokumentation
title: Så här åtgärdar du"Vi kunde inte autentisera din begäran" vid anslutning till Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Så här åtgärdar du&quot;Vi kunde inte autentisera din begäran&quot; vid anslutning till Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Om du får felmeddelandet&quot;Vi kunde inte autentisera din begäran&quot; när du försöker ansluta Sales Connect till Salesforce kan det finnas en begränsning för din åtkomst till Salesforce-API:t. Kontakta din Salesforce-administratör för att kontrollera att följande saker finns på plats.

## Aktivera API i användarbehörigheter {#enable-api-in-user-permissions}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Konfigurera**.
1. Välj **Hantera användare**.
1. Välj **Profiler**.
1. Hitta den profil som ToutApp-användarna befinner sig under och klicka på **Redigera**.
1. Bläddra ned till **Administrativa behörigheter** och kontrollera att **API-aktivering** är markerat.

## Kontrollera om Salesforce blockerar Sales Connect från Connecting {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Låt en Salesforce-administratör logga in på SFDC.
1. Välj **Konfigurera**.
1. Välj **Hantera program**.
1. Välj **Anslutna appar för OAuth-användning**.
1. Se till att Sales Connect visar &quot;Block&quot; bredvid det. Om du ser &quot;Avblockera&quot; klickar du på knappen för att avblockera Sales Connect-åtkomsten till Salesforce.
