---
unique-page-id: 1146978
description: Använd en varaktighet i ett vänteflödessteg - Marketo Docs - produktdokumentation
title: Använd en varaktighet i ett vänteflödessteg
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Använd en varaktighet i ett vänteflödessteg {#use-a-duration-in-a-wait-flow-step}

Du kan använda vänteflödessteget för att pausa en persons resa genom en smart kampanj under en viss tidsperiod. Du kan också ange villkor för veckodag och tidpunkt när den slutar.

1. I din smarta kampanj **[!UICONTROL Flow]** tabb, dra över **[!UICONTROL Wait]** flödessteg.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Ange hur länge du vill pausa.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Så ja! Flödet pausas under den angivna tidslängden. Om du vill ha avancerade alternativ klickar du på kugghjulsikonen till höger.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Ange veckodag då väntesteget ska avslutas.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Du kan också ange tiden. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >En person utlöser en smart kampanj på fredag kl. 17.00. Väntesteget är avancerat: 48 timmar och måste avslutas kl. 9.00 på Mon-Fri.
   >
   >Resultatet skulle bli att personen skulle fortsätta i flödet **Måndag 9**. Detta är första M- F- datumet efter 48 timmar.

   >[!NOTE]
   >
   >Den varaktighet, datum, tid och dagar som används baseras på din prenumerations tidszon.

   >[!MORELIKETHIS]
   >
   >* [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Använd en datumtoken i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
