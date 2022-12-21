---
description: Svarsloggning - Marketo Docs - produktdokumentation
title: Svarsloggning
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
source-git-commit: d960f0ad0d944bd2e74543f3ab15b59a8040b768
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Svarsloggning {#reply-logging}

Sales Insight Actions ger er möjlighet att automatiskt logga presumtiva kunders svar till Salesforce. Strukturen som gör att du kan göra detta baseras på vår spårning av e-postsvar. Om vi kan spåra svar från en potentiell kund kan vi logga svaret till Salesforce.

## Krav {#requirements}

* E-postmeddelanden måste loggas via API-loggning
* Måste kunna [spåra ett svar](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Måste vara ansluten till Salesforce
* Måste ha Salesforce [API-anrop](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) tillgänglig

## Aktivera svarsloggning {#enable-reply-logging}

1. Om du vill aktivera svarsloggning går du till sidan med Salesforce-inställningar. När API-loggningen är avmarkerad ser du alternativet att kontrollera _Loggsvar_.

   >[!NOTE]
   >
   >Svarsloggning följer samma regler som du har för att logga skickade e-postmeddelanden. Detta inkluderar hur e-postmeddelanden loggas. Leads och kontakter. om det finns en dubblettpost, om inga matchande poster hittas.

## Ange typ till svar i Salesforce {#setting-type-to-reply-in-salesforce}

Det är viktigt att du hämtar meningsfulla data från dina Salesforce-rapporter. Om du har möjlighet att fylla i fältet Typ som Svara kan du hämta data genom dina rapporter. Samarbeta med `Salesforce admin` för att få den här konfigurationen.

1. Gå till **Inställningar** > **Anpassa** > **Verksamhet** > **Aktivitetsfält**.
1. Klicka **Typ**.
1. Klicka på under Värden i listan över aktivitetstyper **Nytt**.
1. Skriv&quot;Svara&quot; i den tomma rutan. Se till att du börjar med &quot;R&quot; och klickar **Spara**.

   >[!NOTE]
   >
   >Du behöver inte välja en standard i typväljaren. Sales Insight-åtgärder kommer att se att den här aktivitetstypen är tillgänglig i din Salesforce-instans och fylla i aktivitetsfältet på dina inkommande aktiviteter i enlighet med detta.
