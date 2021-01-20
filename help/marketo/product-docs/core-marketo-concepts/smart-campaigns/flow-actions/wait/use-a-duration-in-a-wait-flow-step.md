---
unique-page-id: 1146978
description: Använd en varaktighet i ett vänteflödessteg - Marketo Docs - Produktdokumentation
title: Använd en varaktighet i ett vänteflödessteg
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Använd en varaktighet i ett vänteflödessteg {#use-a-duration-in-a-wait-flow-step}

Du kan använda vänteflödessteget för att pausa en persons resa genom en smart kampanj under en viss tidsperiod. Du kan också ange villkor för veckodag och tidpunkt när den slutar.

1. Dra över flödessteget **Vänta** i den smarta kampanjen **Flöde**.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Ange hur länge du vill pausa.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Så ja! Flödet pausas under den angivna tidslängden. Om du vill ha avancerade alternativ klickar du på kugghjulsikonen till höger.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Ange veckodag då väntesteget ska avslutas.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Du kan också ange tiden. Klicka på **Spara**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Exempel**
   >
   >En person utlöser en smart kampanj på fredag kl. 17.00. Väntesteget är avancerat: 48 timmar och måste sluta på måndag-fredag kl. 9.
   >
   >Resultatet blir att personen fortsätter i flödet **måndag 9:00**. Detta är första M- F- datumet efter 48 timmar.

   >[!NOTE]
   >
   >Den varaktighet, de datum, tider och dagar som används baseras på din prenumerations tidszon.

   >[!MORELIKETHIS]
   >
   >* [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Använd en datumtoken i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

