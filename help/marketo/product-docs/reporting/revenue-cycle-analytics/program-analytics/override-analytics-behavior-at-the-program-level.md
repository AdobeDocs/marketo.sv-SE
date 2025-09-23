---
unique-page-id: 2360421
description: Åsidosätt analysbeteende på programnivå - Marketo Docs - produktdokumentation
title: Åsidosätt analysbeteende på programnivå
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Åsidosätt analysbeteende på programnivå {#override-analytics-behavior-at-the-program-level}

Du kan ställa in [analysbeteendet på adminnivå i kanalerna](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md), men du kan också åsidosätta det på programnivå. Så här:

1. Gå till området **[!UICONTROL Marketing Activities]**.

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Hitta och välj program.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. Dra **[!UICONTROL Setup]** till arbetsytan på fliken [!UICONTROL Analytics Behavior].

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Markera de [!UICONTROL Analytics Behavior] du vill ha.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **Inkluderande** - Det här alternativet ser till att programmet är tillgängligt för rapportering i intäktsutforskaren och analysprogram, oavsett om du har inkluderat en periodkostnad eller inte.
   >* **Operativ** - Det här alternativet resulterar i att programmet inte visas i någon av intäktsutforskarna eller analysatorerna.

   >[!NOTE]
   >
   >Standardbeteendet (om den här inställningen inte används) är att programmet endast inkluderas i analysen **ENDAST om det finns minst en periodkostnad**, även en med noll dollar tilldelat.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

Snyggt gjort! Nu vet ni hur man åsidosätter analysbeteendet på programnivå.

>[!NOTE]
>
>Ändringarna kommer att träda i kraft nästa dag och antingen göras tillgängliga eller dras ut ur intäktsutforskaren och analysatorerna.
