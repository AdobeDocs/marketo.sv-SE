---
unique-page-id: 7513680
description: Automatisera en varning för Möjliga dubbletter av människor - Marketo Docs - Produktdokumentation
title: Automatisera en avisering om möjliga dubbletter av personer
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatisera en avisering om möjliga dubbletter av personer {#automate-an-alert-for-possible-duplicate-people}

Vill du få en varning varje gång en dubblettperson skapas? Så här konfigurerar du en smart kampanj för att göra det.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. [Skapa en ny smart kampanj](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md). Definiera följande smarta lista:

   * Utlösare: **Personen är skapad**
   * Filter: **Dubblettfält. **Fältnamnet **är** **fullständigt namn**.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Var kreativ. Experimentera med olika fält för att få bättre filtreringsresultat.

1. I flödessteget väljer du åtgärden [Skicka varningsflöde](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Använda [skicka aviseringsinformation-token](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) för att inkludera en länk till personen i CRM.

   >[!CAUTION]
   >
   >Om du importerar en stor lista kan du få en mängd av de här varningarna på en gång!
   >
   >
   >Två personer med samma namn betyder inte heller automatiskt att de är samma person.

1. Aktivera kampanjen på fliken **Schema** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Så ja! Den här smarta kampanjen utlöses varje gång en ny person med ett befintligt fullständigt namn skapas i Marketo.

>[!MORELIKETHIS]
>
>* [Sök och sammanfoga duplicerade personer](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

