---
unique-page-id: 4719306
description: Dölj ett Salesforce-fält i Marketo Sync - Marketo Docs - produktdokumentation
title: Dölj ett Salesforce-fält från Marketo Sync
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 1%

---

# Dölj ett [!DNL Salesforce]-fält från Marketo Sync {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Alla fält i Salesforce är inte användbara för marknadsföring. Du kan optimera synkroniseringsprestanda genom att endast inkludera fält som du behöver. Så här kan du dölja ett fält för Marketo Engage.

1. Klicka på din namnmeny och välj **[!UICONTROL Setup]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Ange&quot;profiler&quot; i sökfältet och klicka på **[!UICONTROL Profiles]** under **[!UICONTROL Manage Users]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Klicka på synkroniseringsanvändarens profil.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Under avsnittet **[!UICONTROL Field-Level Security]** klickar du på **[!UICONTROL View]** bredvid objektet som innehåller målfältet.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Avmarkera kryssrutan **[!UICONTROL Visible]** bredvid fältet som du vill dölja. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Om fältet som du döljer i [!DNL Salesforce] redan har synkroniserats med Marketo måste du dölja det i Marketo också om du inte vill använda det.

   Så ja! Du kommer inte längre att se det här fältet i Marketo när nästa synkronisering är klar.

   >[!MORELIKETHIS]
   >
   >[Dölj och visa ett fält](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
