---
unique-page-id: 2360403
description: Jämför programeffektiviteten med Program Analyzer - Marketo Docs - Produktdokumentation
title: Jämför programeffektiviteten med programanalysen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# Jämför programeffektiviteten med programanalysen {#compare-program-effectiveness-with-the-program-analyzer}

Använd Program Analyzer för att identifiera era mest effektiva program genom att jämföra programkostnader, medlemsförvärv, pipeline och intäkter.

>[!PREREQUISITES]
>
>* [Skapa en programanalys](create-a-program-analyzer.md)


1. Klicka på Analytics.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Välj programanalyseraren.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Ändra vyn till Efter program.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Använd kanalfiltret om du vill förminska vyn till bara en eller två kanaler. För tillfället ska vi titta på program i Tradeshow-kanalen.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Ett snabbt sätt att filtrera program till endast en kanal är att välja **Visa > Efter kanal**, klicka på bubblan för den kanalen och sedan klicka på kanalnamnet i popup-dialogrutan.

1. Använd listrutan X-axel för att välja ett mått för den vågräta axeln. Vi börjar med Programkostnad.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Använd listrutan Y-axel för att välja ett mått för den lodräta axeln. Låt oss välja Nya namn för att hitta program som är bra på att fånga upp nya leads.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Aktivera reglagen för att zooma in.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >Du kan också försöka förbättra visningen genom att ändra från en linjär till en logaritmisk skala, eller tvärtom. Använd menyn **Skala** längst upp.

1. Utforska det resulterande diagrammet.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   I vårt exempel lär vi oss att Origami Expo är mycket bättre än alla andra program i den kanalen när det gäller att hämta nya namn, till en medelhög kostnad. Men det är inte hela historien. Vi lägger till ytterligare två mätvärden för att få en djupare förståelse.

1. Använd listrutan Bubbelstorlek för att välja ett mätvärde som ska jämföras med bubblornas storlek. Vi ska välja (FT) Revenue Won som exempel.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >Många av de mätvärden du kan välja i programanalysen är tillgängliga med beräkningar med första beröringen (FT) och multitouch (MT). Det är viktigt att förstå skillnaden [mellan FT- och MT-attribuering](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Se bubblorna ändra storlek i diagrammet.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   Genom att lägga till **(FT) Revenue Won** ser vi snabbt att medan Origami Expo köpte många nya namn resulterar det i relativt liten intäkt. Vi ser också att Paper Fest 12-programmet får färre men bättre namn eftersom det påverkar fler intäkter (större bubbla).

1. Använd listrutan Färg för att lägga till ett fjärde mått. Vi ska titta på (FT) Revenue to Investment.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Se hur färgerna ändras i diagrammet.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

Vi ser att Paper Fest 12-programmet inte bara påverkar mer intäkter (större bubbla), utan trots dess relativt höga programkostnad (längst till höger) har det den bästa avkastningen på investeringar (grönaste bubblan) i alla program i Tradeshow-kanalen.

>[!TIP]
>
>Du kan snabbt jämföra program i en kanal med program i en annan. Använd bara **kanalfiltret** längst upp i fönstret för att lägga till fler kanaler.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Utforska program- och kanalinformation med Program Analyzer](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Jämför kanaleffektiviteten med programanalysen](compare-channel-effectiveness-with-the-program-analyzer.md)


>[!NOTE]
>
>Läs mer om avancerad analys i [Inkomstcykelutforskaren](http://docs.marketo.com/display/docs/revenue+cycle+analytics).
