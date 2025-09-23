---
unique-page-id: 4718683
description: Godkänna faser och tilldela leads till en intäktsmodell - Marketo Docs - produktdokumentation
title: Godkänna faser och tilldela leads till en intäktsmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 1%

---

# Godkänna faser och tilldela leads till en intäktsmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Kom igång med din **intäktsmodell** genom att lägga till befintliga leads och skapa tilldelningsregler för nya leads.

## Godkännandesteg {#approving-stages}

Låt oss godkänna modellens faser innan du lägger till några leads.

1. Gå till området **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Välj den modell vars stadier du vill godkänna.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Välj **[!UICONTROL Model Actions]** under **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Du får en varning. Klicka på **[!UICONTROL Assign Leads]**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Underbar! Låt oss gå vidare och tilldela dessa leads.

## Tilldela befintliga leads {#assigning-existing-leads}

[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för att identifiera leads för en fas i modellen i din lead-databas.

1. När du har [skapat din smarta lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) klickar du på fliken **[!UICONTROL Leads]**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicka på **[!UICONTROL Select All]** för att välja leads.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öppna listrutan **[!UICONTROL Lead Actions]** och välj **[!UICONTROL Special]**. Klicka på **[!UICONTROL Change Revenue Stage...]**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Välj rätt **[!UICONTROL Model]** och rätt **[!UICONTROL Stage]**. Klicka på **[!UICONTROL Run Now]**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Upprepa tills alla dina leads har tilldelats de olika stegen i modellen.

Bra! Om du vill ange hur nya leads tilldelas till faser skapar du tilldelningsregler.

>[!NOTE]
>
>Om din modell är i läget Godkända stadier visas inga Change Revenue Stage-händelser i leads aktivitetsloggar. Om modellen är helt godkänd hoppas det här flödessteget över om du flyttar ett lead till samma fas som det befinner sig i.

## Nya leads: Skapa tilldelningsregler  {#new-leads-create-assignment-rules}

1. Klicka på **Marketo Home** igen och välj sedan **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicka på modellen i trädet, välj **[!UICONTROL Model Actions]** på menyn **[!UICONTROL Assignment Rules]**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Om dina tilldelningsregler innehåller fler än ett standardalternativ klickar du på **[!UICONTROL Stage]** och väljer sedan **[!UICONTROL Add Choice]**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exempel på tilldelningsregel {#example-assignment-rule}

Skapa en [!UICONTROL Lead Score]-regel för att tilldela nya leads med ett minimipoängvärde till ett lämpligt steg.

1. Under **[!UICONTROL If]** väljer du **[!UICONTROL Lead Score]**. Välj sedan **[!UICONTROL at least]**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Ange **40** i fältet och välj **[!UICONTROL Sales Lead]** som [!UICONTROL Stage]. Klicka på **[!UICONTROL Save]** för att slutföra.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Om du vill godkänna din modell kan du läsa hjälpsidan om **[Godkänna och avgodkänna en intäktsmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
