---
unique-page-id: 2360217
description: Ändra attributinställningar för analys - Marketo Docs - produktdokumentation
title: Ändra attributinställningar för analys
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Ändra attributinställningar för analys {#change-attribution-settings-for-analytics}

Ni kan ändra det sätt på vilket Marketo knyter kontakter till möjligheter till första- och flerberöringsattribuering, konverteringsstatistik för leads och flaggan för marknadspåverkade affärsmöjligheter.

De här inställningarna påverkar [!UICONTROL Revenue Explorer] rapporter enligt [Analys av affärsmöjligheter](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Affärsmöjlighetsanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)och områden för Lead Analysis. Detta påverkar även [!UICONTROL Program Analyzer] rapport.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicka på **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicka på **[!UICONTROL Edit]** länk under **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Om du ändrar den här inställningen ändras inga Marketo-data. helt enkelt förändrar hur era rapporter fungerar. Detta kan återställas när som helst.

1. Välj ett alternativ och klicka på **[!UICONTROL Save]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Explicit]**: Endast kontakter med roller (standard).
   >
   >**[!UICONTROL Hybrid]**: Kontakter med roller, om sådana finns. Om det inte finns några tillgängliga används alla kontakter i kontona.
   >
   >**[!UICONTROL Implicit]**: Alla kontakter oavsett roll.

>[!CAUTION]
>
>När du använder **[!UICONTROL Implicit]** kommer Marketo alltid att undersöka alla kontakter som är kopplade till kontot, oavsett roll. **Marketo rekommenderar starkt att du använder [!UICONTROL Explicit] läge**. Använda [!UICONTROL Implicit] kan skapa falskt positiva resultat, dvs. människor som har beröm för en möjlighet trots att de inte har något verkligt inflytande på möjligheten. Använd [!UICONTROL Implicit] med försiktighet.
