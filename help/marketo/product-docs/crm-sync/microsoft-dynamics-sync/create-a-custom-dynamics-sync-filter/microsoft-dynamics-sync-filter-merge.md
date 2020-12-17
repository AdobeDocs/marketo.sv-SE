---
unique-page-id: 10092969
description: Microsoft Dynamics Sync-filter -Merge - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Sammanfoga
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Synkroniseringsfilter för Microsoft Dynamics: Sammanfoga {#microsoft-dynamics-sync-filter-merge}

Sammanslagningsleads i Microsoft Dynamics använder typen Två alternativ - Synkroniseringsfilter = Ja (SANT) och Synkroniseringsfilter = Nej (FALSKT). När du sammanfogar två poster varierar resultatet beroende på vilken post som är Sant och vilken som är Falskt.

Leadposterna blir sanna eller falska baserat på arbetsflödesreglerna som definierats av administratören för att avgöra vinnaren. Synkroniseringsfiltret för den vinnande posten är det som bestämmer om MS Dynamics-posten synkroniseras med Marketo.

Det är när en post är sann och en är falsk som det blir svårt.

| Om synkroniseringsfiltret för den förlorade posten är: | och synkroniseringsfiltret för den vinnande posten är: | Detta är resultatet i Marketo |
|---|---|---|
| True | True | Den vinnande posten fortsätter synkroniseringen med Marketo |
| Falskt | Falskt | Den vinnande posten fortsätter att **inte** synkronisera med Marketo |
| Falskt | True | Den vinnande posten synkroniseras med Marketo |
| True | Falskt | Den vinnande posten synkroniseras inte med Marketo |

