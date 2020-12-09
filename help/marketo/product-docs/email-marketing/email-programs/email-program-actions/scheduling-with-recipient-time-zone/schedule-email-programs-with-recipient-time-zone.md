---
unique-page-id: 12982903
description: Schemalägg e-postprogram med mottagartidszon - Marketo Docs - Produktdokumentation
title: Schemalägg e-postprogram med mottagartidszon
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---


# Schemalägg e-postprogram med mottagartidszon {#schedule-email-programs-with-recipient-time-zone}

Det finns två möjliga scenarier när du schemalägger ett e-postprogram när Mottagarens tidszon är aktiverad:

1. Schemalägger programmet att köras **inom** de närmaste 25 timmarna
1. Schemalägga att programmet ska köras **mer** än 25 timmar i framtiden (dvs. nästa vecka)

## Scenario 1: Inom 25 timmar {#scenario-within-hours}

Säg att du godkänner ett e-postprogram med Mottagarens tidszon aktiverad och en schemalagd leveranstid inom de närmaste 25 timmarna. Du kan ha personer i din smarta lista som bor i tidszoner där den schemalagda tiden redan har passerat.

I det här scenariot kan du bestämma vad du ska göra med den här delmängden kvalificerade personer. Klicka på kugghjulsikonen bredvid **Mottagarens tidszon** i rutan **Schema** i e-postprogrammet.

![](assets/image2017-12-5-10-3a46-3a42.png)

Detta ger dig två alternativ:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definition**
>
>* **Leverera följande dag i mottagarens tidszon**: Om e-postmeddelandet är schemalagt att skickas ut på tisdag kl. 9.00, kommer kvalificerade personer som bor i tidszoner där den schemalagda tiden redan har passerat att få e-postmeddelandet på *onsdagen* kl. 9.00.
   >
   >
* **Leverera med programmets standardinställda tid**: Om e-postmeddelandet är schemalagt att skickas ut på tisdag kl. 9.00, kommer kvalificerade personer som bor i tidszoner där den schemalagda tiden redan har passerat att få e-postmeddelandet *baserat på dina prenumerationstidszonsinställningar*. Så om dina [inställningar](../../../../../product-docs/administration/settings/select-your-language-locale-and-time-zone.md) för [prenumerationstidszon](../../../../../product-docs/administration/settings/set-default-location-settings-for-a-subscription.md) är PDT America/Los Angeles får dessa mottagare fortfarande e-postmeddelandet på tisdag klockan 9:00 PDT (oavsett tid i deras egna tidszoner).

>



>[!NOTE]
>
>[Läs mer](https://docs.marketo.com/display/DOCS/Understanding+Recipient+Time+Zone#UnderstandingRecipientTimeZone-CalculatingTimeZone) om hur Marketo beräknar tidszoner för mottagare.

Låt oss titta närmare på det här scenariot. Anta att du är i San Francisco och schemalägger ett mejl kl. 07:00 för en **9:00** -sändning. I din smarta lista finns det personer från följande områden:

* San Francisco
* Texas
* New York
* Italien

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 har redan gått i New York och Italien, så kvalificerade personer i dessa två tidszoner får e-postmeddelandet baserat på inställningarna för **tidszon**:

* **Leverera följande dag i mottagarens tidszon:** onsdag klockan 9:00 i respektive tidszon, **ELLER**

* **Leverera med programmets standardinställda tid**: Tisdag klockan 9:00 PDT (New York - 12:00 EDT och Italien - 18:00 CET).

När du godkänt programmet börjar det köras inom 15 minuter.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Även om programmet kommer att starta *processen* med att skicka e-post på 15 minuter, kommer e-post inte att *levereras* just då. Mottagarna får fortfarande e-post baserat på de **tidszonsinställningar** du väljer.

## Scenario 2: Mer än 25 timmar {#scenario-more-than-hours}

I det andra scenariot godkänner du ett e-postprogram med **mottagartidszon** aktiverad och en schemalagd leveranstid som är mer än 25 timmar framåt. I det här fallet kommer programmet att börja köras vid den schemalagda tidpunkten i den **tidigaste** tidszonen i världen (UTC + 14:00). Det kan finnas personer som är kvalificerade för din smarta lista i alla tidszoner över hela världen, så med början i den tidigaste tidszonen kan vi leverera e-postmeddelandet på det schemalagda datumet/den schemalagda tiden till alla mottagare i deras respektive tidszoner.

Startpunkt

Nu ska vi prata om hur [Head Start](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) fungerar med **mottagartidszon**. Vår befintliga funktion för Head Start kräver att programmet schemaläggs minst 12 timmar i förväg. Så vad betyder det för mottagarens tidszon? Kom ihåg att när Mottagarens tidszon är aktiverad börjar vi köra e-postprogrammet vid den schemalagda tidpunkten i den tidigaste tidszonen (UTC +14:00). För att aktivera **både** Head Start och Receipient Time Zone måste e-postprogram schemaläggas **minst 12 timmar före den schemalagda tiden i UTC +14:00.**

Det innebär att om du är i Amerika/Los Angeles och vill aktivera både Head Start och Receipient Time Zone måste du schemalägga programmet **34 timmar** i förväg. Hur kom vi till det här numret?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Kort och gott: e-postprogram som schemalagts med mottagartidszon måste börja köras vid den schemalagda tidpunkten i den tidigaste tidszonen (dvs. där den når midnatt först) för att varje tidszon ska få plats. Så om du schemalägger ett e-postprogram..

* **med en leveranstid *inom* 25 timmar** börjar programmet köras inom 15 minuter. Mottagare som redan har passerat den schemalagda tiden får e-postmeddelandet baserat på de tidszonsinställningar du har valt.
* **med en leveranstid på *mer* *än* 25 timmar i framtiden** börjar programmet köras vid den schemalagda tidpunkten i den tidigaste tidszonen (UTC +14:00).
* **med Head Start** börjar programmet bearbeta 12 timmar före den schemalagda tiden i den tidigaste tidszonen (UTC +14:00).

>[!CAUTION]
>
>Alla som avbeställer prenumerationen mellan den tidpunkt då du börjar skicka e-postmeddelandet och den dag det levereras får fortfarande e-postmeddelandet. Vi rekommenderar att du justerar avbeställningsmeddelandet så att det inte tar mer än 1-2 arbetsdagar att avsluta prenumerationen.

>[!MORELIKETHIS]
>
>* [Förstå mottagartidszon](understanding-recipient-time-zone.md)
>* [Head Start for Email Programs](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Avbryt leverans av e-postprogram som schemalagts med mottagartidszon](abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

>



