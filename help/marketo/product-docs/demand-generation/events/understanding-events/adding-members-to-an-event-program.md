---
unique-page-id: 37355758
description: Lägga till medlemmar i ett Event Program - Marketo Docs - produktdokumentation
title: Lägga till medlemmar i ett händelseprogram
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Lägga till medlemmar i ett händelseprogram {#adding-members-to-an-event-program}

Den här artikeln gäller endast användare som använder Event Cap- eller Event-mål.

>[!CAUTION]
>
>Om du importerar en lista med personer direkt till ett Event Program hindras dessa poster från att räknas i de faktiska registreringarna i rapporten för målspårning och i rapporten om händelseavslut. Följ instruktionerna nedan för att försäkra dig om att dina poster räknas.

1. Skapa och [lägga till personer i en statisk lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Skapa en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. I den smarta listan för den smarta kampanj du skapade i steg två söker du efter och lägger till **List-medlem** filter.

   ![](assets/three.png)

1. Sök efter och markera listan som du skapade i steg 1.

   ![](assets/four.png)

1. I Flöde söker du efter och lägger till **Ändra programstatus** flödessteg.

   ![](assets/five.png)

1. Hitta och välj ditt Event Program.

   ![](assets/six.png)

1. Välj önskad status.

   ![](assets/seven.png)

1. Klicka på fliken Schema **Kör en gång**.

   ![](assets/eight.png)

1. Välj **Kör nu** och klicka **Kör**.

   ![](assets/nine.png)

1. När den smarta kampanjen körs läggs medlemmarna till i programmet och räknas i beräkningarna för målspårning och händelseavståndsprognos.
