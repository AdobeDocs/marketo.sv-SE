---
unique-page-id: 7513680
description: Automatisera en varning för Möjliga dubbletter av människor - Marketo Docs - Produktdokumentation
title: Automatisera en avisering om möjliga dubbletter av personer
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Automatisera en avisering om möjliga dubbletter av personer {#automate-an-alert-for-possible-duplicate-people}

Vill du få en varning varje gång en dubblettperson skapas? Så här konfigurerar du en smart kampanj för att göra det.

1. [Skapa en ny smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md). Definiera följande smarta lista:

* Utlösare: **Personen är skapad**
* Filter: **Duplicera fält.** Fältnamnet **är fullständigt namn**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Var kreativ. Experimentera med olika fält för att få bättre filtreringsresultat.

1. I flödessteget väljer du åtgärden [Skicka varningsflöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Använda [skicka aviseringsinformation-token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) för att inkludera en länk till personen i CRM.

   >[!CAUTION]
   >
   >Om du importerar en stor lista kan du få en mängd av de här varningarna på en gång!
   >
   >Två personer med samma namn betyder inte heller automatiskt att de är samma person.

1. Aktivera kampanjen på fliken **Schema** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Så ja! Den här smarta kampanjen utlöses varje gång en ny person med ett befintligt fullständigt namn skapas i Marketo.

>[!MORELIKETHIS]
>
>[Sök och sammanfoga duplicerade personer](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
