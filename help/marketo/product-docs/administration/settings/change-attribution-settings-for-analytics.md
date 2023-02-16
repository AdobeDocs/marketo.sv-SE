---
unique-page-id: 2360217
description: Ändra attributinställningar för analys - Marketo Docs - produktdokumentation
title: Ändra attributinställningar för analys
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Ändra attributinställningar för analys {#change-attribution-settings-for-analytics}

Ni kan ändra det sätt på vilket Marketo knyter kontakter till möjligheter till första- och flerberöringsattribuering, konverteringsstatistik för leads och flaggan för marknadspåverkade affärsmöjligheter.

De här inställningarna kommer att påverka rapporter i Intresseutforskaren under [Analys av affärsmöjligheter](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Affärsmöjlighetsanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)och områden för Lead Analysis. Det här påverkar även rapporten för Program Analyzer.

1. Gå till **Administratör** område.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicka **Analys av intäktscykler**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicka på **Redigera** länk under **Attribut**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Om du ändrar den här inställningen ändras inga Marketo-data. helt enkelt förändrar hur era rapporter fungerar. Detta kan återställas när som helst.

1. Välj ett alternativ och klicka på **Spara**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**Explicit**: Endast kontakter med roller (standard).
   >
   >**Hybrid**: Kontakter med roller, om sådana finns. Om det inte finns några tillgängliga används alla kontakter i kontona.
   >
   >**Implicit**: Alla kontakter oavsett roll.

>[!CAUTION]
>
>När du använder **Implicit** kommer Marketo alltid att undersöka alla kontakter som är kopplade till kontot, oavsett roll. **Marketo rekommenderar starkt att du använder läget Explicit**. Om du använder Implicit kan det skapa falska positiva resultat. dvs. människor som har beröm för en möjlighet trots att de inte har något verkligt inflytande på möjligheten. Använd implicit med försiktighet.
