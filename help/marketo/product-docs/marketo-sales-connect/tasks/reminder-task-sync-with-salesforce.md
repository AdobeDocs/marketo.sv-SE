---
description: Synkronisering av påminnelseuppgifter med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisering av påminnelseaktivitet med Salesforce
hide: true
hidefromtoc: true
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Synkronisering av påminnelseaktivitet med Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Om du vill veta mer om hur du aktiverar uppgiftssynkronisering kan du checka ut [Synkronisera aktiviteter/påminnelser för Sales Connect till Salesforce-aktiviteter](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

När inställningarna för uppgiftssynkronisering är aktiverade kommer användare att se sina påminnelseuppgifter dubbelsynkroniserade med Salesforce. Det innebär att användare kan hantera uppgifter från antingen Salesforce eller Sales Connect och känna sig säkra på att systemen är anpassade efter varandra.

## Synkronisering av påminnelseaktivitetsfält {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nedan visas en lista över påminnelseuppgiftsfälten i Sales Connect och deras motsvarande Salesforce-fält som stöds via dubbelriktad uppgiftssynkronisering.

<table>
 <tr>
  <th>Aktivitetsfält för försäljningskontakt</th>
  <th>Salesforce-aktivitetsfält</th>
  <th>Salesforce-aktivitet</th>
 </tr>
 <tr>
  <td>Aktivitetsnamn</td>
  <td>Ämnesfält</td>
  <td>Ett kort sammanfattningsfält som ska visa aktivitetens titel.</td>
 </tr>
 <tr>
  <td>Status</td>
  <td>Aktivitetsstatus</td>
  <td><p>Visar aktivitetens status. Sales Connect-aktiviteter har två statusvärden som är mappade till två av värdena i Salesforce-uppgiftsstatuslistan.</p>
  <p>Öppna i försäljningskontakt = Inte startat i Salesforce.</p>
  <p>Slutför i försäljningskontakt = Slutförd i Salesforce.</p>
  <p>De andra statusvärdena i Salesforce kommer inte att synkroniseras med Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Prioritet</td>
  <td>Prioritet</td>
  <td><p>Prioriteten för Säljanslutning kan vara Normal eller Hög, vilket mappar till värdena Normal och Hög prioritet i Salesforce.</p>
  <p>Värdet med låg prioritet i Salesforce synkroniseras inte med Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Förfallodatum</td>
  <td>Förfallodatum</td>
  <td>Datumet då uppgiften förfaller.</td>
 </tr>
 <tr>
  <td>Detaljer</td>
  <td>Kommentarer</td>
  <td>Visar mer detaljerad information om vad som var tänkt att slutföras med påminnelseaktiviteten.</td>
 </tr>
</table>

## Synkroniserar Sales Connect-aktiviteter med Salesforce för första gången {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan Sales Connect- och Salesforce-uppgifter importerar vi dina Salesforce-uppgifter. Vi ska **not** föra över alla aktuella uppgifter du har i Sales Connect till Salesforce. För att minska problem och dubbletter är de enda uppgifter som synkroniseras från Sales Connect till Salesforce de uppgifter som skapas *efter* du synkroniserar Sales Connect med SFDC.

Det här händer när du synkroniserar Sales Connect- och SFDC-uppgifter:

* När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

* Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till Sales Connect. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

* Om synkronisering har aktiverats tidigare och du tar bort några uppgifter i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

* Vi synkroniserar kontinuerligt uppgifter mellan Sales Connect och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i Sales Connect att synkroniseras med din uppgiftslista i Salesforce. Och allt som du har skapat, redigerat, slutfört eller tagit bort i Salesforce kommer att uppdatera din uppgiftslista i Sales Connect.

Aktivera synkroniseringen genom att markera synkroniseringsrutan i [Sidan Inställningar](https://toutapp.com/login) i webbprogrammet.
