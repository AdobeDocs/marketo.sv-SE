---
unique-page-id: 2950396
description: Prioritet, Urklipp, Relativ poäng och Bästa val - Marketo Docs - Produktdokumentation
title: Prioritet, Urklipp, Relativa poäng och Bästa val
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Prioritet, Urklipp, Relativa poäng och Bästa val {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight väljer ut dina bästa leads och kontakter baserat på deras prioritet. En lead eller kontakts prioritet har två komponenter - trängsel och relativ poäng.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

De bygger på huvudpoängen - ett mått på personens intresse för dina produkter. Ju högre poäng, desto mer troligt är det att de svarar positivt på ett samtal från säljteamet.

>[!NOTE]
>
>Ni behöver flera poängsättningskampanjer för att få ut maximalt av prioritet, brådskande och relativ poäng.  För få eller inga poängkampanjer gör de här fälten inte användbara.

## Akut {#urgency}

Lågorna är brådskande - hur mycket personens ledspår har ändrats nyligen. Ett mycket brådskande (mer lågornas) innebär att poängen för detta lead har ökat mycket på sistone. är det ett gott tecken på att denna lead är intresserad av ditt erbjudande. Du borde följa upp med den här personen snabbt!

En lead som till exempel har begärt en demo och besökt flera webbsidor kommer förmodligen att ha en väldigt hög prioritet. En ledare som inte besökt din webbsida eller öppnade dina e-postmeddelanden kommer att ha låg brådska. Det är angeläget att prioritera vilka som ska kontaktas härnäst.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Relativa poäng {#relative-score}

Stjärnorna representerar relativa poäng - ett mått på hur den här personens poäng kan jämföras med alla andras. En hög relativ poäng innebär att den här personen förmodligen är mer intresserad och informerad om ditt erbjudande jämfört med personer med lägre relativa poäng.

Om två leads är lika brådskande kan du använda relativa poäng för att avgöra vilken som är värd att ringa ett telefonsamtal först. Den som har den högre relativa poängen kan reagera mer positivt på ert erbjudande jämfört med den lägre.

## Bästa val {#best-bets}

Bästa valet är dina leads och kontakter med högsta prioritet och relativa poäng. Endast de leads du äger visas i listan och listan uppdateras när poängen ändras.

>[!NOTE]
>
>Om dina bästa val inte matchar de bästa leads och kontakter du äger, kan du prata med någon på ditt företag som har tillgång till Marketo om hur du uppdaterar dina [Poängregler](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Hur brådskande och relativ poäng beräknas

Om du vill beräkna antalet stjärnor och lågor sorteras dina leads och kontakter först efter poäng- eller poängändring (för Relativ poäng respektive Urbräda). Sedan delas de in i lager - den översta nivån får flest stjärnor eller lågor, den nästa får färre och så vidare.

Efterhand som poängen ändras räknas värdena för tränglighet, prioritet och relativ poäng om omedelbart. Behovet och de relativa poängnivåerna beräknas automatiskt varje kväll på Marketo-servrar.

>[!NOTE]
>
>Antalet Relativa nödlägen (lågor) och Relativa bakgrundsmusik (stjärnor) är heltal i Marketo. Möjliga värden för var och en är 0-3.
