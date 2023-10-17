---
unique-page-id: 1147031
description: Ta bort person från SFDC - Marketo Docs - produktdokumentation
title: Ta bort person från SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Ta bort person från SFDC {#delete-person-from-sfdc}

Om du behöver ta bort en viss uppsättning leads från Salesforce men låta dem vara personer i Marketo Engage kan du använda åtgärden Ta bort person från SFDC-flöde.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Klicka i databasen på den person som du vill ta bort från Salesforce. Klicka sedan på **[!UICONTROL Person Actions]** och markera **[!DNL Salesforce]**.

   ![](assets/person-actions-salesforce.png)

1. Välj **[!UICONTROL Delete Person from SFDC]**.

   ![](assets/delete-person-from-sfdc.png)

1. Se till att **[!UICONTROL Delete in Marketo]** inställningen är **[!UICONTROL false]** och sedan klicka **[!UICONTROL Run Now]**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   När flödessteget har körts är din person inte längre en lead i Salesforce, men den stannar kvar i Marketo.

   >[!CAUTION]
   >
   >Om du anger **[!UICONTROL Delete in Marketo]** till **[!UICONTROL true]** och ta bort personer från Marketo och leads från Salesforce är de borta för evigt. Det här kan inte ångras.
