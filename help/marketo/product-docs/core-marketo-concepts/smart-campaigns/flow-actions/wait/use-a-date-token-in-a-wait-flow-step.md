---
unique-page-id: 1146997
description: Använd en datumtoken i ett vänteflödessteg - Marketo Docs - produktdokumentation
title: Använd en datumtoken i ett vänteflödessteg
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Använd en datumtoken i ett vänteflödessteg {#use-a-date-token-in-a-wait-flow-step}

Du kan använda steget Väntflöde för att pausa en persons resa genom en smart kampanj tills ett visst datum som använder en datumtoken. Du kan också ändra slutdatumet med ett antal dagar.

>[!NOTE]
>
>Detta gäller endast utlösarkampanjer. Du kan inte använda den här funktionen i gruppkampanjer.

1. Dra över flödessteget **[!UICONTROL Flow]** på fliken Smart Campaign **[!UICONTROL Wait]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Klicka på kugghjulet.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. Välj **[!UICONTROL Type]** i listrutan **[!UICONTROL Date Token]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Välj en [!UICONTROL Date token] som du vill ange när steget Vänta ska avslutas:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Markera kryssrutan om du vill vänta till nästa årsdag för datumet som infaller under det aktuella eller nästa kalenderår.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Använd det här alternativet för datumtoken som refererar till tidigare datum, t.ex. en födelsedag eller ett kontraktstartdatum.

1. Du kan också ändra slutdatumet med ett visst antal dagar.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >Du kan också ange antalet dagar med en `{{lead.`- eller `{{company.`-token som representerar ett heltalsfält eller en `{{my.`-token av taltyp.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Använd en varaktighet i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
