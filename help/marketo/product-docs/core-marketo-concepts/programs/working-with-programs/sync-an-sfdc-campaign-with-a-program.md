---
unique-page-id: 1147154
description: Synkronisera en SFDC-kampanj med ett program - Marketo Docs - Produktdokumentation
title: Synkronisera en SFDC-kampanj med ett program
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Synkronisera en SFDC-kampanj med ett program {#sync-an-sfdc-campaign-with-a-program}

Med Marketo kan ni synkronisera program med Salesforce-kampanjer för att behålla samma lista över personer i båda systemen, inklusive deras status. Kom så börjar vi!

>[!PREREQUISITES]
>
>Du måste [aktivera Salesforce-kampanjsynkronisering](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) först.

>[!CAUTION]
>
>När en SFDC-kampanj synkroniseras med ett Marketo-program inaktiveras de implicita SFDC-åtgärderna (t.ex. lägg till i SFDC Campaign, Synkronisera till SFDC) för underordnade kampanjer i programmet.

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Välj program.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicka på **Programåtgärder** och välj sedan **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Välj **Skapa ny **eller välj en befintlig Salesforce-kampanj.

   >[!TIP]
   >
   >Om du väljer en befintlig Salesforce-kampanj måste du se till att [matcha programstatusvärdena för Salesforce-kampanjen och Marketo-programmet](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Ange ett namn för den nya kampanjen och klicka på **Spara**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Nu kan du verifiera kampanjsynkroniseringsinformationen på programsammanfattningssidan.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Underbar! Nu synkroniseras alla ändringar av programstatus i Marketo till SFDC-kampanjen och vice versa.

