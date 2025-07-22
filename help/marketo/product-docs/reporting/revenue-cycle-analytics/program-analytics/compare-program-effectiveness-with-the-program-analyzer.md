---
unique-page-id: 2360403
description: Jämför programeffektiviteten med programanalysen - Marketo Docs - produktdokumentation
title: Jämför programeffektiviteten med programanalysen
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Jämför programeffektivitet med [!UICONTROL Program Analyzer] {#compare-program-effectiveness-with-the-program-analyzer}

Använd [!UICONTROL Program Analyzer] för att identifiera dina mest och minst effektiva program genom att jämföra programkostnader, medlemskap, pipeline och intäkter.

>[!PREREQUISITES]
>
>[Skapa en [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Klicka på **[!UICONTROL Analytics]**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Välj programanalyseraren.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Ändra vyn till **[!UICONTROL By Program]**.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Använd **[!UICONTROL Channel Filter]** om du vill minska vyn till endast en eller två kanaler. För tillfället ska vi titta på program i **[!UICONTROL Tradeshow]**-kanalen.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Ett snabbt sätt att filtrera program till endast en kanal är att välja **[!UICONTROL View]** > **[!UICONTROL By Channel]**, klicka på bubblan för den kanalen och sedan klicka på kanalnamnet i popup-dialogrutan.

1. Använd listrutan **[!UICONTROL X Axis]** för att välja ett mått för den vågräta axeln. Vi börjar med **[!UICONTROL Program Cost]**.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Använd listrutan **[!UICONTROL Y Axis]** för att välja ett mått för den lodräta axeln. Vi väljer **[!UICONTROL New Names]** för att hitta program som är bra på att hämta nya leads.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Aktivera skjutreglagen för att zooma in.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >Du kan också försöka förbättra visningen genom att ändra från en linjär till en logaritmisk skala, eller tvärtom. Använd menyn **[!UICONTROL Scale]** överst.

1. Utforska det resulterande diagrammet.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   I det här exemplet lär vi oss att [!DNL Origami Expo] är mycket bättre än alla andra program i den kanalen när det gäller att hämta nya namn, till en medelhög kostnad. Men det är inte hela historien. Vi lägger till ytterligare två mätvärden för att få en djupare förståelse.

1. Använd listrutan **[!UICONTROL Bubble Size]** för att välja ett mätvärde som ska jämföras med bubblornas storlek. Vi väljer **[!UICONTROL (FT) Revenue Won]** som exempel.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Många av de mätvärden du kan välja i programanalysen är tillgängliga med beräkningar med första beröringen (FT) och multitouch (MT). Det är viktigt att förstå skillnaden [mellan FT- och MT-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Se bubblorna ändra storlek i diagrammet.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Genom att lägga till **[!UICONTROL (FT) Revenue Won]** ser vi snabbt att även om [!DNL Origami Expo] har skaffat många nya namn så ger det en relativt liten intäkt. Dessutom ser vi att programmet [!DNL Paper Fest 12] får färre men bättre namn eftersom det påverkar fler intäkter (större bubbla).

1. Använd listrutan Färg för att lägga till ett fjärde mått. Vi tittar på **[!UICONTROL (FT) Revenue to Investment]**.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Se hur färgerna ändras i diagrammet.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vi ser att programmet [!DNL Paper Fest 12] inte bara påverkar mer intäkter (större bubbla), utan även om det är relativt högt (längst till höger) har det den bästa avkastningen på investeringen (den grönaste bubblan) för alla program i kanalen [!UICONTROL Tradeshow].

>[!TIP]
>
>Du kan snabbt jämföra program i en kanal med program i en annan. Använd bara **kanalfiltret** längst upp i fönstret för att lägga till fler kanaler.

>[!MORELIKETHIS]
>
>* [Utforska program- och kanalinformation med [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Jämför kanaleffekt med [!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
