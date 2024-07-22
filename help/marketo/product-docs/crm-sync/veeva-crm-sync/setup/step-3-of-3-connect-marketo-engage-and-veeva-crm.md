---
description: Steg 3 av 3 - Connect Marketo Engage och Veeva CRM - Marketo Docs - produktdokumentation
title: Steg 3 av 3 - Connect Marketo Engage och Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 1%

---

# Steg 3 av 3: Connect Marketo Engage och Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

I den här artikeln konfigurerar du Marketo Engage att synkronisera med din konfigurerade Veeva CRM-instans. **Salesforce visas i vissa av popup-fönstren** när Veeva CRM är byggt på Salesforce-plattformen.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Steg 2 av 3: Skapa en veeva-användare för Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Endast en Marketo-instans i taget kan anslutas till en Veeva CRM-instans.

## Anslut till Veeva CRM med OAuth {#connect-to-veeva-crm-using-oauth}

1. Klicka på **[!UICONTROL Admin]** i Marketo. Markera **[!UICONTROL CRM]** och klicka på **[!UICONTROL Sync with Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >[Dölj alla fält som du inte behöver](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} i Marketo från synkroniseringsanvändaren innan du klickar på Synkronisera fält. När du klickar på Synkronisera fält skapas alla fält som användaren kan se i Marketo permanent och kan inte tas bort.

1. Klicka på **[!UICONTROL Login with Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Markera Sandbox om du synkroniserar en Marketo-sandlåda till en Veeva CRM-sandlåda.

1. Klicka på **[!UICONTROL Confirm Credentials]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Ett popup-fönster med Salesforce-inloggningssidan visas. Ange dina autentiseringsuppgifter för Marketo Sync-användare och klicka på **[!UICONTROL Log In]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Ange verifieringskoden som du fick via e-post (skickad av Salesforce) och klicka på **[!UICONTROL Verify]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. När verifieringen är klar visas åtkomstsidan och begär åtkomst. Klicka på **[!UICONTROL Allow]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. Om några minuter visas ett popup-fönster i Marketo Engine. Klicka på **[!UICONTROL Confirm Credentials]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Starta veeva-synkronisering {#start-veeva-sync}

1. Klicka på **[!UICONTROL Start Veeva Sync]** för att påbörja den beständiga Marketo-Veeva CRM-synkroniseringen.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en Veeva CRM-synkronisering eller när du anger leads manuellt.

1. Klicka på **[!UICONTROL Start Sync]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Tiden det tar att slutföra den inledande synkroniseringen varierar beroende på databasens storlek och komplexitet.

## Verifiera synkronisering {#verify-sync}

Marketo tillhandahåller statusmeddelanden för Veeva CRM-synkronisering i administratörsområdet. Du kan kontrollera att synkroniseringen fungerar som den ska genom att följa dessa steg.

1. I Marketo klickar du på **[!UICONTROL Admin]** och sedan på **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Synkroniseringsstatusen visas längst upp till höger. Det visar ett av tre meddelanden: Senaste synkronisering, Pågående synkronisering eller Misslyckades.

>[!MORELIKETHIS]
>
>[Konfigurera anpassade objekt](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
