---
description: Synkronisering av påminnelseuppgifter med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisering av påminnelseaktivitet med Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Synkronisering av påminnelseaktivitet med Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Om du vill veta mer om hur du aktiverar aktivitetssynkronisering kan du checka ut [Synkronisera försäljningsanslutningsuppgifter/påminnelser till Salesforce-uppgifter](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

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
  <td>Information</td>
  <td>Kommentar</td>
  <td>Visar mer detaljerad information om vad som var tänkt att slutföras med påminnelseaktiviteten.</td>
 </tr>
</table>

## Synkroniserar Sales Connect-aktiviteter med Salesforce för första gången {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan Sales Connect- och Salesforce-uppgifter importerar vi dina Salesforce-uppgifter. Vi kommer **inte** att föra över aktuella uppgifter som du har i Sales Connect till Salesforce. För att minska problem och dubbletter är de enda uppgifter som synkroniseras från Sales Connect till Salesforce aktiviteter som skapas *efter* att du synkroniserat Sales Connect med SFDC.

Det här händer när du synkroniserar Sales Connect- och SFDC-uppgifter:

* När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

* Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till Sales Connect. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

* Om synkronisering har aktiverats tidigare och du tar bort några uppgifter i SFDC, kommer allt som har tagits bort de senaste 15 dagarna att tas bort från kommandocentralen.

* Vi synkroniserar kontinuerligt uppgifter mellan Sales Connect och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i Sales Connect att synkroniseras med din uppgiftslista i Salesforce. Och allt som du har skapat, redigerat, slutfört eller tagit bort i Salesforce kommer att uppdatera din uppgiftslista i Sales Connect.

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på [inställningssidan](https://toutapp.com/login) i webbprogrammet.

>[!NOTE]
>
>Ämnesfältet för en aktivitet kan uppdateras i Sales Connect och den uppdateringen synkroniseras i Salesforce-ämnesfältet för motsvarande synkroniserade uppgift, om du använder det dynamiska fältet `{{activity_subject}}` i dina [inställningar för anpassning av aktivitetsinformation](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Omvänt kommer alla uppdateringar som görs i ämnesfältet i Salesforce _inte_ att synkroniseras till ämnesfältet i påminnelseaktiviteten för Sales Connect.
