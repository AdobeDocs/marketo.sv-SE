---
description: fliken Namn - Marketo Docs - produktdokumentation
title: Fliken Namn
hide: true
hidefromtoc: true
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: 983f47ded61198b015f92a770be1004a13547296
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Fliken Namn {#name-tab}

Resor representeras genom en serie utlösar-, filter- och flödeskort. Om du klickar på vart och ett av korten öppnas motsvarande utfällningspanel.

Utlösaröversikt: Kortet visar antalet utlösare i den specifika kampanjen. Om du klickar på det här kortet utökas även utlösaren så att utlösardetaljkort visas och utfällningspanelen öppnas samtidigt med följande information:

Kampanj som utlösaren tillhör

Knappen Redigera utlösare för att få åtkomst till fliken med smarta listor

Lista med utlösarnamn

SCREENSHOT

Utlösardetalj: Kortet visar utlösarnamn. Om du klickar på det här kortet öppnas en utfällbar panel med följande information:

Kampanj som utlösaren tillhör

Knappen Redigera utlösare för att få åtkomst till fliken med smarta listor

Lista över begränsningar som är kopplade till utlösaren

SCREENSHOT

Filter: Om du klickar på det här kortet öppnas en utfällbar panel med följande information:

Kampanj som utlösaren tillhör

Knappen Redigera filter för att komma åt fliken med smarta listor

Uppskattat antal personer som är kvalificerade för filtret

Lista över filter och deras respektive begränsningar

SCREENSHOT

Flödessteg: Om ett flödessteg inte innehåller några alternativ visar kortet attribut som är kopplade till flödessteget. Om du klickar på kortet öppnas en utfällbar panel med följande information:

Campaign som flödessteget tillhör

Knappen Redigera flöde för att komma åt fliken Flöde

Lista med attribut som är kopplade till flödessteget

SCREENSHOT

Flödessteg: Om ett flödessteg innehåller alternativ visas flödesstegets namn på kortet. Om du klickar på kortet öppnas en utfällbar panel med följande information:

Campaign som flödessteget tillhör

Knappen Redigera flöde för att komma åt fliken Flöde

Lista med urvalsvillkor som är kopplade till flödessteget

SCREENSHOT

Flödessteg för körnings- och begärandekampanjer:

Om Flödessteget Kör eller Begär kampanj inte innehåller några alternativ visas kampanjens namn på kortet. Om du klickar på kortet öppnas en utfällbar panel med följande information:

Kampanj som flödessteget tillhör

Knappen Redigera flöde för att komma åt fliken Flöde

Lista med attribut som är kopplade till flödessteget

Visa listknapp som öppnar en lista med kampanjer som använder den specifika förfrågan eller som kör kampanj

Obs! Du kan redigera flödessteget från en primär kampanj. Om du vill redigera kapslade kampanjer måste du navigera till kampanjen via hyperlänken i panelen för utfällbara kampanjer.

SCREENSHOT

SCREENSHOT

Om Flödessteget Kör eller Begär kampanj innehåller alternativ visas kampanjens namn på kortet. Om du klickar på kortet öppnas en utfällbar panel med följande information:

Kampanj som flödessteget tillhör

Knappen Redigera flöde för att komma åt fliken Flöde

Lista med urvalsvillkor som är kopplade till flödessteget

SCREENSHOT

SCREENSHOT

Om en kampanj som körs eller begär att få välja visas alla alternativ på enskilda kort när du klickar på flödeskortet.

Om du klickar på ett urvalskort utökas kampanjen som är kopplad till det specifika valet och en bildrutepanel öppnas samtidigt med följande information:

Campaign som valet tillhör

Redigera alternativknapp för att komma åt fliken Flöde

Lista med urvalsvillkor som är kopplade till flödessteget

Visa listknapp som öppnar en lista med kampanjer som använder den specifika förfrågan eller som kör kampanj

SCREENSHOT

Kampanj för att visa kapslad körning (nytt avsnitt)

Kör kampanjer som körs i serie med den överordnade kampanjen, dvs. leads som kvalificerar för en körbar kampanj som slutför alla flödessteg från kampanjen och återgår till den primära kampanjen för att fortsätta genom de flödessteg som gäller för den här kampanjen.

Här är ett exempel på den smarta kampanjen&quot;Campaign A&quot; som innehåller ett körningsflöde för kampanjer. Ni kan tänka er&quot;Campaign A&quot; som er primära kampanj.

SCREENSHOT

Om du klickar på det körda kampanjflödeskortet expanderas det så att information om&quot;Campaign B&quot; visas

Campaign B omfattar filter som ger upphov till okvalificerad och kvalificerad publik.

Kvalificerad målgrupp går igenom de flödessteg som är kopplade till&quot;Campaign B&quot;

Alla mottagare (kvalificerade och inte kvalificerade) går tillbaka till&quot;Campaign A&quot; och går vidare till nästa flödessteg

SCREENSHOT

Du kan klicka på Flödessteget Kör kampanj i&quot;Campaign B&quot;, som kommer att expandera för att visa alternativkort och kampanjer som är kopplade till varje val.

SCREENSHOT

Visualiserar kampanj för begärande (nytt avsnitt)

Begärandekampanjer körs parallellt med den överordnade kampanjen, dvs. leads som kvalificerar för en begärandekampanj slutför alla flödessteg från kampanjen och avslutar kampanjen. Samtidigt kommer samma uppsättning leads också att gå igenom flödessteg från den primära kampanjen

Här är ett exempel på den smarta kampanjen&quot;Campaign A&quot;, som innehåller ett flödessteg för begärandekampanjer. Ni kan tänka er&quot;Campaign A&quot; som er primära kampanj.

SCREENSHOT

Om du klickar på flödeskortet för begärandekampanjen expanderas det så att information om&quot;Campaign B&quot; visas

Campaign B innehåller filter som ger ut till en kvalificerad målgrupp.

Kvalificerad målgrupp går igenom de flödessteg som är kopplade till&quot;Campaign B&quot;

Samtidigt går alla målgrupper vidare till nästa flödessteg i&quot;Campaign A&quot;

SCREENSHOT

Du kan fördjupa dig i kapslade kampanjer om något av flödesstegen innehåller ytterligare en kampanj genom att klicka på flödeskortet för att visa information om kampanjen

SCREENSHOT

Här är ett exempel på en begärandekampanj med valmöjligheter.

SCREENSHOT

Felhantering:

Fel i smarta listor och flödessteg markeras via en felikon på kortet. Motsvarande felmeddelande visas dessutom i panelen för utskjutning.

Här är ett exempel på fel i utlösaren som visas i utlösaröversiktskortet, panelen för utskjutning samt utlösarkortet för detaljer

SCREENSHOT

SCREENSHOT

Fel på filterkortet kan innehålla

Fel i den smarta listan som gör att kvalificerade målgrupper inte visas

Fel i filterlogik

Fel i begränsningar eller avsaknad av sådana i ett eller flera filter

SCREENSHOT

Om du inte anger värden (attribut) flaggas de inte som fel, utan fortsätter att fungera som på fliken Flöde. Befintliga kampanjer kommer därför inte att störas. Om flödessteg inte innehåller några attribut visas de som varningar.

SCREENSHOT

Obs! Fel i en kapslad kampanj visas inte förrän du har klickat för att expandera den kapslade kampanjen
