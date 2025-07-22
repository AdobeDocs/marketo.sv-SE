---
unique-page-id: 12983291
description: Förstå mottagarens tidszon - Marketo Docs - Produktdokumentation
title: Förstå mottagartidszon
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Förstå mottagartidszon {#understanding-recipient-time-zone}

E-post- och engagemangsprogram kan konfigureras så att de levereras enligt mottagarnas tidszoner, vilket eliminerar behovet av att skapa flera program - skicka en gång och Marketo lagrar automatiskt e-postmeddelandet till rätt lokal tid.

>[!NOTE]
>
>[!UICONTROL Recipient Time Zone] fungerar för närvarande **endast** med e-postinnehåll. Det fungerar inte med standardprogram för engagemang.

## E-postprogram {#email-programs}

Det finns två primära scenarier när [schemalägger ett e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Schemalägger programmet att köras inom de närmaste 25 timmarna.
1. Schemalägger programmet att köras mer än 25 timmar i framtiden (dvs. nästa vecka).

För att varje tidszon ska få plats, börjar e-postprogram som schemalagts med [!UICONTROL Recipient Time Zone] att köras vid midnatt i den **första/tidigaste** tidszonen i världen (UTC +14:00).

## Engagement Programs {#engagement-programs}

När du [schemalägger en engagemangsprogramström](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) och [!UICONTROL Recipient Time Zone] är aktiv börjar programsändningen köras vid midnatt i UTC +14:00. Vi kräver att du schemalägger den första omgången minst 25 timmar i framtiden (24 timmar + lite tid för att komma igång med kampanjen) eftersom folk kan kvalificera sig för omsändningen i varje tidszon över hela världen. Bearbetningen påbörjas nu i UTC +14:00 garanterar att vi skickar e-postmeddelandet på det schemalagda datumet och den schemalagda tidpunkten för varje person som är berättigad för den här sändningen.

## Beräknar tidszon {#calculating-time-zone}

Marketo beräknar tidszonen baserat på en persons ort, delstat, land eller postnummer. Om vi inte kan beräkna någons tidszon utifrån dessa värden, återgår vi till fälten Inced, Incederad stat, Incederat land och Postnummer.

I de fall där vi har **endast** land eller **endast** delstat tillgänglig:

* För länder med tre eller färre tidszoner väljer vi den mellersta tidszonen.
* För lägen med två tidszoner väljer vi det tidigare av de två.

Om vi fortfarande inte kan fastställa någons tidszon från någon kombination av dessa fält, tilldelar vi **inte** en tidszon och e-postmeddelandet skickas baserat på din Marketo-prenumerationstidszon. Om ditt program är schemalagt för 9:00am PDT, skickas e-postmeddelandet till personer som saknar tidszon vid 9:00am PDT.

>[!NOTE]
>
>Marketo beräknar automatiskt om en persons tidszon när något av ovanstående inmatningsfält ändras.

>[!MORELIKETHIS]
>
>* [Schemalägg e-postprogram med [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Startsida för e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Schemalägg engagemangsprogram med [!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
