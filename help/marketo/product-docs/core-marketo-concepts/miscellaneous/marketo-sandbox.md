---
unique-page-id: 11386358
description: Marketo Sandbox - Marketo Docs - produktdokumentation
title: Marketo Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Marketo Sandbox {#marketo-sandbox}

En Marketo-sandlåda är ytterligare en instans som används för testning innan implementering i produktionsmiljön.

>[!AVAILABILITY]
>
>Alla har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

En Marketo-sandlåda kan inte synkroniseras med din vanliga CRM om den redan har synkroniserats med din produktionsinstans. Använd CRM-sandlådan för synkroniseringen och följ samma steg som den ursprungliga synkroniseringen.

## Saker att känna till om sandlådor {#things-to-know-about-sandboxes}

* När Adobe Account Team har konfigurerat din sandlåda och skickar inbjudan måste du använda en annan e-postadress för att logga in än din Marketo-produktionsinstans.
* Om du vill lägga till användare är processen densamma som [lägga till användare i produktion](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Även här måste de använda en annan e-postadress om de redan har en Marketo-inloggning.
* Din Marketo-sandlåda börjar bli tom, men har samma funktioner som din produktionsinstans.
* Om du skapar ett program i sandlådan och vill flytta det till produktion kan du utföra en [programimport](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Sandlådor stryps så att produktionsinstanser inte påverkas negativt av testmiljöer. Du kan skicka upp till 20 e-postmeddelanden per kampanjkörning.

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta kontogruppen på Adobe (din kontoansvarige) för mer information.

## Instanskopia {#instance-copy}

Du kan skicka ett supportärende och begära en engångsinstanskopia för att fylla i din sandlåda. Instanskopian kommer inte att ta över _allt_, dock. Läs [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) för mer information.

>[!NOTE]
>
>Om du ändrar ditt ursprungliga CRM-system behövs en ny Marketo-instans och det går inte att skapa en instanskopia till den nya Marketo-instansen. Kontakta Marketo Support och utforska i stället funktionerna i Importera program.
