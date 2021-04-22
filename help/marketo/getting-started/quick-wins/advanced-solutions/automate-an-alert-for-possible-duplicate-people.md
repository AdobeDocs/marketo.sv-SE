---
unique-page-id: 7513680
description: Automatisera en avisering om möjliga dubbletter av människor - Marketo Docs - produktdokumentation
title: Automatisera en avisering om möjliga dubbletter av personer
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatisera en varning för möjliga dubblettpersoner {#automate-an-alert-for-possible-duplicate-people}

Vill du få en varning varje gång en dubblettperson skapas? Så här konfigurerar du en smart kampanj för att göra det.

1. [Skapa en ny smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md). Definiera följande smarta lista:

* Utlösare: **Personen är skapad**
* Filter: **Duplicera fält.** Fältnamnet  **är fullständigt namn**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Var kreativ. Experimentera med olika fält för att få bättre filtreringsresultat.

1. Välj flödesåtgärden [Skicka varning](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) i flödessteget.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Använd [Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) för att inkludera en länk till personen i CRM.

   >[!CAUTION]
   >
   >Om du importerar en stor lista kan du få en mängd av de här varningarna på en gång!
   >
   >Två personer med samma namn betyder inte heller automatiskt att de är samma person.

1. Aktivera kampanjen på fliken **Schedule**.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Så ja! Den här smarta kampanjen utlöses varje gång en ny person med ett befintligt fullständigt namn skapas i Marketo.

>[!MORELIKETHIS]
>
>[Sök och sammanfoga duplicerade personer](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
