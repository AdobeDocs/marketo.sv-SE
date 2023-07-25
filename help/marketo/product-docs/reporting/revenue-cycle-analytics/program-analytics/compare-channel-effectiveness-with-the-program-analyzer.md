---
unique-page-id: 2360401
description: Jämför kanaleffektivitet med programanalys - Marketo Docs - produktdokumentation
title: Jämför kanaleffektiviteten med programanalysen
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Jämför kanaleffektiviteten med programanalysen {#compare-channel-effectiveness-with-the-program-analyzer}

Använd Program Analyzer för att jämföra kanalkostnader, medlemsförvärv, pipeline, intäkter med mera för att identifiera era mest effektiva kanaler.

>[!PREREQUISITES]
>
>[Skapa en programanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Klicka på **Analyser** in **Mina Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Välj **Program Analyzer**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Ändra vyn till **Efter kanal**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Använd **X-axel** för att välja ett mått för den vågräta axeln. Låt oss börja med **Programkostnad**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Använd listrutan Y-axel för att välja ett mått för den lodräta axeln. Här, vi följer med **(FT) Pipeline skapad**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Många av de mätvärden du kan välja i programanalysen är tillgängliga med beräkningar med första beröringen (FT) och multitouch (MT). Det är viktigt att förstå [skillnaden mellan FT- och MT-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Använd **Y-axel** välj **(MT) Pipeline skapad**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   I den här flerberöringsattribueringsvyn ser vi att webbseminariekanalen har större påverkan på den pipeline som skapas och mindre kostnader än kanalerna Tradeshow och Online Advertising.

   Nu ska vi lägga till ytterligare två dimensioner!

1. Använd **Bubbelstorlek** för att välja ytterligare ett mått, som **Nya namn**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Se hur diagrammet ändras.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vi ser att webbseminariekanalen krymper, mätt med **Nya namn**. Vi kan dra slutsatsen att även om den har många medlemmar är det mindre effektivt att generera nya leads än Tradeshow-kanalen.

1. Använd slutligen listrutan Färg för att lägga till den fjärde dimensionen. Låt oss välja **(FT) Vinstintäkter**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Se hur färgerna ändras i diagrammet.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Av färgerna har vi fått veta att Tradeshow-kanalen, den grönaste bubblan, har påverkat de största intäkterna, som mäts med första-beröringsattribuering.

1. Om vi ändrar färgens mått till **(MT) Intäkter, vinst**, ser vi att webbannonskanalen, nu den grönaste, påverkade mer intäkter - över tid_ än webbseminariet och handelskanalerna.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

I vårt exempel ser vi att Tradeshow-kanalen både är den mest dyra (längst till höger) och den mest framgångsrika (högst på Y-axeln) när man mäter pipeline som skapats med första beröring. Låt oss nu titta på varje kanals pipeline som skapats som en funktion av multitouch-attribuering.

>[!TIP]
>
>Exemplen i dessa steg mäter effektiviteten utifrån den pipeline som skapats. Använd listrutan Y-axel för att välja andra sätt att mäta kanalens effektivitet, t.ex. nya namn, medlemmar, kostnad per lyckad åtgärd osv.

>[!MORELIKETHIS]
>
>* [Utforska program- och kanalinformation med Program Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Jämför programeffektiviteten med programanalysen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
