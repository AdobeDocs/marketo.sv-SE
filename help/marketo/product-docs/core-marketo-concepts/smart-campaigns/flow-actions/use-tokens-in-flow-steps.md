---
unique-page-id: 1146995
description: Använd token i flödessteg - Marketo Docs - produktdokumentation
title: Använd token i flödessteg
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Använd token i flödessteg {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

En variabel är en variabel. Ni använder det i e-postmeddelanden, landningssidor och smarta kampanjer för att göra livet enklare. Du kan använda [Mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (anpassade tokens) i flödessteg, webbhocker, e-post och landningssidor. Du kan använda variabler för att inkludera variabelt innehåll i dessa flödessteg:

* Ändra datavärde
* Ändra medlemsuppgifter för program
* Intressant stund
* Salesforce-kampanjsteg (lägg till, ta bort, ändra status)
* Skapa uppgift
* Skicka avisering (endast i utlösarkampanjer)

1. I flödessteget börjar du skriva `{{` för att hämta tokategorier.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Gå till [Översikt över token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} om du vill se en lista över flera tillgängliga token.

1. Fortsätt skriva tills du hittar den variabel du vill ha och klicka för att välja.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >Flera variabler kan användas i stegen Intressant stund, Skapa uppgift och Skicka avisering.

   >[!NOTE]
   >
   >Token för anpassade fält för programmedlemmar kan användas i: Skapa aktivitet, Skapa aktivitet i Microsoft, Intressanta stunder, Ändra dataflödesåtgärder och Webhooks.

   Häftig! Data hämtas från token när Smart Campaign körs.

   >[!MORELIKETHIS]
   >
   >* [Hantera mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Förstå mina token i ett program](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
