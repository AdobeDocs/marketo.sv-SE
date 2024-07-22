---
unique-page-id: 4718683
description: Godkänna faser och tilldela leads till en intäktsmodell - Marketo Docs - produktdokumentation
title: Godkänna faser och tilldela leads till en intäktsmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Godkänna faser och tilldela leads till en intäktsmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Kom igång med din **intäktsmodell** genom att lägga till befintliga leads och skapa tilldelningsregler för nya leads.

## Godkännandesteg {#approving-stages}

Låt oss godkänna modellens faser innan du lägger till några leads.

1. Gå till området **Analyser**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Välj den modell vars stadier du vill godkänna.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Välj **Godkänn faser** under **Modellåtgärder**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Du får en varning. Klicka på **Tilldela leads**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Underbar! Låt oss gå vidare och tilldela dessa leads.

## Tilldela befintliga leads {#assigning-existing-leads}

[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för att identifiera leads för en fas i modellen i din lead-databas.

1. När du har [skapat din smarta lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) klickar du på fliken **Leads** .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicka på **Markera alla** för att välja leads.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öppna listrutan **Leadåtgärder** och välj **Special**. Klicka på **Ändra intäktsfas**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Välj rätt **modell** och rätt **scen**. Klicka på **Kör nu**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Upprepa tills alla dina leads har tilldelats de olika stegen i modellen.

Bra! Om du vill ange hur nya leads tilldelas till faser skapar du tilldelningsregler.

>[!NOTE]
>
>Om din modell är i läget Godkända stadier visas inga Change Revenue Stage-händelser i leads aktivitetsloggar. Om modellen är helt godkänd hoppas det här flödessteget över om du flyttar ett lead till samma fas som det befinner sig i.

## Nya leads: Skapa tilldelningsregler  {#new-leads-create-assignment-rules}

1. Klicka på **Marketo Home** igen och välj sedan **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicka på modellen i trädet, sedan på menyn **Modellåtgärder** och välj **Uppdragsregler**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Om dina tilldelningsregler innehåller fler än bara ett standardval klickar du på **Stage** och väljer sedan **Lägg till val**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exempel på tilldelningsregel {#example-assignment-rule}

Skapa en huvudpoängsregel om du vill tilldela nya leads med ett minimipoängtal till ett lämpligt steg.

1. Under **Om** väljer du **Leadpoäng**. Välj sedan **minst**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Ange **40** i fältet och välj **Försäljningslead** som en scen. Klicka på **Spara** för att slutföra.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Om du vill godkänna din modell kan du läsa hjälpsidan om **[Godkänna och avgodkänna en intäktsmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
