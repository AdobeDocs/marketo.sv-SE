---
unique-page-id: 14352480
description: SFDC (Reply Logging) - Marketo Docs - Produktdokumentation
title: SFDC (Reply Logging)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# SFDC (Reply Logging) {#reply-logging-sfdc}

Sales Connect ger dig möjlighet att automatiskt logga presumtiva kunders svar till Salesforce. Strukturen som gör att du kan göra detta baseras på vår spårning av e-postsvar. Om vi kan spåra svar från en potentiell kund kan vi logga svaret till Salesforce.

## Krav {#requirements}

* E-postmeddelanden måste loggas via API-loggning
* Måste kunna [spåra ett svar](http://docs.marketo.com/x/BYPS)
* Måste vara ansluten till Salesforce
* Måste ha Salesforce [API-anrop](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) tillgängliga

## Aktivera svarsloggning {#enable-reply-logging}

1. Om du vill aktivera svarsloggning går du till sidan med [Salesforce-inställningar](http://docs.marketo.com/pages/assets/external-link.jspa) . När API-loggningen är avmarkerad ser du alternativet att kontrollera *Loggsvar.\
   *

   >[!NOTE]
   >
   >Svarsloggning följer samma regler som du har för att logga skickade e-postmeddelanden. Detta inkluderar hur e-postmeddelanden loggas. Leads och kontakter. om det finns en dubblettpost, om inga matchande poster hittas.

## Ange typ till svar i Salesforce {#setting-type-to-reply-in-salesforce}

Det är viktigt att du hämtar meningsfulla data från dina Salesforce-rapporter. Om du har möjlighet att fylla i fältet Typ som Svara kan du hämta data genom dina rapporter. Samarbeta med dig `Salesforce admin` för att få den här konfigurationen.

1. Gå till **Inställningar **> **Anpassa **> **Aktiviteter **> **Aktivitetsfält**.
1. Klicka på **Text**.
1. Klicka på **Ny** under Värden för aktivitetstypväljaren.
1. Skriv&quot;Svara&quot; i den tomma rutan. Se till att du börjar med versal och klickar på **Spara**.

   >[!NOTE]
   >
   >Du behöver inte välja en standard i typväljaren. Sales Connect kommer att se att den här aktivitetstypen är tillgänglig i din Salesforce-instans och fylla i aktivitetsfältet på dina inkommande aktiviteter i enlighet med detta.

