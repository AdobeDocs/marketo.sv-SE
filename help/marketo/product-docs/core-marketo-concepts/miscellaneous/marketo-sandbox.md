---
unique-page-id: 11386358
description: Marketo Sandbox - Marketo Docs - Produktdokumentation
title: Marketo Sandbox
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Marketo Sandbox {#marketo-sandbox}

En Marketo-sandlåda är ytterligare en instans som används för testning innan implementering i produktionsmiljön.

>[!AVAILABILITY]
>
>
>Alla kunder har inte köpt den här funktionen. Kontakta din Customer Success Manager för mer information.

En Marketo-sandlåda kan inte synkroniseras med din vanliga CRM om den redan har synkroniserats med din produktionsinstans. Använd CRM-sandlådan för synkroniseringen och följ samma steg som den ursprungliga synkroniseringen.

## Saker att känna till om sandlådor {#things-to-know-about-sandboxes}

* När din Customer Success Manager har konfigurerat din sandlåda och skickar inbjudan måste du använda en annan e-postadress för att logga in än din Marketo-produktionsinstans.
* Om du vill lägga till användare är processen densamma som att [lägga till användare i produktion](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Även här måste de använda en annan e-postadress om de redan har en Marketo-inloggning.
* Din Marketo-sandlåda börjar bli tom, men har samma funktioner som din produktionsinstans.
* Du kan skicka ett supportärende och begära en engångsinstanskopia för att fylla i din sandlåda. Instanskopian tar dock inte över _allt_. Mer information finns i Marketo Support.
* Om du skapar ett program i sandlådan och vill flytta det till produktion kan du utföra en [programimport](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Sandlådor stryps så att produktionsinstanser inte påverkas negativt av testmiljöer. Du kan skicka upp till 30 e-postmeddelanden per kampanjkörning.

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.
