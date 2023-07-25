---
unique-page-id: 4718683
description: Godkänna faser och tilldela leads till en intäktsmodell - Marketo Docs - produktdokumentation
title: Godkänna faser och tilldela leads till en intäktsmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Godkänna faser och tilldela leads till en intäktsmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Skaffa **Intäktsmodell** komma igång genom att lägga till befintliga leads, skapa tilldelningsregler för nya leads.

## Godkännandesteg {#approving-stages}

Låt oss godkänna modellens faser innan du lägger till några leads.

1. Gå till **Analyser** område.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Markera modellen vars stadier du vill godkänna.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Under **Modellåtgärder**, markera **Godkänn steg**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Du får en varning; klicka **Tilldela leads**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Underbar! Låt oss gå vidare och tilldela leads.

## Tilldela befintliga leads {#assigning-existing-leads}

[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) för att identifiera leads för ett steg i modellen i din Lead-databas.

1. När du har [skapade din smarta lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)klickar du på **Leads** -fliken.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicka **Markera alla** för att välja leads.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öppna **Leadåtgärder** nedrullningsbar meny och välj **Special**. Klicka **Ändra intäktsfas**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Välj rätt **Modell** och rätt **Scen**. Klicka **Kör nu**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Upprepa tills alla dina leads har tilldelats de olika stegen i modellen.

Bra! Om du vill ange hur nya leads tilldelas till faser skapar du tilldelningsregler.

>[!NOTE]
>
>Om din modell är i läget Godkända stadier visas inga Change Revenue Stage-händelser i leads aktivitetsloggar. Om modellen är helt godkänd hoppas det här flödessteget över om du flyttar ett lead till samma fas som det befinner sig i.

## Nya leads: Skapa tilldelningsregler  {#new-leads-create-assignment-rules}

1. Klicka **Marketo Home** igen, välj **Analyser**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicka på modellen i trädet och sedan på **Modellåtgärder** meny, välja **Uppdragsregler**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Om dina uppdragsregler innehåller mer än bara ett standardval klickar du på **Scen**, gör ditt val och klickar sedan på **Lägg till alternativ**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exempel på tilldelningsregel {#example-assignment-rule}

Skapa en huvudpoängsregel om du vill tilldela nya leads med ett minimipoängtal till ett lämpligt steg.

1. Under **If**, markera **Leadpoäng**. Välj sedan **minst**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Retur **40** i fältet och välj **Försäljningslead** som en scen. Klicka **Spara** för att slutföra.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Om du vill godkänna din modell kan du läsa hjälpsidan på **[Godkänna och avgodkänna en intäktsmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
