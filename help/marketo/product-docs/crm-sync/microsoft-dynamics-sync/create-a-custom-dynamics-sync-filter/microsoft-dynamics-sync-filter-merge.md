---
unique-page-id: 10092969
description: Microsoft Dynamics Sync Filter -Merge - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Merge
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# [!DNL Microsoft] Dynamics-synkroniseringsfilter: Sammanfoga {#microsoft-dynamics-sync-filter-merge}

Sammanslagning av leads i [!DNL Microsoft Dynamics] använder typen Två alternativ - Synkroniseringsfilter = Ja (SANT) och Synkroniseringsfilter = Nej (FALSKT). När du sammanfogar två poster varierar resultatet beroende på vilken post som är Sant och vilken som är Falskt.

Leadposterna blir sanna eller falska baserat på arbetsflödesreglerna som definierats av administratören för att avgöra vinnaren. Synkroniseringsfiltret för den vinnande posten är det som avgör om posten [!DNL MS Dynamics] synkroniseras med Marketo.

Det är när en post är sann och en är falsk som det blir svårt.

| Om synkroniseringsfiltret för den förlorade posten är: | och synkroniseringsfiltret för den vinnande posten är: | Detta är resultatet i Marketo |
|---|---|---|
| [!UICONTROL True] | [!UICONTROL True] | Den vinnande posten fortsätter att synkroniseras med Marketo |
| [!UICONTROL False] | [!UICONTROL False] | Den vinnande posten fortsätter att **inte** synkroniseras med Marketo |
| [!UICONTROL False] | [!UICONTROL True] | Den vinnande posten synkroniseras med Marketo |
| [!UICONTROL True] | [!UICONTROL False] | Den vinnande posten synkroniseras inte med Marketo |
