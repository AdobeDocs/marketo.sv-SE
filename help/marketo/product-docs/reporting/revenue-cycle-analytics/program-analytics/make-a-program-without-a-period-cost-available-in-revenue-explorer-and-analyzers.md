---
unique-page-id: 2360389
description: Gör ett program utan periodkostnad tillgängligt i Intresseutforskaren och analytiker - Marketo Docs - Produktdokumentation
title: Gör ett program utan periodkostnad tillgängligt i Intäktsutforskaren och analytiker
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Gör ett program utan periodkostnad tillgängligt i Intäktsutforskaren och analytiker {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Med Periodkostnader kan du definiera&quot;Hur mycket pengar&quot; och&quot;När&quot; för ett program. Detta visas i intäktscykelutforskaren och [analysatorer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Vissa program kan behöva inkluderas även om de inte har en periodkostnad. Även om du kan ange 0 för periodkostnaden har vi gjort det enklare att ta med dessa program.

>[!NOTE]
>
>Program Analyzer bygger programmet Success per periodkostnad. Om det inte finns någon tillgänglig periodkostnad visas inte Programslutförande, oavsett programmets analysbeteende. Om analysbeteendet är inställt visas data för mått på affärsmöjligheter (säljmöjligheter, intäkter osv.).

1. Klicka på under Admin **Taggar**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Utöka dina kanaler och dubbelklicka på valfri kanal.

   >[!NOTE]
   >
   >Alla program som använder den här kanalen, oavsett periodkostnad, blir tillgängliga för intäktsutforskaren och analytiker. Ändringen träder i kraft följande dag.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Ändra analysbeteendet till Inkluderande och klicka på **Spara**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Märkte du driftsalternativet? Det här gör tvärtom. Dessa program omfattas inte, oavsett periodkostnad.

Snyggt jobb! Nu kommer alla program som använder den ändrade kanalen att inkluderas i intäktsutforskaren och analytiker utan att man behöver betala en viss period.

>[!MORELIKETHIS]
>
>[Åsidosätt analysbeteende på programnivå](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
