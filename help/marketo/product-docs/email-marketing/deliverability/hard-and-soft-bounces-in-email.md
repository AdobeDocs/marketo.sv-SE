---
unique-page-id: 1147328
description: Hårda och mjuka studsar i e-post - Marketo Docs - Produktdokumentation
title: Hårda och mjuka studsar i e-postmeddelanden
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# Hårda och mjuka studsar i e-postmeddelanden {#hard-and-soft-bounces-in-email}

Ett hårt studsande kan göra en persons e-postadress ogiltig när en e-postserver meddelar Market att personens e-postadress inte kan levereras. Ett mjukt studs innebär att något gick fel när e-postmeddelandet skickades till personen. detta löses automatiskt och kan ibland ta dagar. Både hårda och mjuka studsar består av [flera kategorier](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Studsklassificering {#bounce-classification}

Det finns fem personsträngar i Marketo som är relaterade till problematisk e-postleverans.

1. **Uppskjuten** e-post - Ange som True när en viss typ av hård studsning inträffar.
1. **Orsak** till uppehåll i e-post - Det kan finnas många orsaker. Det här fältet försöker förklara orsaken.
1. **E-post avbruten vid **- När den kränkta studsen inträffar gör Marketo uppehåll i e-postutskick till personen i 24 timmar från den här tidsstämpeln.
1. **Ogiltig** e-post - Ange som true när en viss typ av hård studsning inträffar.
1. **Ogiltig orsak** till e-post - Orsaken till den hårda studsen.

>[!NOTE]
>
>När en person når **status för pausad** e-post finns det inget sätt att avmarkera kryssrutan för pausad e-post. Personen kommer dock fortfarande att kunna mejlas 24 timmar efter det första uppehållet.
>
>När en person har markerats som ogiltig **för** e-post kan de bara återställas manuellt (vilket vi rekommenderar att du bara gör om du vet att deras e-postadress är giltig) genom att avmarkera rutan E-post ogiltig på fliken Personinformation i posten.

>[!PREREQUISITES]
>
>Följ [de här stegen](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) för att skapa en e-postprestandarapport som genererar studsdata.

När du har skapat din e-postprestandarapport ska skärmen se ut ungefär så här: ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Skräppostfilter skapar ibland hårda studsar. Dessa &quot;falskt positiva&quot; är inte en indikation på giltigheten för personens e-postadress.

