---
unique-page-id: 14352541
description: Synkroniserar Sales Connect-uppgifter med Salesforce för första gången - Marketo Docs - produktdokumentation
title: Synkroniserar Sales Connect-aktiviteter med Salesforce för första gången
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Synkroniserar Sales Connect-aktiviteter med Salesforce för första gången {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan Sales Connect- och Salesforce-uppgifter importerar vi dina Salesforce-uppgifter. Vi ska **not** föra över alla aktuella uppgifter du har i Sales Connect till Salesforce. För att minska problem och dubbletter är de enda uppgifter som synkroniseras från Sales Connect till Salesforce de uppgifter som skapas *efter* du synkroniserar Sales Connect med SFDC.

Det här händer när du synkroniserar Sales Connect- och SFDC-uppgifter:

- När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

- Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till Sales Connect. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

- Om synkronisering har aktiverats tidigare och du tar bort några uppgifter i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

- Vi synkroniserar kontinuerligt uppgifter mellan Sales Connect och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i Sales Connect att synkroniseras med din uppgiftslista i Salesforce. Och allt som du har skapat, redigerat, slutfört eller tagit bort i Salesforce kommer att uppdatera din uppgiftslista i Sales Connect.

Aktivera synkroniseringen genom att markera synkroniseringsrutan i [Sidan Inställningar](https://toutapp.com/login) i webbprogrammet.
