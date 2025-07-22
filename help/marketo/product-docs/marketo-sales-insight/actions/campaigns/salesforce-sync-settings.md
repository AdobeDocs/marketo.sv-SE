---
description: Salesforce Sync Settings - Marketo Docs - produktdokumentation
title: Salesforce Sync Settings
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# [!DNL Salesforce] Synkronisera inställningar {#salesforce-sync-settings}

## Loggar e-postaktivitet till [!DNL Salesforce] via API {#logging-email-activity-to-salesforce-via-api}

Den här funktionen kräver att du finns i Enterprise/Unlimited Edition av [!DNL Salesforce] eller Professional Edition om du har köpt Integration via Web Services API.

>[!PREREQUISITES]
>
>[!DNL Salesforce] och [!DNL Sales Insight Actions] måste vara anslutna.

1. Klicka på kugghjulsikonen i [!DNL Sales Insight Actions] och välj **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-1.png)

1. Klicka på [!UICONTROL Admin Settings] under [!UICONTROL My Account] (eller **[!UICONTROL Salesforce]** om du inte är administratör).

   ![](assets/salesforce-sync-settings-2.png)

1. Klicka på fliken **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Klicka på pilen bredvid [!UICONTROL Log Email Activity] till [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Klicka på fliken **[!UICONTROL Salesforce API]**. På det här kortet kan du ange din inställning för loggningsinformation till [!DNL Salesforce]. Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/salesforce-sync-settings-5.png)

## Loggar e-postaktivitet till [!DNL Salesforce] via e-post till [!DNL Salesforce] (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

När du har aktiverat [!UICONTROL Email to Salesforce (BCC)] får du en kopia av dina säljmeddelanden och dina e-postmeddelanden loggas som aktiviteter på affärsmöjligheter, leads och kontakter.

>[!PREREQUISITES]
>
>[!DNL Salesforce] och [!DNL Sales Insight Actions] måste vara anslutna.

**Logga in dina e-postmeddelanden i [!DNL Salesforce] via e-post (BCC)**

1. I Marketo Sales klickar du på kugghjulsikonen och väljer **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-6.png)

1. Klicka på [!UICONTROL Admin Settings] under [!UICONTROL My Account] (eller **[!UICONTROL Salesforce]** om du inte är administratör).

   ![](assets/salesforce-sync-settings-7.png)

1. Klicka på fliken **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Klicka på fliken **[!UICONTROL Email to Salesforce (BCC)]** och klicka på **[!UICONTROL Activate]**.

   ![](assets/salesforce-sync-settings-9.png)

Om din e-postadress till [!DNL Salesforce] av någon anledning inte kommer in följer du de här stegen för att aktivera funktionen Hemlig kopia i ditt [!DNL Salesforce]-konto:

1. Logga in på din [!DNL Salesforce]-instans.
1. Hitta ditt användarnamn i det övre högra hörnet och välj listrutan.
1. Välj **[!UICONTROL My Settings]**.
1. Välj **[!UICONTROL Email]**.
1. Välj **[!UICONTROL My Email to Salesforce]**.
1. På den här sidan visas ett fält med namnet [!UICONTROL Email to Salesforce Address]. Bläddra nedåt till [!UICONTROL My Acceptable Email Addresses] om inget fylls i bredvid det.
1. Ange den eller de e-postadresser som du vill ska kopieras.
1. Klicka på **[!UICONTROL Save Changes]**.

**Det går inte att hitta min e-postadress till [!DNL Salesforce] i Mina inställningar**

Om du inte ser Min e-post till [!DNL Salesforce] under dina inställningar har administratören kanske inte aktiverat den. Detta kan inträffa om ditt team inte har använt [!DNL Salesforce] tidigare eller om ditt team aldrig har använt den hemkontrolladress som [!DNL Salesforce] tillhandahåller.

>[!NOTE]
>
>Du måste ha administratörsbehörighet för att kunna konfigurera detta.

1. Klicka på **[!UICONTROL Setup]**.
1. Klicka på **[!UICONTROL Email Administration]**.
1. Klicka på **[!UICONTROL Email to Salesforce]**.
1. Klicka på **[!UICONTROL Edit]**.
1. Markera rutan bredvid&quot;Aktiv&quot;.
1. Klicka på **[!UICONTROL Save]**.

## Synkronisera [!DNL Sales Insight Actions] aktiviteter/påminnelser till [!DNL Salesforce] uppgifter {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Klicka på kugghjulsikonen i [!DNL Sales Insight Actions] och välj **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-10.png)

1. Klicka på [!UICONTROL Admin Settings] under [!UICONTROL My Account] (eller **[!UICONTROL Salesforce]** om du inte är administratör).

   ![](assets/salesforce-sync-settings-11.png)

1. Klicka på fliken **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Klicka på pilen bredvid Synkronisera Marketo säljaktiviteter/påminnelser till [!DNL Salesforce] aktiviteter.

   ![](assets/salesforce-sync-settings-13.png)

1. Välj önskat alternativ (&quot;Synkronisera inte till [!DNL Salesforce] uppgifter&quot; är valt som standard).

   ![](assets/salesforce-sync-settings-14.png)

## Synkroniserar [!DNL Sales Insight Actions] aktiviteter med [!DNL Salesforce] för första gången {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

När du först aktiverar synkroniseringen mellan [!DNL Sales Insight Actions] och [!DNL Salesforce] aktiviteter importerar vi dina [!DNL Salesforce]-aktiviteter. Vi kommer inte att föra över några aktuella uppgifter som du har i [!DNL Sales Insight Actions] till [!DNL Salesforce]. För att undvika rörighet och dubbletter är de enda uppgifter som synkroniseras från [!DNL Sales Insight Actions] till [!DNL Salesforce] uppgifter som skapas efter att du har synkroniserat [!DNL Sales Insight Actions] med SFDC.

Det här händer när du synkroniserar [!DNL Sales Insight Actions]- och SFDC-uppgifter:

När du klickar på Spara för uppgifter synkroniseras de om. Det här kommer att ta en stund från början.

Påminnelser som har uppdaterats eller skapats under de senaste 24 timmarna hämtas in från SFDC till [!DNL Sales Insight Actions]. Synkroniseringen baseras på förfallodatum och alla dessa uppgifter synkroniseras på baksidan, men i kommandocentralen visas endast uppgifter som förfaller idag och imorgon.

Om synkronisering har aktiverats tidigare och du tar bort åtgärder i SFDC, tas allt som har tagits bort de senaste 15 dagarna bort från kommandocentralen.

Vi synkroniserar kontinuerligt uppgifter mellan [!DNL Sales Insight Actions] och SFDC så länge synkroniseringen är aktiverad.

Efter den första synkroniseringen kommer alla uppgifter du skapar, redigerar, slutför eller tar bort i [!DNL Sales Insight Actions] att synkroniseras till din uppgiftslista i [!DNL Salesforce]. Och allt som har skapats, redigerats, slutförts eller tagits bort i [!DNL Salesforce] kommer att uppdatera din uppgiftslista i [!DNL Sales Insight Actions].

Om du vill aktivera den här synkroniseringen markerar du bara synkroniseringsrutan på [!UICONTROL Settings]-sidan i webbprogrammet.
