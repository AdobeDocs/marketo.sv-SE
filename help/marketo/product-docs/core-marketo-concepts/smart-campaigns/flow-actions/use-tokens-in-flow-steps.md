---
unique-page-id: 1146995
description: Använd token i flödessteg - Marketo Docs - Produktdokumentation
title: Använd token i flödessteg
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Använd token i flödessteg {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [Lägg till ett flödessteg i en smart kampanj](add-a-flow-step-to-a-smart-campaign.md)


En variabel är en variabel. Ni använder det i [e-postmeddelanden](https://docs.marketo.com/pages/viewpage.action?pageId=557076), [landningssidor](https://docs.marketo.com/pages/viewpage.action?pageId=2359689)och [smarta kampanjer](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) för att göra livet enklare. Du kan använda [Mina token](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (anpassade tokens) i flödessteg, på webbhocker, i e-postmeddelanden och på landningssidor.  Du kan använda variabler för att inkludera variabelt innehåll i dessa flödessteg:

* Ändra datavärde
* Intressant stund
* Salesforce-kampanjsteg (lägg till, ta bort, ändra status)
* Skapa uppgift
* Skicka avisering (endast i utlösarkampanjer)

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Börja skriva i flödessteget `{{` för att hämta tokategorier. ![](assets/image2014-9-22-14-3a3-3a17.png)>

   >[!NOTE]
   >
   >**Djupdykning**
   >
   >Se [Token Overview](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) för en lista över flera tillgängliga tokens.

1. Fortsätt skriva tills du hittar den variabel du vill ha och klicka för att välja.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Flera variabler kan användas i stegen Intressant stund, Skapa uppgift och Skicka avisering.

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >* [Hantera mina token](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Förstå mina token i ett program](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


Häftig! Data hämtas från token när den smarta kampanjen körs.