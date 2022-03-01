---
unique-page-id: 2359909
description: Hantera användarroller och behörigheter - Marketo Docs - Produktdokumentation
title: Hantera användarroller och behörigheter
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Hantera användarroller och behörigheter {#managing-user-roles-and-permissions}

Ange, skapa och redigera användarroller och tilldela dem till användare. På så sätt kan du styra vilka områden och funktioner som varje Marketo-användare har tillgång till.

En marknadsföringsanvändare behöver till exempel vanligtvis bred åtkomst i hela programmet för att kunna skapa, ändra och distribuera e-post, landningssidor och program. En webbdesigner däremot spenderar nästan hela sin tid på Design Studio och skapar material för e-post och landningssidor. Och även om företagsledare i stor utsträckning använder Marketo rapporter i Analytics-området kanske de inte behöver skapa eller driva tillgångarna eller programmen själva.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Marketo har flera inbyggda roller med olika åtkomstnivåer:

* **Administratör** - alla delar av programmet, inklusive administrationsavsnittet
* **Standardanvändare** - alla delar av programmet, utom administrationsavsnittet
* **Marknadsförare** - alla delar av programmet, utom administrationsavsnittet
* **Webbdesigner** - endast Design Studio
* **Analysanvändare** - endast Analytics-avsnittet

Du kan inte redigera rollerna Admin och Standard User, men du kan redigera de andra. Du kan också skapa nya anpassade roller som matchar de särskilda organisationsstrukturerna i ditt företag.

## Marketo med Adobe Identity {#marketo-with-adobe-identity}

Om du använder Marketo med Adobe Identity, listan över profilbeskrivningar [finns här](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## Tilldela roller till en användare {#assign-roles-to-a-user}

Du kan tilldela roller till en användare när du [skapa användare för första gången](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) eller av [redigera en befintlig användare](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Om du vill redigera en befintlig användare går du till **Administratör** och klicka **Användare och roller**.

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. I listan väljer du den användare du vill redigera och klickar på **Redigera användare**.

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. Under **Roller** väljer du de roller du vill tilldela användaren, baserat på de behörigheter användaren behöver, och klickar på **Spara**.

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >Mer information om de olika rollerna finns i  [Beskrivningar av rollbehörigheter](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Skapa en ny roll {#create-a-new-role}

Ibland har din organisation mycket specifika medarbetare som kräver en anpassad kombination av behörigheter.

1. Om du vill skapa en ny användarroll går du till Admin och klickar på **Användare och roller**.

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. Klicka på **Roller** -fliken.

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. Klicka **Ny roll**.

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. Ange **Rollnamn**, a **Beskrivning** (valfritt) och välj de behörigheter som användare med den här rollen behöver.

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## Redigera en roll {#edit-a-role}

Om du behöver ändra behörigheterna som är kopplade till en befintlig roll kan du redigera rollen.

1. Gå till **Administratör** och klicka **Användare och roller**.

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. Klicka på **Roller** -fliken.

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. Välj den roll du vill ändra i listan och klicka på **Redigera roll**.

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. Ändra **Rollnamn** och **Beskrivning** vid behov, och sedan ändra urvalet av associerade **Behörigheter**.

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >Användare som har den roll du har redigerat får de ändrade behörigheterna när de har loggat ut och loggat in igen.

## Ta bort en roll {#delete-a-role}

Om en roll blir onödig kan du ta bort den.

1. Gå till Admin och klicka på **Användare och roller**.

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. Klicka på **Roller** -fliken.

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. I listan väljer du den roll du vill ta bort och klickar på **Ta bort roll**.

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. Klicka **Ta bort** för att bekräfta.

   ![](assets/image2014-9-9-18-3a10-3a50.png)
