---
unique-page-id: 2360389
description: Gör ett program utan periodkostnad tillgängligt i Intresseutforskaren och analytiker - Marketo Docs - Produktdokumentation
title: Gör ett program utan periodkostnad tillgängligt i Intäktsutforskaren och analytiker
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---


# Gör ett program utan periodkostnad tillgängligt i intäktsutforskaren och analytiker {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Med Periodkostnader kan du definiera&quot;Hur mycket pengar&quot; och&quot;När&quot; för ett program. Detta visas i [utforskaren av intäktscykel](http://docs.marketo.com/display/docs/revenue+cycle+analytics) och [analysatorer](../../../../product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Vissa program kan behöva inkluderas även om de inte har en periodkostnad. Även om du kan ange 0 för periodkostnaden har vi gjort det enklare att ta med dessa program.

>[!NOTE]
>
>Program Analyzer bygger programmet Success per periodkostnad. Om det inte finns någon tillgänglig periodkostnad visas inte Programslutförande, oavsett programmets analysbeteende. Om analysbeteendet är inställt visas data för mått på affärsmöjligheter (säljmöjligheter, intäkter osv.).

1. Klicka på Taggar under avsnittet Admin.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Utöka dina kanaler och dubbelklicka på valfri kanal.

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Alla program som använder den här kanalen, oavsett periodkostnad, blir tillgängliga för intäktsutforskaren och analytiker. Ändringen träder i kraft följande dag.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Ändra Analytics-beteendet till Inclusive och klicka på Save.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Märkte du driftsalternativet? Det här gör tvärtom. Dessa program omfattas inte, oavsett periodkostnad.

Snyggt jobb! Nu kommer alla program som använder den ändrade kanalen att inkluderas i intäktsutforskaren och analytiker utan att man behöver betala en viss period.

>[!MORELIKETHIS]
>
>* [Åsidosätt analysbeteende på programnivå](override-analytics-behavior-at-the-program-level.md)

>



