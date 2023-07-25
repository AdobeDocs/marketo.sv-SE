---
unique-page-id: 8159286
description: Filter och utlösare för affärsmöjligheter - Marketo Docs - produktdokumentation
title: Filter och utlösare för affärsmöjligheter
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filter och utlösare för affärsmöjligheter {#opportunity-filters-and-triggers}

Med filter och utlösare för affärsmöjligheter kan du spåra affärsmöjlighetshändelser från Salesforce. De är lite annorlunda jämfört med andra filter och utlösare.

## Filter för affärsmöjlighet {#opportunity-filters}

Med säljprojektsfilter kan du fördjupa dig i dina Salesforce-leads som har möjligheter. Du kan hitta dem i mappen Affärsmöjligheter på paletten när du redigerar en smart lista. De kommer i några smaker.

* Antal optyer
* Totalt tomt belopp
* Förväntad intäkt för total optisk summa
* Har möjlighet
* Affärsmöjligheten har lagts till
* Affärsmöjligheten har tagits bort
* Affärsmöjligheten har uppdaterats

Om du letar efter dina säljprojektsfält (anpassade eller standard) använder du **Har möjlighet** filter eller **Möjligheten var`[Added/Removed/Updated]`** filter eller utlösare.

**Antal optyer, totalt belopp för optisk enhet, totalt förväntad intäkt för optisk enhet**

Med de här filtren kan du hitta leads baserat på det totala antalet, beloppet eller den förväntade intäkten för alla deras möjligheter.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Har affärsmöjlighet, lades till i affärsmöjligheten, togs bort från affärsmöjligheten**

Om du letar efter leads som har affärsmöjligheter baserat på en kombination av villkor använder du **Har möjlighet**, **lades till i affärsmöjligheten**, eller **Borttagen från affärsmöjligheten** filter. De säger:

* **Har möjlighet**: Om denna lead för närvarande har någon matchande affärsmöjlighet
* **lades till i affärsmöjligheten**: Om denna lead någonsin lagts till i en matchande affärsmöjlighet
* **Borttagen från affärsmöjligheten**: Om denna lead någonsin tagits bort från en matchande affärsmöjlighet

Lägg till sökvillkoren som **Begränsningar** på filtret. Begränsningarna inkluderar affärsmöjlighetens standardfält och anpassade fält:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Anta att du vill hitta leads som har öppna möjligheter på minst 5 000 USD. Dra i **Har möjlighet** filtrera och använda **Är stängd** och **Belopp** begränsningar:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>När du använder flera säljprojektsfilter kan du få felaktiga svar. Om du har skapat exemplet ovan med två säljprojektsfilter får du en lista över leads som har en affärsmöjlighet som är minst 5 000 USD och en affärsmöjlighet som är stängd, även om de är separata affärsmöjligheter.

**Affärsmöjligheten har uppdaterats**

The **Affärsmöjligheten har uppdaterats** filter söker efter alla affärsmöjligheter när ett specifikt affärsmöjlighetsfält har uppdaterats. Välj det fält som ska kontrolleras med listrutan Utlösarattribut och använd sedan begränsningarna för att begränsa uppsättningen ändringar.

Det här filtret visar t.ex. alla leads som har haft stängningsdatum ändrade inom de senaste 30 dagarna:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Affärsmöjligheter - utlösare {#opportunity-triggers}

Följande affärsmöjlighetsutlösare är tillgängliga. De fungerar precis som motsvarande filter (beskrivs tidigare), förutom att de kan utlösa kampanjer direkt när händelsen inträffar:

* Affärsmöjligheten har uppdaterats
* Tillagt i affärsmöjlighet
* Borttagen från affärsmöjlighet

Du kan till exempel använda den här smarta listan för att utlösa när någon lead läggs till i en affärsmöjlighet. I flödet kan du lägga till dem i listan Marketing Suspended (Pausad) eller skicka ett riktat e-postmeddelande till dem.

![](assets/image2015-6-11-12-3a33-3a48.png)

Använd **Affärsmöjligheten har uppdaterats** utlösa och plocka fältet i pulldown:

![](assets/image2015-6-11-12-3a33-3a34.png)
