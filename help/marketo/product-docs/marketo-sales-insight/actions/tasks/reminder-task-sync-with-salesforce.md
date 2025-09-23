---
description: Synkronisera påminnelseuppgifter med Salesforce - Marketo Docs - produktdokumentation
title: Synkronisera påminnelseuppgifter med Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Synkronisering av påminnelseaktivitet med [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Om du vill lära dig hur du aktiverar aktivitetssynkronisering kan du checka ut [Synkronisera åtgärder för försäljningsinformation/påminnelser till Salesforce-aktiviteter](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

När inställningarna för uppgiftssynkronisering är aktiverade kommer användare att se sina påminnelseaktiviteter dubbelsynkroniserade med [!DNL Salesforce]. Det innebär att användare kan hantera uppgifter från antingen [!DNL Salesforce] eller [!DNL Sales Insight Actions] och känna sig säkra på att systemen är anpassade efter varandra.

## Synkronisering av påminnelseaktivitetsfält {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nedan visas en lista över påminnelseaktivitetsfälten i [!DNL Sales Insight Actions] och deras motsvarande [!DNL Salesforce]-fält som stöds via dubbelriktad uppgiftssynkronisering.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Uppgiftsfält</th>
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
  <td><p>Visar aktivitetens status. [!DNL Sales Insight Actions] aktiviteter har två statusvärden som är mappade till två av värdena i listan [!DNL Salesforce] med uppgiftsstatus.</p>
  <p>Öppna i [!DNL Sales Insight Actions] = Inte startat i [!DNL Salesforce].</p>
  <p>Slutförd i [!DNL Sales Insight Actions] = Slutförd i [!DNL Salesforce].</p>
  <p>De andra statusvärdena i [!DNL Salesforce] synkroniseras inte till [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Insight Actions] prioriteten kan vara Normal eller Hög, vilket mappar till värdena Normal och Hög prioritet i [!DNL Salesforce].</p>
  <p>Värdet för låg prioritet i [!DNL Salesforce] synkroniseras inte till [!DNL Sales Insight Actions].</p></td>
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

## Synkroniserar [!DNL Sales Insight Actions] aktiviteter med [!DNL Salesforce] för första gången {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan [!DNL Sales Insight Actions] och [!DNL Salesforce] aktiviteter importerar vi dina [!DNL Salesforce]-aktiviteter. Vi kommer **inte** att föra över aktuella uppgifter som du har i [!DNL Sales Insight Actions] till [!DNL Salesforce]. För att undvika rörighet och dubbletter är de enda uppgifter som synkroniseras från [!DNL Sales Insight Actions] till [!DNL Salesforce] uppgifter som skapas *efter* att du har synkroniserat [!DNL Sales Insight Actions] med SFDC.

Det här händer när du synkroniserar [!DNL Sales Insight Actions]- och SFDC-uppgifter:

* När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

* Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till [!DNL Sales Insight Actions]. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

* Om synkronisering har aktiverats tidigare och du tar bort åtgärder i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

* Vi synkroniserar uppgifter mellan [!DNL Sales Insight Actions] och SFDC hela tiden så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i [!DNL Sales Insight Actions] att synkroniseras till din uppgiftslista i [!DNL Salesforce]. Och allt som har skapats, redigerats, slutförts eller tagits bort i [!DNL Salesforce] kommer att uppdatera din uppgiftslista i [!DNL Sales Insight Actions].

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på [inställningssidan](https://toutapp.com/login) i webbprogrammet.

>[!NOTE]
>
>Ämnesfältet för en aktivitet kan uppdateras i [!DNL Sales Insight Actions] och den uppdateringen synkroniseras i ämnesfältet [!DNL Salesforce] för motsvarande synkroniserade uppgift, om du använder det dynamiska fältet `{{activity_subject}}` i inställningarna för anpassning av [ aktivitetsinformation ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) . Omvänt synkroniseras alla uppdateringar som görs i ämnesfältet i [!DNL Salesforce] *inte* till ämnesfältet [!DNL Sales Insight Actions] för påminnelseaktiviteten.
