---
unique-page-id: 4719306
description: Dölj ett Salesforce-fält från Marketo Sync - Marketo Docs - Produktdokumentation
title: Dölj ett Salesforce-fält från markeringssynkroniseringen
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---


# Dölj ett Salesforce-fält från Marketo-synkronisering {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Alla fält i Salesforce är inte användbara för marknadsföring. Du kan optimera synkroniseringsprestanda genom att endast inkludera fält som du behöver. Så här kan du dölja ett fält för Marketo.

1. Klicka på menyn och välj **Inställningar**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Ange **profiler** i sökfältet och klicka på **Profiler** under **Hantera användare**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicka på synkroniseringsanvändarens profil.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Under avsnittet **Fältnivåsäkerhet** klickar du på **Visa** bredvid objektet som innehåller målfältet.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicka på **Redigera**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Avmarkera kryssrutan **Synlig** bredvid fältet som du vill dölja. Klicka på **Spara**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Om fältet som du döljer i Salesforce redan har synkroniserats med Marketo måste du dölja det i Marketo också om du inte vill använda det.

   Så ja! Du kommer inte längre att se det här fältet i Marketo när nästa synkronisering är klar.

   >[!MORELIKETHIS]
   >
   >[Dölja och visa ett fält](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
