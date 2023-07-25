---
unique-page-id: 1147031
description: Ta bort person från SFDC - Marketo Docs - produktdokumentation
title: Ta bort person från SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Ta bort person från SFDC {#delete-person-from-sfdc}

Om du behöver ta bort en viss uppsättning leads från Salesforce men låta dem vara personer i Marketo kan du använda åtgärden Ta bort person från SFDC-flöde.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Klicka i databasen på den person som du vill ta bort från Salesforce. Klicka sedan på **Personåtgärder** och markera **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Välj **Ta bort person från SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Se till att **Ta bort i Marketo** inställningen är **false** och sedan klicka **Kör nu**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   När flödessteget har körts är din person inte längre en lead i Salesforce, men den stannar kvar i Marketo.

   >[!CAUTION]
   >
   >Om du anger **Ta bort i Marketo** till **true** och ta bort personer från Marketo och leads från Salesforce är de borta för evigt. Det här kan inte ångras.
