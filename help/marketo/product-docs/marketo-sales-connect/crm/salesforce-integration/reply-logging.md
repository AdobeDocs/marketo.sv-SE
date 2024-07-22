---
unique-page-id: 14352480
description: SFDC (Reply Logging) - Marketo Docs - produktdokumentation
title: SFDC (Reply Logging)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# SFDC (Reply Logging) {#reply-logging-sfdc}

Sales Connect ger dig möjlighet att automatiskt logga dina prospects svar till Salesforce. Strukturen som gör att du kan göra detta baseras på vår spårning av e-postsvar. Om vi kan spåra svar från en potentiell kund kan vi logga svaret till Salesforce.

## Krav {#requirements}

* E-postmeddelanden måste loggas via API-loggning
* Du måste kunna [spåra ett svar](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Måste vara ansluten till Salesforce
* Salesforce [API-anrop](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) måste vara tillgängliga

## Aktivera svarsloggning {#enable-reply-logging}

1. Om du vill aktivera svarsloggning går du till sidan med Salesforce-inställningar. När API-loggningen är utcheckad ser du alternativet att kontrollera _Logga svar_.

   >[!NOTE]
   >
   >Svarsloggning följer samma regler som du har för att logga skickade e-postmeddelanden. Detta inkluderar hur e-postmeddelanden loggas, till Leads och Kontakter, när det finns en dubblettpost och om inga matchande poster hittas.

## Ange typ till svar i Salesforce {#setting-type-to-reply-in-salesforce}

Det är viktigt att du hämtar meningsfulla data från dina Salesforce-rapporter. Om du har möjlighet att fylla i fältet Typ som Svara kan du hämta data genom dina rapporter. Anslut till din `Salesforce admin` för att få den här konfigurationen.

1. Gå till **Inställningar** > **Anpassa** > **Aktiviteter** > **Åtgärdsfält**.
1. Klicka på **Typ**.
1. Klicka på **Ny** under Värden för aktivitetstypväljaren.
1. Skriv&quot;Svara&quot; i den tomma rutan. Se till att du börjar med versal och klickar på **Spara**.

   >[!NOTE]
   >
   >Du behöver inte välja en standard i typväljaren. Sales Connect ser att den här aktivitetstypen är tillgänglig i din Salesforce-instans och fyller i aktivitetsfältet på dina inkommande aktiviteter därefter.
