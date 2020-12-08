---
unique-page-id: 10092977
description: Microsoft Dynamics Sync-filter -Kvalificera - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Kvalificera
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Synkroniseringsfilter för Microsoft Dynamics: Kvalificera {#microsoft-dynamics-sync-filter-qualify}

När du vill konvertera ett lead till en kontakt i Microsoft Dynamics ska du använda den här standardprocessen för kvalificering. Synkronisera den sedan med Marketo.

## Konverteringsprocessen {#the-conversion-process}

Så här fungerar filtren under konverteringen.

| Om blysynkroniseringsfiltret är: | och kontaktsynkroniseringsfiltret är: | Detta är resultatet i Marketo |
|---|---|---|
| Falskt | Falskt | Ingenting synkroniseras i Marketo |
| True | True | Kontakten synkroniseras i Marketo |
| Falskt | True | Ny kontaktpost skapas i Marketo |
| True | Falskt | MS Dynamics uppdaterar lead-information i Marketo men kontaktposten synkroniseras inte |

>[!CAUTION]
>
>Vi stöder endast den körklara konverteringsprocessen Kvalificera.

