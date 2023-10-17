---
unique-page-id: 1147034
description: Lägg till i SFDC-kampanj - Marketo Docs - produktdokumentation
title: Lägg till i SFDC-kampanj
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Lägg till i SFDC-kampanj {#add-to-sfdc-campaign}

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

## Översikt {#overview}

Det här flödessteget kan användas i Marketo-kampanjer eller som ett enda flödessteg för att lägga till personer som leads i en Salesforce-kampanj. Om leadet ännu inte finns i Salesforce synkroniseras det automatiskt och läggs till i kampanjen med den angivna statusen.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Användning {#usage}

1. Hitta och välj den Salesforce-kampanj som du vill lägga till dina leads i.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Om du inte kan se en Salesforce-kampanj i kampanjlistan:
   >
   >  1. Se till att [kampanjsynkronisering är aktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Bekräfta att [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} is a [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} i Salesforce.

   >[!TIP]
   >
   >Du kan använda Salesforce-kampanj [Mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} för att göra programkloningen enklare.

1. Välj den Salesforce-kampanjmedlemskapsstatus som du vill tilldela leads när de läggs till.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Om en person redan är huvudmedlem i Salesforce-kampanjen hoppas de över och deras status uppdateras INTE. Du kan använda [ändra deras status i en SFDC-kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"} i stället.
