---
unique-page-id: 6094890
description: Versionsinformation -februari 2015 - Marketo Docs - Produktdokumentation
title: Versionsinformation - februari 2015
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# Versionsinformation: Februari 2014 {#release-notes-february}

Följande funktioner finns i februari 2015-versionen. Kontrollera om din Marketo Edition innehåller funktioner. Efter releasen måste du komma tillbaka för att hitta länkar till detaljerade artiklar för varje funktion. Trumrulle...

## Förbättringar av marknadsföringsautomatisering {#marketing-automation-enhancements}

** [Flytta smart kampanj](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Rejöst! Nu kan du flytta smarta kampanjer in och ut ur programmen genom att dra och släppa eller flytta funktionen Flytta i trädet.

** [Dynamics 2015 (Online)](http://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) **- stöds!

**Ändringar av HTTPS-certifikat**

För att skydda sekretess och integritet för kunddata och SaaS-tjänster följer Marketo Saas branschstandarder

och kommer att ersätta de säkerhetsprotokoll som för närvarande används (SHA-1 och SSL) med säkrare versioner (SHA-2 (alias). SHA-256) och TLS) för följande domäner:

`·` [marketo.net](http://marketo.net)  (krypterad Munchkin-trafik)

`·` [marketo.com](http://marketo.com) (de viktigaste SaaS-programmen)

Det här kommer att hända kort efter den här versionen. SHA-1-protokollet stöds tillfälligt på domänen [mktoapi.com](http://mktoapi.com) till december 2015 så att ägare av äldre system och program kan uppdatera sina system med SHA-2-kompatibilitet.

**Secure Munchkin**

Vi tar bort vårt stöd för SSL3. Vi har underhållit SSL3 hittills för att behålla stödet för gamla webbläsare, men 2015 ser vi inte längre någon större webbtrafik från dessa webbläsare. Detta påverkar bara Munchkin när det används på säkra sidor och kommer att lanseras långsamt efter februari-utgåvan.

## Förbättringar av personalisering i realtid {#real-time-personalization-enhancements}

** [Mål-URL för kampanjer](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Välj de sidor som du vill att din realtidskampanj ska visa när du använder Lägg till en mål-URL. Den här funktionen fungerar med alla kampanjtyper (Dialog, In Zone, Widgets), men är särskilt värdefull för In Zone-kampanjer där en kampanj återges i zon-ID:t för endast den valda mål-URL:en. Det har stöd för att lägga till flera URL:er för olika webbsidor.

![](assets/image2015-2-19-11-3a0-3a30.png)

** [Land och delstat tillagd i kontobaserad målgruppering](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)**

Land och stat kan nu läggas till i dina namngivna kontolistor. Rikta presumtiva kunder för nyckelkonton från specifika platser.
