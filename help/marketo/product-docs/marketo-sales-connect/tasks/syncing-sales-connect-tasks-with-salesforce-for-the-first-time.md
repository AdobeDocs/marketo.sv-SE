---
unique-page-id: 14352541
description: Synkronisera Sales Connect-uppgifter med Salesforce för första gången - Marketo Docs - produktdokumentation
title: Synkronisera Sales Connect-aktiviteter med Salesforce för första gången
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Synkroniserar [!DNL Sales Connect] aktiviteter med [!DNL Salesforce] för första gången {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan [!DNL Sales Connect] och [!DNL Salesforce] aktiviteter importerar vi dina [!DNL Salesforce]-aktiviteter. Vi kommer **inte** att föra över aktuella uppgifter som du har i [!DNL Sales Connect] till [!DNL Salesforce]. För att undvika rörighet och dubbletter är de enda uppgifter som synkroniseras från [!DNL Sales Connect] till [!DNL Salesforce] uppgifter som skapas *efter* att du har synkroniserat [!DNL Sales Connect] med SFDC.

Det här händer när du synkroniserar [!DNL Sales Connect]- och SFDC-uppgifter:

- När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

- Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till [!DNL Sales Connect]. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

- Om synkronisering har aktiverats tidigare och du tar bort åtgärder i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

- Vi synkroniserar uppgifter mellan [!DNL Sales Connect] och SFDC hela tiden så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i [!DNL Sales Connect] att synkroniseras till din uppgiftslista i [!DNL Salesforce]. Och allt som har skapats, redigerats, slutförts eller tagits bort i [!DNL Salesforce] kommer att uppdatera din uppgiftslista i [!DNL Sales Connect].

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på [inställningssidan](https://toutapp.com/login) i webbprogrammet.
