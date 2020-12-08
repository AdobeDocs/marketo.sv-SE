---
unique-page-id: 12983291
description: Förstå mottagarens tidszon - Marketo Docs - Produktdokumentation
title: Förstå mottagartidszon
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---


# Förstå mottagartidszon {#understanding-recipient-time-zone}

E-post- och engagemangsprogram kan konfigureras så att de levereras enligt mottagarnas tidszoner, vilket eliminerar behovet av att skapa flera program - skicka en gång och Marketo lagrar e-postmeddelandet automatiskt tills rätt lokal tid.

>[!NOTE]
>
>Mottagarens tidszon fungerar för närvarande **bara** med e-postinnehåll. Det fungerar inte med standardprogram för engagemang.

## E-postprogram {#email-programs}

Det finns två primära scenarier när du [schemalägger ett e-postprogram](schedule-email-programs-with-recipient-time-zone.md):

1. Schemalägger programmet att köras inom de närmaste 25 timmarna.
1. Schemalägger programmet att köras mer än 25 timmar i framtiden (dvs. nästa vecka).

För att varje tidszon ska få plats börjar e-postprogram som schemalagts med mottagartidszon att köras vid midnatt i den **första/tidigaste** tidszonen i världen (UTC +14:00).

## Engagement Programs {#engagement-programs}

När du [schemalägger en interaktionsprogramström](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) och Mottagarens tidszon är aktiv, kommer programsändningen att börja köras vid midnatt i UTC +14:00. Vi kräver att du schemalägger den första omgången minst 25 timmar i framtiden (24 timmar + lite tid för att komma igång med kampanjen) eftersom folk kan kvalificera sig för omsändningen i varje tidszon över hela världen. Bearbetningen påbörjas nu i UTC +14:00 garanterar att vi skickar e-postmeddelandet på schemalagt datum och tid för alla som är kvalificerade för den här sändningen.

## Beräknar tidszon {#calculating-time-zone}

Marketo beräknar tidszonen baserat på en persons ort, delstat, land eller postnummer. Om vi inte kan beräkna någons tidszon utifrån dessa värden, återgår vi till fälten Inced, Incederad stat, Incederat land och Postnummer.

Om vi har **only **Country eller **only** State available:

* För länder med tre eller färre tidszoner väljer vi den mellersta tidszonen.
* För lägen med två tidszoner väljer vi det tidigare av de två.

Om vi fortfarande inte kan fastställa någons tidszon från någon kombination av dessa fält, kommer vi **inte** att tilldela någon tidszon och e-postmeddelandet levereras baserat på din Marketo-prenumerationstidszon. Om ditt program är schemalagt till 9:00 PDT får personer utan tidszon e-postmeddelandet kl. 9:00 PDT.

>[!NOTE]
>
>Marketo beräknar automatiskt om en persons tidszon när något av ovanstående inmatningsfält ändras.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Schemalägg e-postprogram med mottagartidszon](schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start for Email Programs](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Schemalägg engagemangsprogram med mottagartidszon](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



