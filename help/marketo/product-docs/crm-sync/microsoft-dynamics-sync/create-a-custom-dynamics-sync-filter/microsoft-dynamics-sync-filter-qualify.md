---
unique-page-id: 10092977
description: Microsoft Dynamics Sync-filter -Kvalificera - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Kvalificera
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 0%

---

# Microsoft Dynamics Sync-filter: Kvalificera {#microsoft-dynamics-sync-filter-qualify}

När du vill konvertera ett lead till en kontakt i Microsoft Dynamics ska du använda den här standardprocessen för kvalificering. Synka sedan till Marketo Engage.

## Konverteringsprocessen {#the-conversion-process}

Så här fungerar filtren under konverteringen.

| Om blysynkroniseringsfiltret är: | och kontaktsynkroniseringsfiltret är: | Detta är resultatet i Marketo |
|---|---|---|
| Falskt | Falskt | Ingenting synkroniseras i Marketo |
| True | True | Kontakten synkroniseras i Marketo |
| Falskt | True | Ny kontaktpost skapas i Marketo |
| True | Falskt | MS Dynamics uppdaterar lead-information i Marketo, men kontaktposten synkroniseras inte |

>[!CAUTION]
>
>Vi stöder endast den körklara konverteringsprocessen Kvalificera.
