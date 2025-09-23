---
unique-page-id: 12982903
description: Schemalägg e-postprogram med mottagartidszon - Marketo Docs - produktdokumentation
title: Schemalägg e-postprogram med mottagartidszon
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Schemalägg e-postprogram med mottagartidszon {#schedule-email-programs-with-recipient-time-zone}

Det finns två möjliga scenarier när du schemalägger ett e-postprogram när Mottagarens tidszon är aktiverad:

1. Schemalägger programmet att köra **inom** de kommande 25 timmarna
1. Schemalägger programmet att köra **mer** än 25 timmar i framtiden (det vill säga nästa vecka)

## Scenario 1: Inom 25 timmar {#scenario-within-hours}

Säg att du godkänner ett e-postprogram med Mottagarens tidszon aktiverad och en schemalagd leveranstid inom de närmaste 25 timmarna. Du kan ha personer i din smarta lista som bor i tidszoner där den schemalagda tiden redan har passerat.

I det här scenariot kan du bestämma vad du ska göra med den här delmängden kvalificerade personer. Klicka på kugghjulsikonen bredvid **[!UICONTROL Recipient Time Zone]** i rutan **[!UICONTROL Schedule]** i e-postprogrammet.

![](assets/image2017-12-5-10-3a46-3a42.png)

Detta ger dig två alternativ:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definition**
>
>* **[!UICONTROL Deliver the following day in the recipient's time zone]**: Om e-postmeddelandet är schemalagt att skickas på tisdag klockan 9:00am får kvalificerade personer som bor i tidszoner där den schemalagda tiden redan har passerat e-postmeddelandet *onsdag* kl. 9:00am.
>
>* **[!UICONTROL Deliver using the program's default set time]**: Om e-postmeddelandet är schemalagt att skickas på tisdag kl. 9:00am får kvalificerade personer som bor i tidszoner där den schemalagda tiden redan har passerat e-postmeddelandet *baserat på dina inställningar för prenumerationstidszon*. Om dina [prenumerationstidszonsinställningar](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) är inställda på PDT America/Los Angeles får dessa mottagare fortfarande e-postmeddelandet på tisdag klockan 9:00am PDT (oavsett tid i deras egna tidszoner).

>[!NOTE]
>
>[Läs mer](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) om hur Marketo beräknar tidszoner för mottagare.

Låt oss titta närmare på det här scenariot. Anta att du är i San Francisco och schemalägger ett e-postmeddelande på 7:00am för en **9:00am**-sändning. I din smarta lista finns det personer från följande områden:

* San Francisco
* Texas
* New York
* Italien

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am har redan passerat i New York och Italien, så kvalificerade personer i dessa två tidszoner får e-postmeddelandet baserat på **tidszonsinställningarna**:

* **[!UICONTROL Deliver the following day in the recipient's time zone]:** onsdag klockan 9:00am i deras respektive tidszoner, **OR**

* **[!UICONTROL Deliver using the program's default set time]**: Tisdag klockan 9:00am PDT (New York - 12:00pm EDT and Italy - 6:00pm CET).

När du godkänt programmet börjar det köras inom 15 minuter.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Även om programmet startar *processen* för att skicka e-post om 15 minuter, kommer e-post inte att *levereras* vid den tidpunkten. Mottagarna får fortfarande e-post baserat på den **[!UICONTROL Time Zone Settings]** du väljer.

## Scenario 2: Mer än 25 timmar {#scenario-more-than-hours}

I det andra scenariot godkänner du ett e-postprogram med **[!UICONTROL Recipient Time Zone]** aktiverat och en schemalagd leveranstid som är mer än 25 timmar framöver. I det här fallet börjar programmet köras vid den schemalagda tidpunkten i den **tidigaste** tidszonen i världen (UTC + 14:00). Det kan finnas personer som är kvalificerade för din smarta lista i alla tidszoner över hela världen, så med början i den tidigaste tidszonen kan vi leverera e-postmeddelandet på det schemalagda datumet/den schemalagda tiden till alla mottagare i deras respektive tidszoner.

**Startpunkt**

Låt oss nu prata om hur [[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) fungerar med **[!UICONTROL Recipient Time Zone]**. Vår befintliga funktion för Head Start kräver att programmet schemaläggs minst 12 timmar i förväg. Så vad betyder det för mottagarens tidszon? Kom ihåg att när Mottagarens tidszon är aktiverad börjar vi köra e-postprogrammet vid den schemalagda tidpunkten i den tidigaste tidszonen (UTC +14:00). Om du vill aktivera **både** Starttid och Mottagarens tidszon måste e-postprogram schemaläggas **minst 12 timmar före den schemalagda tiden i UTC +14:00.**

Det innebär att om du befinner dig i Amerika/Los Angeles och vill aktivera både Head Start och Receipient Time Zone måste du schemalägga programmet **34 timmar** i förväg. Hur kom vi till det här numret?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Kort och gott: e-postprogram som schemalagts med mottagartidszon måste börja köras vid den schemalagda tidpunkten i den tidigaste tidszonen (d.v.s. där den når midnatt först) för att varje tidszon ska få plats. Så om du schemalägger ett e-postprogram..

* **med en leveranstid på *inom* 25 timmar** börjar programmet köras inom 15 minuter. Mottagare som redan har passerat den schemalagda tiden får e-postmeddelandet baserat på de tidszonsinställningar du har valt.
* **med en leveranstid på *mer än* 25 timmar i framtiden**, kommer programmet att börja köras vid den schemalagda tidpunkten i den tidigaste tidszonen (UTC +14:00).
* **med Head Start** startar programmet bearbetningen 12 timmar före den schemalagda tiden i den tidigaste tidszonen (UTC +14:00).

>[!CAUTION]
>
>Alla som avbeställer prenumerationen mellan den tidpunkt då du börjar skicka e-postmeddelandet och den dag det levereras får fortfarande e-postmeddelandet. Vi rekommenderar att du justerar avbeställningsmeddelandet för att förklara att det kan ta 1-2 arbetsdagar innan du säger upp prenumerationen.

>[!MORELIKETHIS]
>
>* [Förstå mottagarens tidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Startsida för e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Avbryt leverans av e-postprogram som schemalagts med mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
