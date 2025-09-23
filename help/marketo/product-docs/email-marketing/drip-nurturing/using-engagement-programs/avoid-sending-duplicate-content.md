---
unique-page-id: 10096409
description: Undvik att skicka duplicerat innehåll - Marketo Docs - produktdokumentation
title: Undvik att skicka duplicerat innehåll
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Undvik att skicka duplicerat innehåll {#avoid-sending-duplicate-content}

Har du någonsin fått samma mejl två gånger? Irriterande, eller hur?

Här är sju möjliga scenarier och resultat som du bör vara medveten om för att förhindra att någon skickar samma budskap två gånger med engagemangsprogram.

## Scenarier {#scenarios}

| E-postmeddelandet skickas från | Personen är | Personen får e-post |
|---|---|---|
| En kampanj i ett separat, fristående standardprogram | Inte medlem i standardprogrammet | Ja |
| En kampanj i ett separat, fristående standardprogram | En medlem i standardprogrammet | Nej |
| En kampanj i ett standardprogram som utlöses från en sändning inom CEE-programmet **same** | En medlem i standardprogrammet | Nej |
| En kampanj i ett standardprogram som utlöses från en sändning inom CEE-programmet **same** | Inte medlem i standardprogrammet | Ja |
| En kampanj i ett standardprogram som aktiveras från en sändning inom ett **annat** CEE-program | En medlem i standardprogrammet | Nej |
| En kampanj i ett standardprogram som aktiveras från en sändning inom ett **annat** CEE-program | Inte medlem i standardprogrammet | Ja |
| Ett **annat** CEE-program som använder en smart ström | En medlem i båda CEE-programmen | Nej |
