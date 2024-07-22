---
unique-page-id: 6094890
description: Versionsinformation -februari 2015 - Marketo Docs - produktdokumentation
title: Versionsinformation - februari 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Versionsinformation: februari 2015 {#release-notes-february}

Följande funktioner finns i februari 2015-versionen. Kontrollera om det finns funktioner i Marketo Edition. Efter releasen måste du komma tillbaka för att hitta länkar till detaljerade artiklar för varje funktion. Trumrulle...

## Förbättringar av marknadsföringsautomatisering {#marketing-automation-enhancements}

**[Flytta smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Rejöst! Nu kan du flytta smarta kampanjer in och ut ur programmen genom att dra och släppa eller flytta funktionen Flytta i trädet.

**[Dynamics 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - stöds!

**HTTPS-certifikatändringar**

För att skydda sekretess och integritet för kunddata och SaaS-tjänster följer Marketo SaaS branschstandarder

och kommer att ersätta de säkerhetsprotokoll som används (SHA-1 och SSL) med säkrare versioner (SHA-2 (även SHA-256) och TLS) för följande domäner:

* marketo.net (krypterad Munchkin-trafik)

* [marketo.com](https://marketo.com) (SaaS-huvudprogram)

Det här kommer att hända kort efter den här versionen. SHA-1-protokollet stöds tillfälligt på domänen [mktoapi.com](https://mktoapi.com) fram till december 2015 så att ägare av äldre system och program kan uppdatera sina system med SHA-2-kompatibilitet.

**Secure Munchkin**

Vi tar bort vårt stöd för SSL3. Vi har underhållit SSL3 hittills för att behålla stödet för gamla webbläsare, men 2015 ser vi inte längre någon större webbtrafik från dessa webbläsare. Detta påverkar bara Munchkin när det används på säkra sidor och kommer att lanseras långsamt efter februari-utgåvan.

## Förbättringar av Personalization i realtid {#real-time-personalization-enhancements}

**[Mål-URL för kampanjer](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Välj de sidor som du vill att din realtidskampanj ska visa när du använder Lägg till en mål-URL. Den här funktionen fungerar med alla kampanjtyper (Dialog, In Zone, Widgets), men är särskilt värdefull för In Zone-kampanjer där en kampanj återges i zon-ID:t för endast den valda mål-URL:en. Det har stöd för att lägga till flera URL:er för olika webbsidor.

![](assets/image2015-2-19-11-3a0-3a30.png)

**Land och delstat har lagts till i kontobaserad marknadsföring**

Land och stat kan nu läggas till i dina namngivna kontolistor. Rikta presumtiva nyckelkonton från specifika platser.
