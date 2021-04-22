---
unique-page-id: 1147031
description: Ta bort person från SFDC - Marketo Docs - produktdokumentation
title: Ta bort person från SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Ta bort person från SFDC {#delete-person-from-sfdc}

Om du behöver ta bort en viss uppsättning leads från Salesforce men låta dem vara personer i Marketo kan du använda åtgärden Ta bort person från SFDC-flöde.

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Klicka i databasen på den person som du vill ta bort från Salesforce. Klicka sedan på **Personåtgärder** och välj **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Välj **Ta bort person från SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Kontrollera att inställningen **Ta bort i Marketo** är **false** och klicka sedan på **Kör nu**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   När flödessteget har körts är din person inte längre en lead i Salesforce, men den stannar kvar i Marketo.

   >[!CAUTION]
   >
   >Om du anger **Ta bort i Marketo** till **true** och tar bort personer från Marketo och leads från Salesforce är de borta för alltid. Det här kan inte ångras.
