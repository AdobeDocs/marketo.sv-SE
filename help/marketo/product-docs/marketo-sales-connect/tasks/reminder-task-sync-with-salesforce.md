---
description: Synkronisera påminnelseuppgifter med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisera påminnelseuppgifter med Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Synkronisering av påminnelseaktivitet med [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Om du vill veta mer om hur du aktiverar aktivitetssynkronisering kan du checka ut [Synkronisera [!DNL Sales Connect] Aktiviteter/påminnelser till [!DNL Salesforce] Aktiviteter](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

När inställningarna för uppgiftssynkronisering är aktiverade kommer användare att se sina påminnelseaktiviteter dubbelsynkroniserade med [!DNL Salesforce]. Det innebär att användare kan hantera uppgifter från antingen [!DNL Salesforce] eller [!DNL Sales Connect] och känna sig säkra på att systemen är anpassade efter varandra.

## Synkronisering av påminnelseaktivitetsfält {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nedan visas en lista över påminnelseaktivitetsfälten i [!DNL Sales Connect] och deras motsvarande [!DNL Salesforce]-fält som stöds via dubbelriktad uppgiftssynkronisering.

<table>
 <tr>
  <th>[!DNL Sales Connect] Uppgiftsfält</th>
  <th>[!DNL Salesforce] Uppgiftsfält</th>
  <th>[!DNL Salesforce] Uppgift</th>
 </tr>
 <tr>
  <td>[!UICONTROL Task Name]</td>
  <td>[!UICONTROL Subject Field]</td>
  <td>Ett kort sammanfattningsfält som ska visa aktivitetens titel.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Task Status]</td>
  <td><p>Visar aktivitetens status. [!DNL Sales Connect] aktiviteter har två statusvärden som är mappade till två av värdena i listan [!DNL Salesforce] med uppgiftsstatus.</p>
  <p>Öppna i [!DNL Sales Connect] = Inte startat i [!DNL Salesforce].</p>
  <p>Slutförd i [!DNL Sales Connect] = Slutförd i [!DNL Salesforce].</p>
  <p>De andra statusvärdena i [!DNL Salesforce] synkroniseras inte till [!DNL Sales Connect].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Connect] prioriteten kan vara Normal eller Hög, vilket mappar till värdena Normal och Hög prioritet i [!DNL Salesforce].</p>
  <p>Värdet för låg prioritet i [!DNL Salesforce] synkroniseras inte till [!DNL Sales Connect].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Due Date]</td>
  <td>[!UICONTROL Due Date]</td>
  <td>Datumet då uppgiften förfaller.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Comments]</td>
  <td>Visar mer detaljerad information om vad som var tänkt att slutföras med påminnelseaktiviteten.</td>
 </tr>
</table>

## Synkroniserar [!DNL Sales Connect] aktiviteter med [!DNL Salesforce] för första gången {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan [!DNL Sales Connect] och [!DNL Salesforce] aktiviteter importerar vi dina [!DNL Salesforce]-aktiviteter. Vi kommer **inte** att föra över aktuella uppgifter som du har i [!DNL Sales Connect] till [!DNL Salesforce]. För att undvika rörighet och dubbletter är de enda uppgifter som synkroniseras från [!DNL Sales Connect] till [!DNL Salesforce] uppgifter som skapas *efter* att du har synkroniserat [!DNL Sales Connect] med SFDC.

Det här händer när du synkroniserar [!DNL Sales Connect]- och SFDC-uppgifter:

* När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

* Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till [!DNL Sales Connect]. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

* Om synkronisering har aktiverats tidigare och du tar bort åtgärder i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

* Vi synkroniserar uppgifter mellan [!DNL Sales Connect] och SFDC hela tiden så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i [!DNL Sales Connect] att synkroniseras till din uppgiftslista i [!DNL Salesforce]. Och allt som har skapats, redigerats, slutförts eller tagits bort i [!DNL Salesforce] kommer att uppdatera din uppgiftslista i [!DNL Sales Connect].

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på [inställningssidan](https://toutapp.com/login) i webbprogrammet.

>[!NOTE]
>
>Ämnesfältet för en aktivitet kan uppdateras i [!DNL Sales Connect] och den uppdateringen synkroniseras i ämnesfältet [!DNL Salesforce] för motsvarande synkroniserade uppgift, om du använder det dynamiska fältet `{{activity_subject}}` i inställningarna för anpassning av [ aktivitetsinformation ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) . Omvänt synkroniseras alla uppdateringar som görs i ämnesfältet i [!DNL Salesforce] *inte* till ämnesfältet [!DNL Sales Connect] för påminnelseaktiviteten.
