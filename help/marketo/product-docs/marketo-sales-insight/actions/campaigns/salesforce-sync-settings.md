---
description: Salesforce Sync Settings - Marketo Docs - produktdokumentation
title: Synkroniseringsinställningar för Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 350490c93d8f2bcc278f9f3e82018a1db91a1146
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Synkroniseringsinställningar för Salesforce {#salesforce-sync-settings}

## Logga e-postaktivitet till Salesforce via API {#logging-email-activity-to-salesforce-via-api}

Den här funktionen kräver att du finns i Enterprise/Unlimited Edition av Salesforce eller Professional Edition om du har köpt Integration via Web Services API.

>[!PREREQUISITES]
>
>Salesforce- och Sales Insight-åtgärder måste vara kopplade.

1. I Sales Insight Actions klickar du på kugghjulsikonen och väljer **Inställningar**.

   ![](assets/salesforce-sync-settings-1.png)

1. Under Administratörsinställningar (eller &quot;Mitt konto&quot; om du inte är administratör) klickar du på **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. Klicka på **Synkronisera inställningar** -fliken.

   ![](assets/salesforce-sync-settings-3.png)

1. Klicka på pilen bredvid Logga e-postaktivitet till Salesforce.

   ![](assets/salesforce-sync-settings-4.png)

1. Klicka på **Salesforce API** -fliken. På det här kortet kan du ange din inställning för att logga information till Salesforce. Klicka **Spara** när det är klart.

   ![](assets/salesforce-sync-settings-5.png)

## Loggning av e-postaktivitet till Salesforce via e-post till Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

När du har aktiverat&quot;E-post till Salesforce (BCC)&quot; får du en kopia av dina säljmeddelanden och dina e-postmeddelanden loggas som aktiviteter på affärsmöjligheter, leads och kontakter.

>[!PREREQUISITES]
>
>Salesforce- och Sales Insight-åtgärder måste vara kopplade.

**Logga dina e-postmeddelanden i Salesforce via e-post (BCC)**

1. I Marketo Sales klickar du på kugghjulsikonen och väljer **Inställningar**.

   ![](assets/salesforce-sync-settings-6.png)

1. Under Administratörsinställningar (eller &quot;Mitt konto&quot; om du inte är administratör) klickar du på **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. Klicka på **Synkronisera inställningar** -fliken.

   ![](assets/salesforce-sync-settings-8.png)

1. Klicka på **E-post till Salesforce (BCC)** och klicka **Aktivera**.

   ![](assets/salesforce-sync-settings-9.png)

Om din e-postadress till Salesforce inte kommer in av någon anledning, följer du de här stegen för att aktivera funktionen Kontroll av webbläsarkompatibilitet i ditt Salesforce-konto:

1. Logga in på din Salesforce-instans.
1. Hitta ditt användarnamn i det övre högra hörnet och välj listrutan.
1. Välj **Mina inställningar**.
1. Välj **E-post**.
1. Välj **Min e-post till Salesforce**.
1. På den här sidan visas ett fält med namnet&quot;E-post till Salesforce-adress&quot;. Om inget fylls i bredvid det bläddrar du nedåt till&quot;Mina godkända e-postadresser&quot;.
1. Ange den eller de e-postadresser som du vill ska kopieras.
1. Klicka **Spara ändringar**.

**Det går inte att hitta min e-post till Salesforce i Mina inställningar**

Om du inte ser Min e-post till Salesforce under dina inställningar har administratören kanske inte aktiverat den. Det här kan hända om ditt team inte har använt Salesforce tidigare, eller om ditt team aldrig har använt den BCC-adress som Salesforce erbjuder.

>[!NOTE]
>
>Du måste ha administratörsbehörighet för att kunna konfigurera detta.

1. Klicka **Inställningar**.
1. Klicka **E-postadministration**.
1. Klicka **E-post till Salesforce**.
1. Klicka **Redigera**.
1. Markera rutan bredvid&quot;Aktiv&quot;.
1. Klicka **Spara**.

## Synkronisera uppgifter/påminnelser för försäljningsinsikter till Salesforce-uppgifter {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. I Sales Insight Actions klickar du på kugghjulsikonen och väljer **Inställningar**.

   ![](assets/salesforce-sync-settings-10.png)

1. Under Administratörsinställningar (eller &quot;Mitt konto&quot; om du inte är administratör) klickar du på **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. Klicka på **Synkronisera inställningar** -fliken.

   ![](assets/salesforce-sync-settings-12.png)

1. Klicka på pilen bredvid Synkronisera Marketo säljuppgifter/påminnelser till Salesforce-uppgifter.

   ![](assets/salesforce-sync-settings-13.png)

1. Välj önskat alternativ (&quot;Synkronisera inte till Salesforce-uppgifter&quot; är valt som standard).

   ![](assets/salesforce-sync-settings-14.png)

## Synkronisera åtgärder för försäljningsinsikter med Salesforce för första gången {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan Sales Insight-åtgärder och Salesforce-uppgifter importerar vi dina Salesforce-uppgifter. Vi kommer inte att föra över några aktuella uppgifter som du har i Sales Insight Actions till Salesforce. För att minska problem och dubbletter är de enda uppgifter som synkroniseras från Sales Insight Actions till Salesforce uppgifter som skapas efter att du har synkroniserat Sales Insight Actions med SFDC.

Det här händer när du synkroniserar Sales Insight-åtgärder och SFDC-åtgärder:

När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till Sales Insight Actions. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

Om synkronisering har aktiverats tidigare och du tar bort några uppgifter i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

Vi synkroniserar kontinuerligt uppgifter mellan Sales Insight Actions och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter som du skapar, redigerar, slutför eller tar bort i Sales Insight-åtgärder att synkroniseras med din uppgiftslista i Salesforce. Och allt som har skapats, redigerats, slutförts eller tagits bort i Salesforce kommer att uppdatera din uppgiftslista i Sales Insight-åtgärder.

Om du vill aktivera synkroniseringen markerar du bara synkroniseringsrutan på sidan Inställningar i webbprogrammet.
