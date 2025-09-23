---
unique-page-id: 2360401
description: Jämför kanaleffektivitet med programanalys - Marketo Docs - produktdokumentation
title: Jämför kanaleffektiviteten med programanalysen
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Jämför kanaleffektivitet med [!UICONTROL Program Analyzer] {#compare-channel-effectiveness-with-the-program-analyzer}

Använd [!UICONTROL Program Analyzer] för att jämföra kanalkostnader, medlemsförvärv, pipeline, intäkter med mera för att identifiera dina mest och minst effektiva kanaler.

>[!PREREQUISITES]
>
>[Skapa en [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Klicka på **[!UICONTROL Analytics]** i **Min Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Välj programanalyseraren.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Ändra vyn till **[!UICONTROL By Channel]**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Använd listrutan **[!UICONTROL X Axis]** för att välja ett mått för den vågräta axeln. Vi börjar med **[!UICONTROL Program Cost]**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Använd listrutan **[!UICONTROL Y Axis]** för att välja ett mått för den lodräta axeln. Här följer **[!UICONTROL (FT) Pipeline Created]**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Många av de mätvärden du kan välja i programanalysen är tillgängliga med beräkningar med första beröringen (FT) och multitouch (MT). Det är viktigt att förstå skillnaden [mellan FT- och MT-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Använd listrutan **[!UICONTROL Y Axis]** för att välja **[!UICONTROL (MT) Pipeline Created]**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   I den här flerberöringsattribueringsvyn ser vi att webbseminariekanalen har större påverkan på den pipeline som skapas och kostar mindre än kanalerna Tradeshow och Online Advertising.

   Nu ska vi lägga till ytterligare två dimensioner!

1. Använd listrutan **[!UICONTROL Bubble Size]** för att välja ytterligare ett mått, som **[!UICONTROL New Names]**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Se hur diagrammet ändras.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vi ser att webbseminariekanalen krymper, enligt **[!UICONTROL New Names]**. Vi kan dra slutsatsen att även om den har många medlemmar är det mindre effektivt att generera nya leads än Tradeshow-kanalen.

1. Använd slutligen listrutan Färg för att lägga till den fjärde dimensionen. Vi väljer **[!UICONTROL (FT) Revenue Won]**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Se hur färgerna ändras i diagrammet.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Av färgerna har vi fått veta att Tradeshow-kanalen, den grönaste bubblan, har påverkat de största intäkterna, som mäts med första-beröringsattribuering.

1. Om vi nu ändrar Color-måttet till **[!UICONTROL (MT) Revenue Won]** ser vi att Advertising-onlinekanalen, som nu är den grönaste, påverkade mer intäkter _över tid_ än webbseminariet och handelskanalen.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

I vårt exempel ser vi att Tradeshow-kanalen både är den mest dyra (längst till höger) och den mest framgångsrika (högst på Y-axeln) när man mäter pipeline som skapats med första beröring. Låt oss nu titta på varje kanals pipeline som skapats som en funktion av multitouch-attribuering.

>[!TIP]
>
>Exemplen i dessa steg mäter effektiviteten utifrån den pipeline som skapats. Använd listrutan [!UICONTROL Y Axis] för att välja andra sätt att mäta kanalens effektivitet, som [!UICONTROL New Names], [!UICONTROL Members], [!UICONTROL Cost per Success] osv.

>[!MORELIKETHIS]
>
>* [Utforska program- och kanalinformation med [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Jämför programeffektivitet med [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
