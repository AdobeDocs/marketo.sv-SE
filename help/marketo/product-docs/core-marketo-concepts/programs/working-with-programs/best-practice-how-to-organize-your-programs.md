---
unique-page-id: 6848705
description: Bästa praxis -Hur du organiserar program - Marketo Docs - Produktdokumentation
title: Bästa praxis -Så här organiserar du dina program
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---


# God praxis: Organisera dina program {#best-practice-how-to-organize-your-programs}

Det finns många sätt att organisera trädet i marknadsföringsaktiviteter samt innehållet i ett enda program. Men det finns vissa sätt som är bättre och som kommer att hjälpa marknadsförare.

>[!TIP]
>
>En dag (när du blir befordrad!) någon annan kommer att försöka förstå dina program. En bra organisation kommer att hjälpa dem att bli produktiva snabbt.

## Mappar {#folders}

I marknadsföringsaktiviteter bör du använda mappar för att ordna dina program. Strukturen vi rekommenderar finns i följande exempel:

>[!NOTE]
>
>**Exempel**
>
>* Aktiva marknadsföringsprogram
>
>    * E-post
>    * Händelser
>
>        * Live Events/Roadshows
>        * Varumärken
>        * Webbinarier
>   * Nyhetsbrev
>   * Nätur
>   * Webbinnehåll
>   * Webbformulär
>* Utbildning
>* Operativ
>
>   * Livscykel
>   * Poäng
>   * Datahantering
>* Sales Insight
>   * Intressanta ögonblick
>   * Försäljningsmejl
>   * Begärda försäljningskampanjer
>* **Arkiv**
>   * Arkivera händelser
>      * Arkiv 2012
>      * Arkiv 2013







Var och en av dessa nämns i exemplet är en mapp. Lägg märke till att de alla är unikt namngivna. Du kan ha duplicerade (enklare) namn på mappar INUTI-program, men inte i roten av trädet.

>[!TIP]
>
>Mappen&quot;Arkiv&quot; är en speciell typ av mapp som är utformad för att ta bort objekt från utvalda listor samt rapporter. Det gör att systemet kan köras snabbare. Läs [mer om mappar](../../../../product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

Du kan lägga till fler mappar när du vill. Tänk bara på att framtida generationer marknadsförare i företaget kommer att leva med dina beslut om hur ni namnger/organiserar saker.

## Namngivningsscheman {#naming-schemes}

Namngivning är viktigt eftersom alla Marketos funktioner använder ett gemensamt språk för att kommunicera. För program bör du ge dem ett unikt namn. **Två program får inte ha samma namn**. Det bästa sättet är att använda följande format:

[Förkortning av programtyp ] [YYYY]-[MM]-[Optional ] [DDBrief - beskrivning]

>[!NOTE]
>
>**Exempel**
>
>Exempel på programnamn:
>
>1. ES 2015-09-21 Widget Intro
>1. NL 2015-06 nyhetsbrev
>1. WBN 2015-12-01 Webbseminarium här

>



Programnamnen måste vara unika i prenumerationen, även i olika [arbetsytor](../../../../product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  För lokala resurser i program är regeln att **behålla namnet enkelt**. Ange bara&quot;Inbjudan&quot; till skillnad från&quot;2015 Juniwebbinariet Invitation&quot;. Eftersom dessa finns i ett program är det överordnade programmet automatiskt en del av namnet när du väljer det någon annanstans. Med andra ord behöver lokala resurser bara vara unika inom programmet. Du kan ha hundratals resurser som heter&quot;Bjud in&quot;, var och en i ett annat program och det kommer inte att försvåra dig.

## Tokens {#tokens}

Tokens använder mappar och program som ett hjälpmedel för att ange variabler som ska användas av landningssidor, e-postmeddelanden och andra resurser. Lär dig [allt om tokens](http://docs.marketo.com/display/docs/tokens).

Med den organisation som nämns ovan kan du placera tokens i händelsemappen så att den överlappar alla händelser.

>[!NOTE]
>
>**Exempel**
>
>**Din företagsadress**. Använd en variabel i stället för att skriva den varje gång. På så sätt kan du uppdatera den på en plats utan att behöva skapa många utkast. Åsidosätt sedan variabeln efter behov i en mapp på lägre nivå.

## Händelser {#events}

En händelse har vanligtvis många rörliga delar, bland annat: inbjudningar, landningssidor, formulär, sociala widgetar och smarta kampanjer. Det bästa sättet att organisera dem för att underlätta användningen är att använda händelsefasen. Här är ett exempel på hur mappträdet ska söka efter en händelse.

![](assets/capture.png)

## Åtagandeprogram {#engagement-programs}

Lär dig [allt om engagemangsprogram](../../../../product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). Det bästa sättet att organisera engagemangsprogrammet är med mappar. Skapa en mapp för varje ström och placera sedan e-postmeddelandena eller programmen i den mappen. Inkludera en arkivmapp i varje ström när innehållet blir inaktuellt och du vill ta bort det.

## Operativa program {#operational-programs}

De används för datarensning. Ha mappar för de datum som programmen kördes och arkivera sedan mapparna. Genom att göra programmet operativt utelämnar ni den från att rapportera, vilket är bra för den här typen av aktiviteter.

## Kapslar e-postprogram {#nesting-email-programs}

E-postprogram är utformade för att vara ditt verktyg för massutskick av e-post. Du kan placera dem i Evenemang och andra program för kampanjer, inbjudningar och påminnelser. De har en häftig kontrollpanel och andra A/B-testfunktioner. Dessutom kan de enkelt hanteras i [programschemavyn](http://docs.marketo.com/display/docs/program+schedule+view).

Du kan också skapa ett e-postprogram som ett fristående program. E-postprogram tillåts inte i andra e-postprogram. Det vore galet!

## Klona {#cloning}

En av de coolaste funktionerna i Marketo är möjligheten att klona program. Det innebär att ni kan skapa en programmall med alla smarta kampanjer och e-postmeddelanden ni vill ha. Installera den i förväg och klona den sedan för nästa marknadsföringsinitiativ.

>[!TIP]
>
>Lägg märke till händelsemallarna i exemplet längst upp. Lägg in olika typer av händelser för enkel kloning.

En del människor kan till och med abstrahera större delen av texten i e-postmeddelanden och landningssidor till tokens. Detta gör att du kan klona och sedan redigera tokenerna. Till sist går du till programschemavyn och justerar datumen så är du klar. Voila!

## Sammanfattning {#summary}

Som du ser finns det mycket kraft i Marketo. Grunderna har beskrivits här, men tänk på ytterligare [tjänster från Marketo Experts](http://www.marketo.com/services/) för att finjustera och konfigurera dig själv för att lyckas.
