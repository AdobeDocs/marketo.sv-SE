---
unique-page-id: 10092969
description: Microsoft Dynamics Sync-filter -Merge - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Sammanfoga
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Synkroniseringsfilter för Microsoft Dynamics: Sammanfoga {#microsoft-dynamics-sync-filter-merge}

Sammanslagningsleads i Microsoft Dynamics använder typen Två alternativ - Synkroniseringsfilter = Ja (SANT) och Synkroniseringsfilter = Nej (FALSKT). När du sammanfogar två poster varierar resultatet beroende på vilken post som är Sant och vilken som är Falskt.

Leadposterna blir sanna eller falska baserat på arbetsflödesreglerna som definierats av administratören för att avgöra vinnaren. Synkroniseringsfiltret för den vinnande posten är det som avgör om MS Dynamics-posten synkroniseras med Marketo.

Det är när en post är sann och en är falsk som det blir svårt.

| Om synkroniseringsfiltret för den förlorade posten är: | och synkroniseringsfiltret för den vinnande posten är: | Detta är resultatet i Marketo |
|---|---|---|
| True | True | Den vinnande posten fortsätter synkroniseringen med Marketo |
| Falskt | Falskt | Den vinnande posten fortsätter att **inte** synkroniseras med Marketo |
| Falskt | True | Den vinnande posten synkroniseras med Marketo |
| True | Falskt | Den vinnande posten synkroniseras inte med Marketo |
