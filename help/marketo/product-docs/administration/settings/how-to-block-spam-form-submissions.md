---
description: Blockera inskickning av skräppostformulär - Marketo Docs - produktdokumentation
title: Blockera inskickning av skräppostformulär
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Så här blockerar du inskickade skräppostformulär {#how-to-block-spam-form-submissions}

Formuläröverföringar med en ogiltig eller saknad kontrollsumma (vanligtvis från bot) kan ofta generera falsk statistik. Så här förhindrar du det.

>[!CAUTION]
>
>Den här funktionen avvisar formuläröverföringar som gjorts med programmatiska POST:er till leadCapture/save2-slutpunkten. Om ni använder en integrering som skickar in blanketter till Marketo med den metoden blockerar den här funktionen dessa. Användning av leadCapture/save2 som API eller direkt inskickning av programmatiska formulär stöds inte heller. Se till att ditt företag endast skickar in formulär med: Formulärresurser, inbäddad formulärkod, Forms2.js API eller Submit Form REST API.

1. Klicka på **Admin**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Klicka på **Resurs Chest**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. Bredvid **Personhämtning - Ignorera ogiltiga kontrollsummevärden** klickar du på **Redigera**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Markera kryssrutan **Aktiverad** och klicka på **Spara**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>När du aktiverar den här funktionen kan du se en nedgång i formuläraktiviteten när falska siffror filtreras bort.
