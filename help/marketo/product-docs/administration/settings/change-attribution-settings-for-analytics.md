---
unique-page-id: 2360217
description: Ändra attributinställningar för analys - Marketo Docs - Produktdokumentation
title: Ändra attributinställningar för analys
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Ändra attributinställningar för analys {#change-attribution-settings-for-analytics}

Ni kan ändra det sätt Marketo knyter kontakter till möjligheter för första- och flerberöringsattribuering, konverteringsstatistik för leads och flaggan för marknadspåverkade affärsmöjligheter.

De här inställningarna påverkar Intresseutforskarrapporter under [Programsäljprojektsanalys](../../../product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Affärsmöjlighetsanalys](../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) och Leadanalys. Det här påverkar även rapporten för Program Analyzer.

1. Klicka på **Intäktscykelanalys** under **Admin**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Klicka på länken **Redigera** under **Attribution**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Om du ändrar den här inställningen ändras inga Marketo-data. helt enkelt förändrar hur era rapporter fungerar. Detta kan återställas när som helst.

1. Välj ett alternativ och klicka på **Spara**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >
   >**Explicit**: Endast kontakter med roller (standard).
   >
   >
   >**Hybrid**: Kontakter med roller, om sådana finns. Om det inte finns några tillgängliga används alla kontakter i kontona.
   >
   >
   >**Implicit**: Alla kontakter oavsett roll.

>[!CAUTION]
>
>När du använder **Implicit** kommer Marketo alltid att undersöka alla kontakter som är kopplade till kontot, oavsett roll. **Marketo rekommenderar starkt att du använder läget Explicit.** Om du använder Implicit kan det skapa falska positiva resultat. dvs. människor som har beröm för en möjlighet trots att de inte har något verkligt inflytande på möjligheten. Använd implicit med försiktighet.

