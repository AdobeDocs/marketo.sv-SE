---
unique-page-id: 10097202
description: Head Start for Email Programs - Marketo Docs - Product Documentation
title: Head Start for Email Programs
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Head Start for Email Programs {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>* [Skapa ett e-postprogram](../../../../product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

>



När du väljer ett datum/tid för ett e-postprogram avgör det när programmet ska börja bearbeta. Om du vill att dina e-postmeddelanden ska starta vid den valda tidpunkten, får du det alternativet med Head Start genom att bearbeta programmet i förväg.

## Standardbörjan {#standard-head-start}

1. Klicka på **Marknadsföringsaktiviteter**.

   ![](assets/one-1.png)

1. Hitta och välj e-postprogram.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Det går inte att använda Head Start med A/B-testning.

1. Schemalägg e-postmeddelandet i rutan Schemalägg och markera sedan rutan **Starta**.

   ![](assets/three-1.png)

   När Head Start är valt börjar programmet bearbeta cirka 12 timmar före den schemalagda tiden. När bearbetningen startar är programmet låst.

   >[!CAUTION]
   >
   >Alla som slutar prenumerera efter programlås får fortfarande e-postmeddelandet. Vi rekommenderar att du justerar avbeställningsmeddelandet så att det inte tar mer än 1-2 arbetsdagar att avsluta prenumerationen.

1. Klicka på **Godkänn program**.

   ![](assets/four-1.png)

   Efter programgodkännandet finns det fyra olika statusar som du kan se på godkännandepanelen.

   * **Väntar på att köras:** När programmet har godkänts.
   * **Bearbetningen har startats, väntar på att köras:** Bearbetningen pågår.
   * **Bearbetningen är klar, väntar på att köras:** Bearbetningen har slutförts, e-postmeddelandet väntar nu på att den schemalagda tiden ska startas.
   * **Slutförd:** Programmet har slutförts.

   >[!TIP]
   >
   >Vill du avbryta efter att programmet har låsts men innan e-postmeddelandet skickas? Inga problem! Klicka bara på **Avbryt program** längst ned till höger i rutan Godkännande.

   >[!NOTE]
   >
   >Om du inte godkänner ditt e-postprogram inom 12 timmar före den schemalagda körtiden, men sedan ändrar dig, måste du välja ett nytt datum/tid som är minst 12 timmar före när du godkänner det.

## Startpunkt med mottagartidszon {#head-start-with-recipient-time-zone}

Vår befintliga funktion för Head Start kräver att programmet schemaläggs minst 12 timmar i förväg. Vad innebär det för mottagartidszon? Kom ihåg att när mottagarens tidszon är aktiv börjar vi köra e-postprogrammet vid midnatt i den tidigaste tidszonen (UTC +14:00). Om du vill aktivera **både** Starttidszon för HEAD och Mottagarens tidszon måste programmen schemaläggas **minst 12 timmar före den tidigaste tidszonen (UTC +14:00**.)

Det innebär att om du är i Amerika/Los Angeles och vill aktivera både Head Start och Receipient Time Zone måste du schemalägga programmet **34 timmar** i förväg. Hur kom vi till det här numret?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Läs ](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) mer om hur du schemalägger e-postprogram med mottagartidszon.

>[!MORELIKETHIS]
>
>* [Schemalägg ditt e-postprogram](schedule-your-email-program.md)
>* [Schemalägg e-postprogram med mottagartidszon](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Förstå mottagartidszon](scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

>



