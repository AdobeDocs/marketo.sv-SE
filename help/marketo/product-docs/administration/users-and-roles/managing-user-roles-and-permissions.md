---
unique-page-id: 2359909
description: Hantera användarroller och behörigheter - Marketo Docs - Produktdokumentation
title: Hantera användarroller och behörigheter
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

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

Om du använder Marketo med Adobe Identity, listan över profilbeskrivningar [finns här](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Tilldela roller till en användare {#assign-roles-to-a-user}

Du kan tilldela roller till en användare när du [skapa användare för första gången](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) eller av [redigera en befintlig användare](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. I listan väljer du den användare du vill redigera och klickar på **[!UICONTROL Edit User]**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. Under **[!UICONTROL Roles]** väljer du de roller du vill tilldela användaren, baserat på de behörigheter användaren behöver, och klickar på **[!UICONTROL Save]**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Mer information om de olika rollerna finns i [Beskrivningar av rollbehörigheter](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## Skapa en ny roll {#create-a-new-role}

Ibland har din organisation mycket specifika medarbetare som kräver en anpassad kombination av behörigheter.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Klicka på **[!UICONTROL Roles]** -fliken.

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Klicka på **[!UICONTROL New Role]**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Ange **[!UICONTROL Role Name]**, a **[!UICONTROL Description]** (valfritt) och välj de behörigheter som användare med den här rollen behöver.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Redigera en roll {#edit-a-role}

Om du behöver ändra behörigheterna som är kopplade till en befintlig roll kan du redigera rollen.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Klicka på **[!UICONTROL Roles]** -fliken.

   ![](assets/managing-user-roles-and-permissions-12.png)

1. Välj den roll du vill ändra i listan och klicka på **[!UICONTROL Edit Role]**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Ändra **[!UICONTROL Role Name]** och **[!UICONTROL Description]** vid behov, och sedan ändra urvalet av associerade **[!UICONTROL Permissions]**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Användare som har den roll du har redigerat får de ändrade behörigheterna när de har loggat ut och loggat in igen.

## Ta bort en roll {#delete-a-role}

Om en roll blir onödig kan du ta bort den.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Klicka på **[!UICONTROL Users & Roles]**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Klicka på **[!UICONTROL Roles]** -fliken.

   ![](assets/managing-user-roles-and-permissions-17.png)

1. I listan väljer du den roll du vill ta bort och klickar på **[!UICONTROL Delete Role]**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Klicka **[!UICONTROL Delete]** för att bekräfta.

   ![](assets/managing-user-roles-and-permissions-19.png)
