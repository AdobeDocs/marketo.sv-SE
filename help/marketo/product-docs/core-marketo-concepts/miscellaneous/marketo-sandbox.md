---
unique-page-id: 11386358
description: Marketo Sandbox - Marketo Docs - produktdokumentation
title: Marketo Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Marketo Sandbox {#marketo-sandbox}

En Marketo Engage-sandlåda är ytterligare en instans som används för testning innan implementering i produktionsmiljön.

>[!AVAILABILITY]
>
>Alla har inte köpt den här funktionen. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

En Marketo-sandlåda kan inte synkroniseras med din vanliga CRM om den redan har synkroniserats med din produktionsinstans. Använd CRM-sandlådan för synkroniseringen och följ samma steg som den ursprungliga synkroniseringen.

## Saker att känna till om sandlådor {#things-to-know-about-sandboxes}

* Om du vill lägga till användare är processen densamma som att [lägga till användare i produktion](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Även här måste de använda en annan e-postadress om de redan har en Marketo-inloggning.
* Din Marketo-sandlåda börjar bli tom, men har samma funktioner som din produktionsinstans.
* Om du skapar ett program i sandlådan och vill flytta det till produktion kan du utföra en [programimport](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Sandlådor stryps så att produktionsinstanser inte påverkas negativt av testmiljöer. Du kan skicka upp till 20 e-postmeddelanden per kampanjkörning.

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta Adobe Account Team (din kontoansvarige) om du vill ha mer information.

## Instanskopia {#instance-copy}

Du kan skicka ett supportärende och begära en engångsinstanskopia för att fylla i din sandlåda. Instanskopian tar dock inte över _allt_. Mer information finns i [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Om du ändrar ditt ursprungliga CRM-system behövs en ny Marketo-instans och det går inte att skapa en instanskopia till den nya Marketo-instansen. Kontakta Marketo Support och utforska i stället funktionerna för att importera program.
