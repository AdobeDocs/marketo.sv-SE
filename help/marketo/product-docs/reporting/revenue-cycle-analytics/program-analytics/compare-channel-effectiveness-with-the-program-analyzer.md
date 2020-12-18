---
unique-page-id: 2360401
description: Jämför kanaleffektivitet med Program Analyzer - Marketo Docs - Produktdokumentation
title: Jämför kanaleffektiviteten med programanalysen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


# Jämför kanaleffektiviteten med programanalysen {#compare-channel-effectiveness-with-the-program-analyzer}

Använd Program Analyzer för att jämföra kanalkostnader, medlemsförvärv, pipeline, intäkter med mera för att identifiera era mest effektiva kanaler.

>[!PREREQUISITES]
>
>* [Skapa en programanalys](create-a-program-analyzer.md)


1. Klicka på **Analytics** i **My Marketo.**

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Välj din **programanalys.**

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Ändra vyn till **By** **Kanal**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Använd listrutan **X-axel** för att välja ett mått för den vågräta axeln. Vi börjar med **Programkostnad**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Använd listrutan Y-axel för att välja ett mått för den lodräta axeln. Här följer en **(FT)-pipeline skapad**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Många av de mätvärden du kan välja i programanalysen är tillgängliga med beräkningar med första beröringen (FT) och multitouch (MT). Det är viktigt att förstå skillnaden [mellan FT- och MT-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Använd listrutan **Y-axel** för att välja **(MT) Pipeline skapad**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   I den här flerberöringsattribueringsvyn ser vi att webbseminariekanalen har större påverkan på den pipeline som skapas och mindre kostnader än kanalerna Tradeshow och Online Advertising.

   Nu ska vi lägga till ytterligare två dimensioner!

1. Använd listrutan **Bubbelstorlek** för att välja ytterligare ett mått, som **Nya namn**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Se hur diagrammet ändras.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vi ser att webbseminariekanalen krymper, enligt **Nya namn**. Vi kan dra slutsatsen att även om den har många medlemmar är det mindre effektivt att generera nya leads än Tradeshow-kanalen.

1. Använd slutligen listrutan Färg för att lägga till den fjärde dimensionen. Vi väljer **(FT) Revenue** **Won**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Se hur färgerna ändras i diagrammet.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Av färgerna har vi fått veta att Tradeshow-kanalen, den grönaste bubblan, har påverkat de största intäkterna, som mäts med första-beröringsattribuering.

1. Om vi nu ändrar Color-måttet till **(MT) Revenue Won** ser vi att Online Advertising Channel, nu den grönaste, påverkade mer intäkter -over time_ än webbseminariet och Tradeshow-kanalerna.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

I vårt exempel ser vi att Tradeshow-kanalen både är den mest dyra (längst till höger) och den mest framgångsrika (högst på Y-axeln) när man mäter pipeline som skapats med första beröring. Låt oss nu titta på varje kanals pipeline som skapats som en funktion av multitouch-attribuering.

>[!TIP]
>
>Exemplen i dessa steg mäter effektiviteten utifrån den pipeline som skapats. Använd listrutan Y-axel för att välja andra sätt att mäta kanalens effektivitet, t.ex. nya namn, medlemmar, kostnad per lyckad åtgärd osv.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Utforska program- och kanalinformation med Program Analyzer](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Jämför programeffektiviteten med programanalysen](compare-program-effectiveness-with-the-program-analyzer.md)

>



>[!NOTE]
>
>Läs mer om avancerad analys i [Inkomstcykelutforskaren](http://docs.marketo.com/display/docs/revenue+cycle+analytics).
