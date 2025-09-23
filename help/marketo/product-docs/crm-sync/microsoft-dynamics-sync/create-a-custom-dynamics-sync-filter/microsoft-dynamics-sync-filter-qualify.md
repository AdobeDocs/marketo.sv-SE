---
unique-page-id: 10092977
description: Microsoft Dynamics Sync Filter -Qualify - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync-filter -Kvalificera
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '108'
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
