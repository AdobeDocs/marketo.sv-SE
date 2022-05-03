---
description: Så här fungerar Veeva Sync - Marketo Docs - produktdokumentation
title: Veeva-synkronisering
hide: true
hidefromtoc: true
source-git-commit: c36b9206494c14a52937fa787a37601eaf6f4bd4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Veeva-synkronisering {#understanding-the-veeva-sync}

Med några enkla steg är det enkelt att synkronisera mellan Adobe Marketo Engage och Veeva CRM.

## Så här fungerar synkroniseringen {#how-the-sync-works}

Marketo Engage synkroniserar med Veeva CRM hela dagen, varje dag. Varje synkronisering tar en stund, pausar i 5 minuter och startar sedan igen.

>[!NOTE]
>
>Den allra första synkroniseringen kan ta timmar eller till och med dagar eftersom Marketo Engage kopierar hela databasen från Veeva. Efter det tar varje synkronisering vanligtvis minuter (ibland sekunder) och synkroniserar bara data som har ändrats.

![](assets/understanding-the-veeva-sync-1.png)

Synkroniseringen mellan Veeva och Marketo Engage är endast dubbelriktad för kontaktfält i Person-kontoobjektet. När du gör ändringar i antingen Veeva eller Marketo Engage återspeglas dina uppdateringar i båda systemen. Alla andra synkningar är endast från Veeva till Marketo Engage. Klicka på länkarna nedan om du vill ha information om var och en av länkarna.

## Vad är Synkroniserat mellan Marketo och Veeva? {#what-is-synced-between-marketo-and-veeva}

Personkonton Användare anropar och anropar nyckelobjekt, anpassade objekt

## Saker att veta {#things-to-know}

* De inloggningsuppgifter du anger i Marketo Engage för Veveva används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

* Veeva CRM baseras på force.com och den omfattande upplevelse som Marketo Engage har med plattformen ärvs till den här synkroniseringen.

* Veeva CRM visar: Lead, kontakt, konton (affärskonton, säljprojekt, kampanj och aktivitet). De stöds dock inte i synkroniseringen med Marketo Engage.
