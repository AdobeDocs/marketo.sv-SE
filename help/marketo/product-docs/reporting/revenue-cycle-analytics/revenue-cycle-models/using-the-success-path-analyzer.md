---
unique-page-id: 3571886
description: Using the Success Path Analyzer - Marketo Docs - Product Documentation
title: Använda sökvägsanalysen
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Använda sökvägsanalysen {#using-the-success-path-analyzer}

Använd en Success Path Analyzer för att utforska de specifika detaljer som återspeglar både flöde (mängd) och hastighet (hastighet, i antal dagar) för personer genom faserna i [intäktscykelmodellen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

>[!PREREQUISITES]
>
>[Skapa en lyckad sökvägsanalys](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. Gå till **Analytics** och välj din **Success Path Analyzer**.

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   Diagrammet till höger visar data i den markerade knappen till vänster. Som standard är detta Balans.

1. Klicka på **I flöde** om du vill visa hur många personer som kom in på scenen under den valda tidsramen.

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * Klicka på Utflöde om du vill visa hur många personer som har lämnat scenen.
   * Klicka på Konvertera % för att ange konverteringsgraden från detta till nästa steg.
   * Klicka på Avg Time för att se hur länge personer tillbringade den här scenen innan de flyttades till nästa fas.

1. Klicka på **Diagramåtgärder** > Jämför period för att jämföra data med en annan tidsram med samma längd.

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. Välj datumet **Från** för jämförelseperioden.

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   Datumet **Till** anges automatiskt så att det matchar längden på den ursprungliga tidsperioden.

1. Klicka på **Jämför**.

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. Diagrammet uppdateras med överlappande data för jämförelseperioden, i grönt.

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. Om du vill ändra tidsskalan för diagrammet klickar du på någon av knapparna **Diagram**: dag (standard), vecka och månad

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. För faser med servicenivåavtal (SLA) klickar du på **Diagramåtgärder** > **Visa SLA-förfallodatum** för att visa alla personer som någon gång har missat ett SLA-mål inom den angivna tidsramen.

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. Diagrammet uppdateras för att visa hur många SLA som förföll till betalning på varje nod, i orange.

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   De personer som visas med orange kan vara *eller kanske inte* fortfarande vara i SLA-scenen.

1. Klicka på **Diagramåtgärder** > **Visa tidigare SLA** om du vill visa alla personer med utgångna SLA-mål som fortfarande befinner sig i SLA-stadiet i slutet av den angivna tidsperioden.

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. Diagrammet uppdateras för att visa hur många SLA som förföll på varje nod, i orange.

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. Håll markören över bubblan om du vill läsa den specifika informationen för en datapunkt på en viss nod (datum).

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. Om du vill skriva ut diagrammet klickar du på **Diagramåtgärder** > **Skriv ut diagram**.

   ![](assets/image2015-6-12-17-3a53-3a34.png)

Analysatorn är här för att hjälpa dig att förstå hur modellen rör sig. I takt med att ni blir mer avancerade blir detta mycket viktigt för att strategiska era era marknadsföringssatsningar.
