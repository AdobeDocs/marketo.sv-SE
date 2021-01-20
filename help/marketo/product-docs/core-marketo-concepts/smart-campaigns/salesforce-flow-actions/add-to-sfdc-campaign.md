---
unique-page-id: 1147034
description: Lägg till i SFDC-kampanj - Marketo Docs - Produktdokumentation
title: Lägg till i SFDC-kampanj
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '0'
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
   >Om du inte kan se en Salesforce-kampanj i Campaign-listan:
   >
   >  1. Kontrollera att [kampanjsynkroniseringen är aktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Bekräfta att din [Marketo Sync-användare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) är en [marknadsföringsanvändare](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) i Salesforce.


   >[!TIP]
   >
   >Du kan använda Salesforce-kampanj [Mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) för att göra programkloningen enklare.

1. Välj den Salesforce-kampanjmedlemskapsstatus som du vill tilldela leads när de läggs till.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Om en person redan är huvudmedlem i Salesforce-kampanjen hoppas de över och deras status uppdateras INTE. Du kan använda [ändra deras status i en SFDC-kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) i stället.
