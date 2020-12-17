---
title: using-a-program-in-an-engagement-program-stream
description: Använda ett program i en Engagement Program Stream
translation-type: tm+mt
source-git-commit: 73df78512226c6c57625a73f14ba8b00bea195bd
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Använda ett program i en Engagement Program Stream

## Varför använda ett kapslat program i en interaktionsprogramström?

Det är enkelt att lägga till e-post i en ström i ett engagemangsprogram, och det fungerar bra. Men om era affärsbehov är mer komplexa kan det vara bra att placera e-postmeddelandet i ett program. Du kanske vill:

* Skicka ett e-postmeddelande till en undergrupp personer i strömmen
* Skicka _olika_-e-postmeddelanden till undergrupper i strömmen
* Inkludera landningssidor, formulär eller andra resurser i engagemangsprogrammet
* Aktivera multitouch-attribuering
* Lägg till extra flödessteg, som varningsmeddelanden

## Vad händer när du använder ett program i en ström?

När du använder ett kapslat program baseras beslutet att skicka ett e-postmeddelande till en person på programmedlemskapet och program-ID:t.

* Om du inte är medlem i programmet kommer du att få alla e-postmeddelanden som ingår i programmet en gång
* Om du är medlem i programmet får du inte e-postmeddelandet
* Om du inte längre är medlem men redan har fått e-postmeddelandet tidigare via det programmet får du inte e-postmeddelandet

När du använder ett program i en ström spelar det ingen roll om du har fått den specifika e-postadressen tidigare. Så länge e-postmeddelandet inte har skickats ut före _i det specifika programmet_ kan du ta emot det igen.

Det kan vara svårt att blanda e-post och program i ett engagemangsprogram. Du kanske vill använda den ena eller den andra.

>[!TIP]
>
>Se till att du använder filtret Medlem i Engagement Program i den smarta listan.

## Vad händer med dem som inte uppfyller villkoren i den smarta listan?

Om någon filtreras bort från den smarta listan i ett kapslat programs smarta kampanj går de inte vidare till nästa innehåll under den aktuella sändningen. De fortsätter till nästa del av innehållet i strömmen för _följande_-sändning.

## Vad innehåller ett kapslat program?

Ett väldesignat kapslat program innehåller e-post, rapporter och smarta kampanjer. Det är vettigt att hålla ihop dessa.

Den e-postadress du använder kan finnas i programmet, i ett annat program eller till och med i Design Studio. Var den finns beror på hur du vill använda den.

Rapportera ändringar med e-postplats. Om e-postmeddelandet till exempel finns i Design Studio visas alla mätvärden på en rad i e-postprestandarapporten - de olika skiftningarna kombineras. I resultatrapporten för Engagement Stream visas dock de olika meddelandena separat.

>[!CAUTION]
>
>Om du vill skicka om något är det säkraste att skapa ett nytt program och en smart kampanj.
