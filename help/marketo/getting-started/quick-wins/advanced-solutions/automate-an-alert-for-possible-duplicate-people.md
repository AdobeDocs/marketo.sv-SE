---
unique-page-id: 7513680
description: Automatisera en avisering om möjliga dubbletter av människor - Marketo Docs - produktdokumentation
title: Automatisera en avisering om möjliga dubbletter av personer
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 50fc46312d2c7c25556994fad4e118c01cf92fc0
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Automatisera en avisering om möjliga dubbletter av personer {#automate-an-alert-for-possible-duplicate-people}

Vill du få en varning varje gång en dubblettperson skapas? Så här konfigurerar du en smart kampanj för att göra det.

1. [Skapa en ny smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Definiera följande smarta lista:

* Utlösare: **Personen är skapad**
* Filter: **Duplicera fält.** Fältnamn **är fullständigt namn**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >Var kreativ. Experimentera med olika fält för att få bättre filtreringsresultat.

1. Välj [Skicka avisering](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target=&quot;_blank&quot;}-flödesåtgärd.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Använda [Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} om du vill inkludera en länk till personen i CRM.

   >[!CAUTION]
   >
   >Om du importerar en stor lista kan du få en mängd av de här varningarna på en gång!
   >
   >Två personer med samma namn betyder inte heller automatiskt att de är samma person.

1. Aktivera kampanjen i **Schema** -fliken.

   ![](assets/automate-an-alert-3.png)

Så ja! Den här smarta kampanjen utlöses varje gång en ny person med ett befintligt fullständigt namn skapas i Marketo.

>[!MORELIKETHIS]
>
>[Sök och sammanfoga duplicerade personer](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
