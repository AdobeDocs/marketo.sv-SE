---
unique-page-id: 1146997
description: Använd en datumtoken i ett vänteflödessteg - Marketo Docs - produktdokumentation
title: Använd en datumtoken i ett vänteflödessteg
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Använd en datumtoken i ett vänteflödessteg {#use-a-date-token-in-a-wait-flow-step}

Du kan använda steget Väntflöde för att pausa en persons resa genom en smart kampanj tills ett visst datum som använder en datumtoken. Du kan också ändra slutdatumet med ett antal dagar.

>[!NOTE]
>
>Detta gäller endast utlösarkampanjer. Du kan inte använda den här funktionen i gruppkampanjer.

1. I din smarta kampanj **[!UICONTROL Flow]** tabb, dra över **[!UICONTROL Wait]** flödessteg.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Klicka på kugghjulet.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Från **[!UICONTROL Type]** nedrullningsbar meny, välja **[!UICONTROL Date Token]**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Välj en datumtoken som anger när vänsteget ska avslutas:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Markera kryssrutan om du vill vänta till nästa årsdag för datumet som infaller under det aktuella eller nästa kalenderår.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Använd det här alternativet för datumtoken som refererar till tidigare datum, t.ex. en födelsedag eller ett kontraktstartdatum.

1. Du kan också ändra slutdatumet med ett visst antal dagar.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Du kan också ange antalet dagar med en `{{lead.` eller `{{company.` token som representerar ett heltalsfält, eller en `{{my.` token av nummertyp.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Använd en varaktighet i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
