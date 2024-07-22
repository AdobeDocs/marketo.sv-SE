---
unique-page-id: 1147154
description: Synkronisera en SFDC-kampanj med ett program - Marketo Docs - produktdokumentation
title: Synkronisera en SFDC-kampanj med ett program
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---

# Synkronisera en SFDC-kampanj med ett program {#sync-an-sfdc-campaign-with-a-program}

Med Marketo Engage kan du synkronisera dina program med [!DNL Salesforce] kampanjer för att behålla samma lista över personer i båda systemen, inklusive deras status. Kom så börjar vi!

>[!PREREQUISITES]
>
>Du måste [aktivera [!DNL Salesforce] kampanjsynkronisering](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"} först.

>[!CAUTION]
>
>När du synkroniserar en SFDC-kampanj med ett Marketo Engage-program inaktiveras de underliggande SFDC-åtgärderna (t.ex. lägg till i SFDC Campaign, Synkronisera med SFDC) för underordnade kampanjer i programmet.

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-1.png)

1. Välj program.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicka på **[!UICONTROL Program Actions]** och välj sedan **[!UICONTROL Salesforce Campaign Sync]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Välj **[!UICONTROL Create New]** eller välj en befintlig [!DNL Salesforce]-kampanj.

   >[!TIP]
   >
   >Om du väljer en befintlig [!DNL Salesforce]-kampanj måste du [matcha programstatusvärdena för  [!DNL Salesforce] kampanjen och Marketo-programmet](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Ange ett namn för den nya kampanjen och klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Nu kan du verifiera kampanjsynkroniseringsinformationen på programsammanfattningssidan.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Underbar! Nu synkroniseras alla programstatusändringar i Marketo till SFDC-kampanjen och vice versa.
