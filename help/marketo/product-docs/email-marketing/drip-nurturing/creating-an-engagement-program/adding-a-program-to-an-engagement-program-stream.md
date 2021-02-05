---
unique-page-id: 10098134
description: Lägga till ett program i en Engagement Program Stream - Marketo Docs - Produktdokumentation
title: Lägga till ett program i en Engagement Program Stream
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Lägga till ett program i en Engagement Program Stream {#adding-a-program-to-an-engagement-program-stream}

## Varför använda ett kapslat program i en interaktionsprogramström? {#why-use-a-nested-program-in-an-engagement-program-stream}

Det är enkelt att lägga till e-post i en ström i ett engagemangsprogram, och det fungerar bra. Men om era affärsbehov är mer komplexa kan det vara bra att placera e-postmeddelandet i ett program. Du kanske vill:

* Skicka ett e-postmeddelande till en undergrupp personer i strömmen
* Skicka *olika*-e-postmeddelanden till undergrupper i strömmen
* Inkludera landningssidor, formulär eller andra resurser i näringen
* Aktivera multitouch-attribuering
* Lägg till extra flödessteg, till exempel varningsmeddelanden

## Vad händer när du använder ett program i en ström? {#what-happens-when-you-use-a-program-in-a-stream}

När du använder ett kapslat program baseras beslutet att skicka ett e-postmeddelande till en person på programmedlemskapet och program-ID:t.

* Om du inte är medlem i ett program får du alla e-postmeddelanden som ingår i programmet en gång
* Om du är medlem i programmet får du inte e-postmeddelandet
* Om du inte längre är medlem men har fått e-postmeddelandet tidigare via det programmet får du inte e-postmeddelandet

När du använder ett program i en ström spelar det ingen roll om du har fått den specifika e-postadressen tidigare. Så länge e-postmeddelandet inte har skickats ut före *i det specifika programmet* kan du ta emot det igen.

Det kan vara svårt att blanda e-post och program i ett engagemangsprogram. Du kanske vill använda den ena eller den andra.

>[!TIP]
>
>Använd ett **Member of Engagement Program**-filter i den smarta listan.

## Vad händer med dem som inte uppfyller villkoren i den smarta listan? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Om någon filtreras bort från den smarta listan i ett kapslat programs smarta kampanj går de inte vidare till nästa innehåll under den aktuella sändningen. De fortsätter till nästa del av innehållet i strömmen för *följande*-sändning.

## Vad innehåller ett kapslat program? {#what-does-a-nested-program-contain}

Ett väldesignat kapslat program innehåller e-post, rapporter och smarta kampanjer. Det är vettigt att hålla ihop dessa.

Den e-postadress du använder kan finnas i programmet, i ett annat program eller till och med i Design Studio. Var den finns beror på hur du vill använda den.

Rapportera ändringar med e-postplats. Om e-postmeddelandet till exempel finns i Design Studio visas alla mätvärden på en rad i e-postprestandarapporten - de olika skiftningarna kombineras. I resultatrapporten för Engagement Stream visas dock de olika meddelandena separat.

>[!CAUTION]
>
>Om du vill skicka om något är det säkraste att skapa ett nytt program och en smart kampanj.

>[!MORELIKETHIS]
>
>* [Lägg till innehåll i en ström](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Förstå program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

