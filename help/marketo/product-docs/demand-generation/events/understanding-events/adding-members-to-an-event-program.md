---
unique-page-id: 37355758
description: Lägga till medlemmar i ett Event Program - Marketo Docs - Produktdokumentation
title: Lägga till medlemmar i ett händelseprogram
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Lägga till medlemmar i ett händelseprogram {#adding-members-to-an-event-program}

Den här artikeln gäller endast användare som använder Event Cap- eller Event-mål.

>[!CAUTION]
>
>Om du importerar en lista med personer direkt till ett Event Program hindras dessa poster från att räknas i de faktiska registreringarna i rapporten för målspårning och i rapporten om händelseavslut. Följ instruktionerna nedan för att försäkra dig om att dina poster räknas.

1. Skapa och [lägg till personer i en statisk lista](http://docs.marketo.com/x/ecKt).
1. [Skapa en smart kampanj](http://docs.marketo.com/x/M4AR).
1. I den smarta listan för den smarta kampanj du skapade i steg två söker du efter och lägger till **medlemslistan** .

   ![](assets/three.png)

1. Sök efter och markera listan som du skapade i steg 1.
1. ![](assets/four.png)

1. I Flow söker du efter och lägger till **Ändra programstatus** .
1. ![](assets/five.png)

1. Hitta och välj ditt Event Program.

   ![](assets/six.png)

1. Välj önskad status.

   ![](assets/seven.png)

1. Klicka på **Kör en gång** på fliken Schema.
1. ![](assets/eight.png)

1. Välj **Kör nu** och klicka på **Kör**.
1. ![](assets/nine.png)

1. När den smarta kampanjen körs läggs medlemmarna till i programmet och räknas i beräkningarna för målspårning och händelseavståndsprognos.

