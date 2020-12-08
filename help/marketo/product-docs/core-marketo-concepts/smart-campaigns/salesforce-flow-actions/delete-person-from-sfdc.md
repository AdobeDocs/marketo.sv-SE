---
unique-page-id: 1147031
description: Ta bort person från SFDC - Marketo Docs - Produktdokumentation
title: Ta bort person från SFDC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Ta bort person från SFDC {#delete-person-from-sfdc}

Om du behöver ta bort en viss uppsättning leads från Salesforce men låta dem vara personer i Marketo, kan du använda åtgärden Ta bort person från SFDC-flöde.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Endast tillgängligt när det är integrerat med Salesforce.

1. Klicka i databasen på den person som du vill ta bort från Salesforce. Klicka sedan på **Personåtgärder** och välj **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Välj **Ta bort person från SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Kontrollera att inställningen **Ta bort i Marketo** är **false** och klicka sedan på **Kör nu**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   När flödessteget har körts blir din person inte längre en lead i Salesforce, men den blir kvar i Marketo.

   >[!CAUTION]
   >
   >Om du anger **Ta bort i Marketo** till **true** och tar bort personer från Marketo och leads från Salesforce är de borta för alltid. Det här kan inte ångras.

