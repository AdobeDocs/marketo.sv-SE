---
unique-page-id: 1146995
description: Använd token i flödessteg - Marketo Docs - produktdokumentation
title: Använd token i flödessteg
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Använd token i flödessteg {#use-tokens-in-flow-steps}

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

>[!PREREQUISITES]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

En variabel är en variabel. Ni använder det i e-postmeddelanden, landningssidor och smarta kampanjer för att göra livet enklare. Du kan använda [Mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (anpassade tokens) i flödessteg, webbhooks, e-post och landningssidor. Du kan använda variabler för att inkludera variabelt innehåll i dessa flödessteg:

* Ändra datavärde
* Ändra medlemsuppgifter för program
* Intressant stund
* Salesforce-kampanjsteg (lägg till, ta bort, ändra status)
* Skapa uppgift
* Skicka avisering (endast i utlösarkampanjer)

1. I flödessteget börjar du skriva `{{` för att hämta tokategorier. ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Se [Översikt över token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) för en lista över flera tillgängliga token.

1. Fortsätt skriva tills du hittar den variabel du vill ha och klicka för att välja.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Flera variabler kan användas i stegen Intressant stund, Skapa uppgift och Skicka avisering.

   >[!NOTE]
   >
   >Anpassade fälttoken för programmedlem kan användas i: Skapa aktivitet, Skapa aktivitet i Microsoft, Intressanta ögonblick, Ändra datavärdesåtgärder och Webhooks.

   Häftig! Data hämtas från token när den smarta kampanjen körs.

   >[!MORELIKETHIS]
   >
   >* [Hantera mina token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Förstå mina token i ett program](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

