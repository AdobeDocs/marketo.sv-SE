---
unique-page-id: 1147031
description: Ta bort person från SFDC - Marketo Docs - produktdokumentation
title: Ta bort person från SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Ta bort person från SFDC {#delete-person-from-sfdc}

Om du behöver ta bort en viss uppsättning leads från Salesforce men låta dem vara personer i Marketo Engage kan du använda åtgärden Ta bort person från SFDC-flöde.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Klicka i databasen på den person som du vill ta bort från Salesforce. Klicka sedan på **[!UICONTROL Person Actions]** och välj **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Välj **[!UICONTROL Delete Person from SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Kontrollera att inställningen **[!UICONTROL Delete in Marketo]** är **[!UICONTROL false]** och klicka sedan på **[!UICONTROL Run Now]**.

   ![](assets/delete-person-from-sfdc-3.png)

   När flödessteget har körts är din person inte längre en lead i Salesforce, men den stannar kvar i Marketo.

   >[!CAUTION]
   >
   >Om du anger **[!UICONTROL Delete in Marketo]** som **[!UICONTROL true]** och tar bort personer från Marketo och leads från Salesforce är de borta för alltid. Det här kan inte ångras.
