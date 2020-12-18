---
unique-page-id: 4718683
description: Godkänna faser och tilldela leads till en intäktsmodell - Marketo Docs - produktdokumentation
title: Godkänna faser och tilldela leads till en intäktsmodell
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Godkänna faser och tilldela leads till en intäktsmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Få igång dina **intäkter** **Modell** genom att lägga till befintliga leads och skapa tilldelningsregler för nya leads.

## Godkänner steg {#approving-stages}

Låt oss godkänna modellens faser innan du lägger till några leads.

1. Gå till **Analytics **området.** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Markera modellen vars stadier du vill godkänna.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Under **Modellåtgärder** väljer du **Godkänn** **Steg**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Du får en varning; klicka på **Tilldela leads**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Underbar! Låt oss gå vidare och tilldela leads.

## Tilldela befintliga leads {#assigning-existing-leads}

[Skapa en smart ](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) lista för att identifiera leads för ett steg i modellen i din lead-databas.

1. När du har [skapat din smarta lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) klickar du på fliken **Leads**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicka på **Markera alla** för att välja leads.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öppna listrutan **Leadåtgärder** och välj **Special**. Klicka på **Ändra intäktsstadium**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Välj rätt **modell** och rätt **scen**. Klicka på **Kör nu**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Upprepa tills alla dina leads har tilldelats de olika stegen i modellen.

Bra! Om du vill ange hur nya leads tilldelas till faser skapar du tilldelningsregler.

>[!NOTE]
>
>Om din modell är i läget Godkända stadier visas inga Change Revenue Stage-händelser i leads aktivitetsloggar. Om modellen är helt godkänd hoppas det här flödessteget över om du flyttar ett lead till samma fas som det befinner sig i.

## Nya leads: Skapa tilldelningsregler {#new-leads-create-assignment-rules}

1. Klicka på* Marketo Home** igen och välj sedan **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exempel på tilldelningsregel {#example-assignment-rule}

Skapa en huvudpoängsregel om du vill tilldela nya leads med ett minimipoängtal till ett lämpligt steg.

1. Under **Om** väljer du **Leadpoäng**. Välj sedan **minst**.
` ![](assets/image2015-4-29-13-3a27-3a8.png)

   `

1. Ange **40** i fältet och välj **Försäljningslead** som en scen. Klicka på **Spara** för att slutföra.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Om du vill godkänna din modell kan du läsa hjälpsidan på ** [Godkänna och avgodkänna en intäktsmodell](approve-unapprove-a-revenue-model.md)**.

