---
unique-page-id: 10097202
description: Head Start for Email Programs - Marketo Docs - Product Documentation
title: Head Start for Email Programs
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Head Start for Email Programs {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Skapa ett e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

När du väljer ett datum/tid för ett e-postprogram avgör det när programmet ska börja bearbeta. Om du vill att dina e-postmeddelanden ska starta vid den valda tidpunkten, får du det alternativet med Head Start genom att bearbeta programmet i förväg.

## Standardbörjan {#standard-head-start}

1. Klicka på **[!UICONTROL Marketing Activities]**.

   ![](assets/one-1.png)

1. Hitta och välj e-postprogram.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Det går inte att använda Head Start med A/B-testning.

1. Schemalägg e-postmeddelandet i rutan [!UICONTROL Schedule] och markera sedan rutan **[!UICONTROL Head Start]**.

   ![](assets/three-1.png)

   När [!UICONTROL Head Start] är markerat börjar programmet bearbeta cirka 12 timmar före den schemalagda tiden. När bearbetningen startar är programmet låst.

   >[!CAUTION]
   >
   >Alla som slutar prenumerera efter programlås får fortfarande e-postmeddelandet. Vi rekommenderar att du justerar avbeställningsmeddelandet så att det inte tar mer än 1-2 arbetsdagar att avsluta prenumerationen.

1. Klicka på **[!UICONTROL Approve Program]**.

   ![](assets/four-1.png)

   Efter programgodkännandet finns det fyra olika statusar som du kan se på godkännandepanelen.

   * **[!UICONTROL Waiting to run]:** När programmet har godkänts.
   * **[!UICONTROL Processing started, waiting to run]:** Bearbetning pågår.
   * **[!UICONTROL Processing finished, waiting to run]:** Bearbetningen har slutförts, e-post väntar nu på att den schemalagda tiden ska startas.
   * **[!UICONTROL Finished]:** Programmet har slutförts.

   >[!TIP]
   >
   >Vill du avbryta efter att programmet har låsts men innan e-postmeddelandet skickas? Inga problem! Klicka bara på **[!UICONTROL Abort Program]** längst ned till höger i rutan Godkännande.

   >[!NOTE]
   >
   >Om du inte godkänner ditt e-postprogram inom 12 timmar före den schemalagda körtiden, men sedan ändrar dig, måste du välja ett nytt datum/tid som är minst 12 timmar före när du godkänner det.

## Startpunkt med mottagartidszon {#head-start-with-recipient-time-zone}

Vår befintliga funktion för Head Start kräver att programmet schemaläggs minst 12 timmar i förväg. Vad innebär det för mottagarens tidszon? Kom ihåg att när mottagarens tidszon är aktiv börjar vi köra e-postprogrammet vid midnatt i den tidigaste tidszonen (UTC +14:00). Om du vill aktivera **både** Start- och mottagartidszon för både  måste programmen schemaläggas **minst 12 timmar före den tidigaste tidszonen (UTC +14:00**).

Det innebär att om du befinner dig i Amerika/Los Angeles och vill aktivera både Head Start och Receipient Time Zone måste du schemalägga programmet **34 timmar** i förväg. Hur kom vi till det här numret?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Läs mer](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) om hur du schemalägger e-postprogram med mottagartidszon.

>[!MORELIKETHIS]
>
>* [Schemalägg ditt e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Schemalägg e-postprogram med mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Förstå mottagarens tidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
