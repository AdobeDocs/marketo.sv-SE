---
unique-page-id: 2950396
description: Prioritet, Urklipp, Relativ poäng och Bästa val - Marketo Docs - Produktdokumentation
title: Prioritet, Urklipp, Relativa poäng och Bästa val
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---


# Prioritet, Urklipp, Relativa poäng och Bästa val {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight väljer ut dina bästa leads och kontakter baserat på deras prioritet. En lead eller kontakts prioritet har två komponenter - trängsel och relativ poäng.

![](assets/one.png)

De bygger på huvudpoängen - ett mått på personens intresse för dina produkter. Ju högre poäng, desto mer troligt är det att de svarar positivt på ett samtal från säljteamet.

>[!NOTE]
>
>Ni behöver flera poängsättningskampanjer för att få ut maximalt av prioritet, brådskande och relativ poäng.  För få eller inga poängkampanjer gör de här fälten inte användbara.

## Akut {#urgency}

Lågorna är brådskande - hur mycket personens ledspår har ändrats nyligen. Ett mycket brådskande (mer lågornas) innebär att poängen för detta lead har ökat mycket på sistone. är det ett gott tecken på att denna lead är intresserad av ditt erbjudande. Du borde följa upp med den här personen snabbt!

En lead som till exempel har begärt en demo och besökt flera webbsidor kommer förmodligen att ha en väldigt hög prioritet. En ledare som inte besökt din webbsida eller öppnade dina e-postmeddelanden kommer att ha låg brådska. Det är angeläget att prioritera vilka som ska kontaktas härnäst.

![](assets/two.png)

## Relativa poäng {#relative-score}

Stjärnorna representerar relativa poäng - ett mått på hur den här personens poäng kan jämföras med andras. En hög relativ poäng innebär att den här personen förmodligen är mer intresserad och informerad om ditt erbjudande jämfört med personer med lägre relativa poäng.

Om två leads är lika brådskande kan du använda relativa poäng för att avgöra vilken som är värd att ringa ett telefonsamtal först. Den som har det högsta relativa poängvärdet kan reagera mer positivt på ditt erbjudande jämfört med det lägre.

## Bästa val {#best-bets}

Bästa valet är dina leads och kontakter med högsta prioritet och relativa poäng. Endast de leads du äger visas i listan och listan uppdateras när poängen ändras.

>[!NOTE]
>
>Om dina bästa val inte matchar de bästa leads och kontakter du äger, kan du prata med någon på ditt företag som har tillgång till Marketo om att uppdatera dina [poängregler](../../../../../getting-started/quick-wins/simple-scoring.md).

### Hur brådskande och relativ poäng beräknas

Om du vill beräkna antalet stjärnor och lågor sorteras dina leads och kontakter först efter poäng- eller poängändring (för Relativ poäng respektive Urbräda). Sedan delas de in i lager - den översta nivån får flest stjärnor eller lågor, den nästa får färre och så vidare.

Efterhand som poängen ändras räknas värdena för tränglighet, prioritet och relativ poäng om omedelbart. Behovet och de relativa poängnivåerna beräknas automatiskt varje kväll på Marketo-servrar.

>[!NOTE]
>
>Antalet Relative Urgent (Lågor) och Relative Score (stjärnor) är heltal i Marketo. Möjliga värden för var och en är 0-3.

>[!MORELIKETHIS]
>
>* [Marketo Sales Insight](http://docs.marketo.com/display/docs/marketo+sales+insight)

