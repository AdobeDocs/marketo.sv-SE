---
unique-page-id: 14352480
description: SFDC (Reply Logging) - Marketo Docs - Produktdokumentation
title: SFDC (Reply Logging)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# SFDC (Reply Logging) {#reply-logging-sfdc}

Sales Connect ger dig möjlighet att automatiskt logga presumtiva kunders svar till Salesforce. Strukturen som gör att du kan göra detta baseras på vår spårning av e-postsvar. Om vi kan spåra svar från en potentiell kund kan vi logga svaret till Salesforce.

## Krav {#requirements}

* E-postmeddelanden måste loggas via API-loggning
* Måste kunna [spåra ett svar](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Måste vara ansluten till Salesforce
* Måste ha Salesforce [API-anrop](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) tillgängliga

## Aktivera svarsloggning {#enable-reply-logging}

1. Om du vill aktivera svarsloggning går du till sidan med Salesforce-inställningar. När API-loggningen är avmarkerad kan du se alternativet _Logga svar_.

   >[!NOTE]
   >
   >Svarsloggning följer samma regler som du har för att logga skickade e-postmeddelanden. Detta inkluderar hur e-postmeddelanden loggas. Leads och kontakter. om det finns en dubblettpost, om inga matchande poster hittas.

## Anger typ som svar i Salesforce {#setting-type-to-reply-in-salesforce}

Det är viktigt att du hämtar meningsfulla data från dina Salesforce-rapporter. Om du har möjlighet att fylla i fältet Typ som Svara kan du hämta data genom dina rapporter. Anslut till din `Salesforce admin` för att få den här konfigurationen.

1. Gå till **Inställningar** > **Anpassa** > **Aktiviteter** > **Åtgärdsfält**.
1. Klicka på **Skriv**.
1. Klicka på **Nytt** under Värden för aktivitetstypväljaren.
1. Skriv&quot;Svara&quot; i den tomma rutan. Se till att du börjar med versal och klicka på **Spara**.

   >[!NOTE]
   >
   >Du behöver inte välja en standard i typväljaren. Sales Connect kommer att se att den här aktivitetstypen är tillgänglig i din Salesforce-instans och fylla i aktivitetsfältet på dina inkommande aktiviteter i enlighet med detta.
