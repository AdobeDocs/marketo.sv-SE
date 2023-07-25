---
unique-page-id: 1147154
description: Synkronisera en SFDC-kampanj med ett program - Marketo Docs - produktdokumentation
title: Synkronisera en SFDC-kampanj med ett program
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Synkronisera en SFDC-kampanj med ett program {#sync-an-sfdc-campaign-with-a-program}

Med Marketo kan ni synkronisera era program med Salesforce-kampanjer för att behålla samma lista över personer i båda systemen, inklusive deras status. Kom så börjar vi!

>[!PREREQUISITES]
>
>Du måste [aktivera Salesforce-kampanjsynkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) först.

>[!CAUTION]
>
>När en SFDC-kampanj synkroniseras med ett Marketo-program inaktiveras de underliggande SFDC-åtgärderna (t.ex. lägg till i SFDC Campaign, Synkronisera till SFDC) för programmets underordnade kampanjer.

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Välj program.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicka **Programåtgärder** väljer **Salesforce Campaign-synkronisering**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Välj **Skapa nytt** eller välj en befintlig Salesforce-kampanj.

   >[!TIP]
   >
   >Om du väljer en befintlig Salesforce-kampanj ska du se till att [matchar programstatusvärdena för Salesforce-kampanjen och Marketo-programmet](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Ange ett namn för den nya kampanjen och klicka på **Spara**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Nu kan du verifiera kampanjsynkroniseringsinformationen på programsammanfattningssidan.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Underbar! Nu synkroniseras alla programstatusändringar i Marketo till SFDC-kampanjen och vice versa.
