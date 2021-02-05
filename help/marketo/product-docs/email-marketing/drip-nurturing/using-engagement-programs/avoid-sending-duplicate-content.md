---
unique-page-id: 10096409
description: Undvik att skicka duplicerat innehåll - Marketo Docs - produktdokumentation
title: Undvik att skicka duplicerat innehåll
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Undvik att skicka duplicerat innehåll {#avoid-sending-duplicate-content}

Har du någonsin fått samma mejl två gånger? Irriterande, eller hur?

Här är sju möjliga scenarier och resultat som du bör vara medveten om för att förhindra att någon skickar samma budskap två gånger med engagemangsprogram.

## Scenarier {#scenarios}

En person får ett e-postmeddelande som skickas från Customer Engagement Engine.

| E-postmeddelandet skickas från | Personen är | Personen får e-post |
|---|---|---|
| En kampanj i ett separat, fristående standardprogram | Inte medlem i standardprogrammet | Ja |
| En kampanj i ett separat, fristående standardprogram | En medlem i standardprogrammet | Nej |
| En kampanj inom ett standardprogram som aktiveras från en sändning inom **samma** CEE-program | En medlem i standardprogrammet | Nej |
| En kampanj inom ett standardprogram som aktiveras från en sändning inom **samma** CEE-program | Inte medlem i standardprogrammet | Ja |
| En kampanj inom ett standardprogram som aktiveras från en sändning inom ett **annat** CEE-program | En medlem i standardprogrammet | Nej |
| En kampanj inom ett standardprogram som aktiveras från en sändning inom ett **annat** CEE-program | Inte medlem i standardprogrammet | Ja |
| Ett **annat** CEE-program som använder en smart ström | En medlem i båda CEE-programmen | Nej |
