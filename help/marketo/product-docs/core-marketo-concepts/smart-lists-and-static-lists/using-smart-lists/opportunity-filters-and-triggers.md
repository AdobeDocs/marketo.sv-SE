---
unique-page-id: 8159286
description: Filter och utlösare för affärsmöjligheter - Marketo Docs - produktdokumentation
title: Filter och utlösare för affärsmöjligheter
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Filter och utlösare för affärsmöjligheter {#opportunity-filters-and-triggers}

Med filter och utlösare för affärsmöjligheter kan du spåra affärsmöjlighetshändelser från Salesforce. De är lite annorlunda jämfört med andra filter och utlösare.

## Affärsmöjlighetsfilter {#opportunity-filters}

Med säljprojektsfilter kan du fördjupa dig i dina Salesforce-leads som har möjligheter. Du kan hitta dem i mappen Affärsmöjligheter på paletten när du redigerar en smart lista. De kommer i några smaker.

* Antal optyer
* Totalt tomt belopp
* Förväntad intäkt för total optisk summa
* Har möjlighet
* Affärsmöjligheten har lagts till
* Möjligheten har tagits bort
* Affärsmöjligheten har uppdaterats

Om du letar efter dina säljprojektsfält (anpassade eller standard) använder du filtret **Har säljprojekt** eller **säljprojektet var`[Added/Removed/Updated]`** filter eller utlösare.

**Antal optyer, totalt otillgängligt belopp, totalt förväntade intäkt för optisk enhet**

Med de här filtren kan du hitta leads baserat på det totala antalet, beloppet eller den förväntade intäkten för alla deras möjligheter.

![](assets/opportunity-filters-and-triggers-1.png)

**Har affärsmöjlighet, har lagts till i affärsmöjligheten, har tagits bort från affärsmöjligheten**

Om du letar efter leads som har affärsmöjligheter baserat på en kombination av villkor använder du filtret **Har affärsmöjlighet**, **lades till i affärsmöjlighet** eller **togs bort från affärsmöjlighet**. De säger:

* **Har affärsmöjlighet**: Om denna lead för närvarande har någon matchande affärsmöjlighet
* **lades till i affärsmöjligheten**: Om denna lead någonsin lagts till i en matchande affärsmöjlighet
* **togs bort från affärsmöjligheten**: Om denna lead någonsin tagits bort från en matchande affärsmöjlighet

Lägg till sökvillkoren som **Begränsningar** i filtret. Begränsningarna inkluderar affärsmöjlighetens standardfält och anpassade fält:

![](assets/opportunity-filters-and-triggers-2.png)

![](assets/opportunity-filters-and-triggers-3.png)

Anta att du vill hitta leads som har öppna möjligheter på minst 5 000 USD. Dra i filtret **Har säljprojekt** och använd begränsningarna **Är stängd** och **Belopp**:

![](assets/opportunity-filters-and-triggers-4.png)

>[!NOTE]
>
>När du använder flera säljprojektsfilter kan du få felaktiga svar. Om du har skapat exemplet ovan med två säljprojektsfilter får du en lista över leads som har en affärsmöjlighet som är minst 5 000 USD och en affärsmöjlighet som är stängd, även om de är separata affärsmöjligheter.

**Affärsmöjligheten har uppdaterats**

Filtret **Affärsmöjligheten har uppdaterats** och söker efter en affärsmöjlighet när ett specifikt affärsmöjlighetsfält uppdaterades. Välj det fält som ska kontrolleras med listrutan Utlösarattribut och använd sedan begränsningarna för att begränsa uppsättningen ändringar.

Det här filtret visar t.ex. alla leads som har haft stängningsdatum ändrade inom de senaste 30 dagarna:

![](assets/opportunity-filters-and-triggers-5.png)

## Affärsmöjligheter - utlösare {#opportunity-triggers}

Följande affärsmöjlighetsutlösare är tillgängliga. De fungerar precis som motsvarande filter (beskrivs tidigare), förutom att de kan utlösa kampanjer direkt när händelsen inträffar:

* Affärsmöjligheten har uppdaterats
* Tillagt i affärsmöjlighet
* Borttagen från affärsmöjlighet

Du kan till exempel använda den här smarta listan för att utlösa när någon lead läggs till i en affärsmöjlighet. I flödet kan du lägga till dem i listan Marketing Suspended (Pausad) eller skicka ett riktat e-postmeddelande till dem.

![](assets/opportunity-filters-and-triggers-6.png)

Använd utlösaren **Opportunity is Updated** och välj fältet i listrutan om du vill aktivera dina anpassade fält för affärsmöjligheten:

![](assets/opportunity-filters-and-triggers-7.png)
