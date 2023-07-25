---
unique-page-id: 10096409
description: Undvik att skicka duplicerat innehåll - Marketo Docs - produktdokumentation
title: Undvik att skicka duplicerat innehåll
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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
| En kampanj i ett standardprogram som aktiveras från en sändning i **samma** CEE-programmet | En medlem i standardprogrammet | Nej |
| En kampanj i ett standardprogram som aktiveras från en sändning i **samma** CEE-programmet | Inte medlem i standardprogrammet | Ja |
| En kampanj i ett standardprogram som aktiveras från en sändning i en **olika** CEE-programmet | En medlem i standardprogrammet | Nej |
| En kampanj i ett standardprogram som aktiveras från en sändning i en **olika** CEE-programmet | Inte medlem i standardprogrammet | Ja |
| A **olika** CEE-program som använder en smart ström | En medlem i båda CEE-programmen | Nej |
