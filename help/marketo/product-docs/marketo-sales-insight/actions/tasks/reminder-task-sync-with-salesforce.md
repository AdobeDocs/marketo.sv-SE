---
description: Synkronisering av påminnelseuppgifter med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisering av påminnelseaktivitet med Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Synkronisering av påminnelseaktivitet med Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Om du vill lära dig hur du aktiverar aktivitetssynkronisering kan du checka ut [Synkronisera åtgärder för försäljningsinformation/påminnelser till Salesforce-aktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

När inställningarna för uppgiftssynkronisering är aktiverade kommer användare att se sina påminnelseuppgifter dubbelsynkroniserade med Salesforce. Det innebär att användare kan hantera uppgifter från antingen Salesforce eller Sales Insight Actions och känna sig säkra på att systemen är anpassade efter varandra.

## Synkronisering av påminnelseaktivitetsfält {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nedan visas en lista över påminnelseuppgiftsfälten i Sales Insight Actions och deras motsvarande Salesforce-fält som stöds via dubbelriktad uppgiftssynkronisering.

<table>
 <tr>
  <th>Aktivitetsfält för försäljningsinsiktsåtgärder</th>
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
  <td><p>Visar aktivitetens status. Aktiviteter för Säljningsåtgärder har två statusvärden som är mappade till två av värdena i Salesforce-uppgiftsstatuslistan.</p>
  <p>Öppna i åtgärder för försäljningsinsikter = Inte startat i Salesforce.</p>
  <p>Slutför i åtgärder för försäljningsinsikter = Slutfört i Salesforce.</p>
  <p>De andra statusvärdena i Salesforce kommer inte att synkroniseras med Sales Insight-åtgärder.</p></td>
 </tr>
 <tr>
  <td>Prioritet</td>
  <td>Prioritet</td>
  <td><p>Prioriteten för Sales Insight Actions kan vara Normal eller High, vilket mappar till värdena Normal och Hög prioritet i Salesforce.</p>
  <p>Värdet med låg prioritet i Salesforce synkroniseras inte med åtgärder för försäljningsinsikter.</p></td>
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

## Synkronisera åtgärder för försäljningsinsikter med Salesforce för första gången {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan Sales Insight-åtgärder och Salesforce-uppgifter importerar vi dina Salesforce-uppgifter. Vi kommer **inte** att föra över aktuella uppgifter som du har i Sales Insight Actions till Salesforce. För att minska oordning och dubbletter är de enda uppgifter som synkroniseras från Sales Insight Actions till Salesforce uppgifter som skapas *efter* att du synkroniserat Sales Insight-åtgärder med SFDC.

Det här händer när du synkroniserar Sales Insight-åtgärder och SFDC-åtgärder:

* När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

* Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till Sales Insight Actions. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

* Om synkronisering har aktiverats tidigare och du tar bort några uppgifter i SFDC, kommer allt som har tagits bort de senaste 15 dagarna att tas bort från kommandocentralen.

* Vi synkroniserar kontinuerligt uppgifter mellan Sales Insight Actions och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter som du skapar, redigerar, slutför eller tar bort i Sales Insight-åtgärder att synkroniseras med din uppgiftslista i Salesforce. Och allt som har skapats, redigerats, slutförts eller tagits bort i Salesforce kommer att uppdatera din uppgiftslista i Sales Insight-åtgärder.

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på [inställningssidan](https://toutapp.com/login) i webbprogrammet.

>[!NOTE]
>
>Ämnesfältet för en aktivitet kan uppdateras i Sales Insight-åtgärder och den uppdateringen synkroniseras i Salesforce-ämnesfältet för motsvarande synkroniserade uppgift, om du använder det `{{activity_subject}}` dynamiska fältet i dina [inställningar för anpassning av aktivitetsinformation](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Omvänt kommer alla uppdateringar som görs i ämnesfältet i Salesforce _inte_ att synkroniseras till ämnesfältet för Sales Insight Actions-påminnelseaktiviteten.
