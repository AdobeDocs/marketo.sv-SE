---
unique-page-id: 12983291
description: Understanding Recipient Time Zone - Marketo Docs - Product Documentation
title: Förstå mottagartidszon
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Förstå mottagartidszon {#understanding-recipient-time-zone}

E-post- och engagemangsprogram kan konfigureras så att de levereras enligt mottagarnas tidszoner, vilket eliminerar behovet av att skapa flera program - skicka en gång och Marketo lagrar automatiskt e-postmeddelandet till rätt lokal tid.

>[!NOTE]
>
>Mottagarens tidszon fungerar för närvarande **endast** med e-postinnehåll. Det fungerar inte med standardprogram för engagemang.

## E-postprogram {#email-programs}

Det finns två primära scenarier när [schemalägga ett e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Schemalägger programmet att köras inom de närmaste 25 timmarna.
1. Schemalägger programmet att köras mer än 25 timmar i framtiden (dvs. nästa vecka).

För att passa i varje tidszon börjar e-postprogram som schemalagts med mottagarens tidszon att köras kl. 24 i **först/tidigaste** tidszon i världen (UTC +14:00).

## Engagement Programs {#engagement-programs}

När du [schemalägg ett engagemangsprogramflöde](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) och mottagarens tidszon är aktiv kommer programsändningen att börja köras vid midnatt i UTC +14:00. Vi kräver att du schemalägger den första omgången minst 25 timmar i framtiden (24 timmar + lite tid för att komma igång med kampanjen) eftersom folk kan kvalificera sig för omsändningen i varje tidszon över hela världen. Bearbetningen påbörjas nu i UTC +14:00 garanterar att vi skickar e-postmeddelandet på schemalagda datum och tid för alla som är kvalificerade för den här sändningen.

## Beräknar tidszon {#calculating-time-zone}

Marketo beräknar tidszonen baserat på en persons ort, delstat, land eller postnummer. Om vi inte kan beräkna någons tidszon utifrån dessa värden, återgår vi till fälten Inced, Incederad stat, Incederat land och Postnummer.

I de fall där vi har **endast** Land eller **endast** Tillstånd:

* För länder med tre eller färre tidszoner väljer vi den mellersta tidszonen.
* För lägen med två tidszoner väljer vi det tidigare av de två.

Om vi fortfarande inte kan fastställa någons tidszon utifrån någon kombination av dessa fält, kommer vi att **not** tilldela en tidszon och mejlet skickas baserat på din Marketo-prenumerationstidszon. Om ditt program är schemalagt till klockan 9:00 PDT, kommer personer utan tidszon att få e-postmeddelandet kl. 9:00 PDT.

>[!NOTE]
>
>Marketo beräknar automatiskt om en persons tidszon när något av ovanstående inmatningsfält ändras.

>[!MORELIKETHIS]
>
>* [Schemalägg e-postprogram med mottagartidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start for Email Programs](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Schemalägg engagemangsprogram med mottagartidszon](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

