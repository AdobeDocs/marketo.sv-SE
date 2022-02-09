---
description: Salesforce Sync Settings - Marketo Docs - produktdokumentation
title: Synkroniseringsinställningar för Salesforce
hide: true
hidefromtoc: true
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '443'
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
