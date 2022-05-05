---
description: Steg 3 av 3 - Connect Marketo Engage och Veeva CRM - Marketo Docs - produktdokumentation
title: Steg 3 av 3 - Connect Marketo Engage och Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Steg 3 av 3: Connect Marketo Engage och Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

I den här artikeln konfigurerar du Marketo Engage att synkronisera med din konfigurerade Veeva CRM-instans. **Salesforce visas i några av popup-fönstren** som Veeva CRM bygger på Salesforce-plattformen.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}
>* [Steg 2 av 3: Skapa en veeva-användare för Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target=&quot;_blank&quot;}


>[!IMPORTANT]
>
>Endast en Marketo-instans i taget kan anslutas till en Veeva CRM-instans.

## Anslut till Veeva CRM med OAuth {#connect-to-veeva-crm-using-oauth}

1. I Marketo klickar du på **Administratör**. Välj **CRM** och klicka **Synkronisera med veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Se till att [dölj alla fält som du inte behöver](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target=&quot;_blank&quot;} i Marketo från synkroniseringsanvändaren innan du klickar på Synkronisera fält. När du klickar på Synkronisera fält skapas alla fält som användaren kan se i Marketo permanent och kan inte tas bort.

1. Klicka **Logga in med Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Markera Sandbox om du synkroniserar en Marketo-sandlåda till en Veeva CRM-sandlåda.

1. Klicka **Bekräfta autentiseringsuppgifter**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Ett popup-fönster med Salesforce-inloggningssidan visas. Ange dina inloggningsuppgifter för Marketo Sync User och klicka på **Logga in**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Ange verifieringskoden som du fick via e-post (skickas av Salesforce) och klicka på **Verifiera**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. När verifieringen är klar visas åtkomstsidan och begär åtkomst. Klicka **Tillåt**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. Om några minuter visas ett popup-fönster i Marketo Engine. Klicka **Bekräfta autentiseringsuppgifter**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Starta veeva-synkronisering {#start-veeva-sync}

1. Klicka **Starta veeva-synkronisering** för att påbörja den beständiga synkroniseringen av Marketo-Veeva CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Veeva CRM-synkronisering eller när du anger leads manuellt.

1. Klicka **Starta synkronisering**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Tiden det tar att slutföra den inledande synkroniseringen varierar beroende på databasens storlek och komplexitet.

## Verifiera synkronisering {#verify-sync}

Marketo tillhandahåller statusmeddelanden för Veeva CRM-synkronisering i administratörsområdet. Du kan kontrollera att synkroniseringen fungerar som den ska genom att följa dessa steg.

1. I Marketo klickar du på **Administratör** sedan **Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Synkroniseringsstatusen visas i det övre högra hörnet. Den visar ett av tre meddelanden: Senaste synkronisering, synkronisering pågår eller misslyckades.

>[!MORELIKETHIS]
>
>[Konfigurera anpassade objekt](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}
