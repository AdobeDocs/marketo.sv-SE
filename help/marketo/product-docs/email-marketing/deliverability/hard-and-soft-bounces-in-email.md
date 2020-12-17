---
unique-page-id: 1147328
description: Hårda och mjuka studsar i e-post - Marketo Docs - Produktdokumentation
title: Hårda och mjuka studsar i e-postmeddelanden
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Hårda och mjuka studsar i e-post {#hard-and-soft-bounces-in-email}

Ett hårt studsande kan göra en persons e-postadress ogiltig när en e-postserver meddelar Market att personens e-postadress inte kan levereras. Ett mjukt studs innebär att något gick fel när e-postmeddelandet skickades till personen. detta löses automatiskt och kan ibland ta dagar. Både hårda och mjuka studsar består av [flera kategorier](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Studsklassificering {#bounce-classification}

Det finns fem personsträngar i Marketo som är relaterade till problematisk e-postleverans.

1. **Uppskjuten**  e-post - Ange som True när en viss typ av hård studsning inträffar.
1. **Orsak**  till avbruten e-post - Det kan finnas många orsaker. Det här fältet försöker förklara orsaken.
1. **E-post avbruten vid **- När den kränkta studsen inträffar gör Marketo uppehåll i e-postutskick till personen i 24 timmar från den här tidsstämpeln.
1. **Ogiltig**  e-post - Ange som True när en viss typ av hård studsning inträffar.
1. **E-postfel orsak**  - Orsaken till den hårda studsen.

>[!NOTE]
>
>När en person når **e-postmeddelandet som är inaktiverat** finns det inget sätt att rensa kryssrutan för att pausa e-postmeddelandet. Personen kommer dock fortfarande att kunna mejlas 24 timmar efter det första uppehållet.
>
>När en person har markerats som **e-post ogiltig** kan de bara återställas manuellt (vilket vi rekommenderar att du bara gör om du vet att deras e-postadress är giltig) genom att avmarkera rutan E-post ogiltig på fliken Personinformation i posten.

>[!PREREQUISITES]
>
>Följ [de här stegen](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) för att skapa en e-postprestandarapport som genererar studsdata.

När du har skapat din e-postprestandarapport ska skärmen se ut ungefär så här: ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Skräppostfilter skapar ibland hårda studsar. Dessa &quot;falskt positiva&quot; är inte en indikation på giltigheten för personens e-postadress.

