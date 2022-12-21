---
unique-page-id: 1147328
description: Hårda och mjuka studsar i e-postmeddelanden - Marketo Docs - produktdokumentation
title: Hårda och mjuka studsar i e-postmeddelanden
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Hårda och mjuka studsar i e-postmeddelanden {#hard-and-soft-bounces-in-email}

Ett hårt studsande kan göra en persons e-postadress ogiltig när en e-postserver meddelar Marketo att personens e-postadress inte kan levereras. Ett mjukt studs innebär att något gick fel när e-postmeddelandet skickades till personen. detta löses automatiskt och kan ibland ta dagar. Både hårda och mjuka studsar består av [flera kategorier](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Studsklassificering {#bounce-classification}

Det finns fem personsträngar i Marketo som är relaterade till problematisk e-postleverans.

1. **E-post pausad** - Ange som Sant när en viss typ av hård studsning inträffar.
1. **Orsak till uppehåll i e-post** - Det kan finnas många orsaker. Det här fältet försöker förklara orsaken.
1. **E-post pausad** - När den felaktiga studsen inträffar gör Marketo uppehåll i utskicket till personen i 24 timmar från den här tidsstämpeln.
1. **Ogiltig e-postadress** - Ange som Sant när en viss typ av hård studsning inträffar.
1. **Ogiltig e-postorsak** - Orsaken till den hårda studsen.

>[!NOTE]
>
>När en person når **e-postmeddelandet har pausats** status, det finns inget sätt att avmarkera kryssrutan för att göra uppehåll i e-postmeddelanden. Personen kommer dock fortfarande att kunna mejlas 24 timmar efter det första uppehållet.
>
>När en person markeras som **e-post ogiltig** kan de bara återställas manuellt (vilket vi rekommenderar att du bara gör om du vet att deras e-postadress är giltig) genom att avmarkera rutan E-post är ogiltig på fliken Personinformation i posten.

>[!PREREQUISITES]
>
>Följ [dessa steg](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) för att skapa en e-postprestandarapport som genererar studsdata.

När du har skapat din e-postprestandarapport ska skärmen se ut ungefär så här:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Skräppostfilter skapar ibland hårda studsar. Dessa &quot;falskt positiva&quot; är inte en indikation på giltigheten för personens e-postadress.
