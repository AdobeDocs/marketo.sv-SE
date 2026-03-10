---
unique-page-id: 10092977
description: Läs mer om Dynamics-synkroniseringsfiltret Kvalificera process när du konverterar ett lead till en kontakt. Förstå hur filtervärden för lead- och kontaktsynkronisering påverkar Marketo-synkroniseringen.
title: Microsoft Dynamics Sync-filter -Kvalificera
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics] Synkroniseringsfilter: Kvalificera {#microsoft-dynamics-sync-filter-qualify}

När du vill konvertera ett lead till en kontakt i [!DNL Microsoft Dynamics] måste du använda den här standardprocessen för kvalificering. Synka sedan till Marketo.

## Konverteringsprocessen {#the-conversion-process}

Så här fungerar filtren under konverteringen.

| Om blysynkroniseringsfiltret är: | och kontaktsynkroniseringsfiltret är: | Detta är resultatet i Marketo |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Ingenting synkroniseras i Marketo |
| [!UICONTROL True] | [!UICONTROL True] | Kontakten synkroniseras i Marketo |
| [!UICONTROL False] | [!UICONTROL True] | Ny kontaktpost skapas i Marketo |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] uppdaterar lead-information i Marketo, men kontaktposten synkroniseras inte |

>[!CAUTION]
>
>Vi stöder endast den körklara konverteringsprocessen Kvalificera.
