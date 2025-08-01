---
unique-page-id: 2360217
description: Ändra attribueringsinställningar för analys - Marketo Docs - produktdokumentation
title: Ändra attributinställningar för analys
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Ändra attributinställningar för analys {#change-attribution-settings-for-analytics}

Ni kan ändra det sätt på vilket Marketo knyter kontakter till möjligheter till första- och flerberöringsattribuering, konverteringsstatistik för leads och flaggan för marknadspåverkade affärsmöjligheter.

De här inställningarna påverkar [!UICONTROL Revenue Explorer] rapporter under områdena [Programsäljprojektsanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Affärsmöjlighetsanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) och Leadanalys. Detta påverkar även rapporten [!UICONTROL Program Analyzer].

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Klicka på **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Klicka på länken **[!UICONTROL Edit]** under **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Om du ändrar den här inställningen ändras inga Marketo-data, utan det är bara hur dina rapporter körs. Detta kan återställas när som helst.

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
>När du använder **[!UICONTROL Implicit]** kommer Marketo alltid att undersöka alla kontakter som är kopplade till kontot, oavsett roll. **Marketo rekommenderar starkt [!UICONTROL Explicit] mode**. Om du använder [!UICONTROL Implicit] kan det skapa falskt positiva effekter, dvs. personer som har krediter för en affärsmöjlighet trots att de inte har något verkligt inflytande på affärsmöjligheten. Använd [!UICONTROL Implicit] med försiktighet.
