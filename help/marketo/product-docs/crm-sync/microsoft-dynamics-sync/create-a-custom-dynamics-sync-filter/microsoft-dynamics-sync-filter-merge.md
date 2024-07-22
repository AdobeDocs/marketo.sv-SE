---
unique-page-id: 10092969
description: Microsoft Dynamics Sync-filter -Merge - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter - Sammanfoga
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Microsoft Dynamics Sync-filter: Sammanfoga {#microsoft-dynamics-sync-filter-merge}

Sammanslagningsleads i Microsoft Dynamics använder typen Två alternativ - Synkroniseringsfilter = Ja (SANT) och Synkroniseringsfilter = Nej (FALSKT). När du sammanfogar två poster varierar resultatet beroende på vilken post som är Sant och vilken som är Falskt.

Leadposterna blir sanna eller falska baserat på arbetsflödesreglerna som definierats av administratören för att avgöra vinnaren. Synkroniseringsfiltret för den vinnande posten är det som avgör om MS Dynamics-posten synkroniseras med Marketo.

Det är när en post är sann och en är falsk som det blir svårt.

| Om synkroniseringsfiltret för den förlorade posten är: | och synkroniseringsfiltret för den vinnande posten är: | Detta är resultatet i Marketo |
|---|---|---|
| True | True | Den vinnande posten fortsätter att synkroniseras med Marketo |
| Falskt | Falskt | Den vinnande posten fortsätter att _inte_ synkroniseras med Marketo |
| Falskt | True | Den vinnande posten synkroniseras med Marketo |
| True | Falskt | Den vinnande posten synkroniseras inte med Marketo |
