---
unique-page-id: 7513771
description: Inloggning och användarhantering - Marketo Docs - produktdokumentation
title: Inloggning och användarhantering
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Inloggning och användarhantering {#login-and-user-management}

## Skapa en [!UICONTROL Web Personalization]-användarroll {#create-a-web-personalization-user-role}

1. Gå till avsnittet **[!UICONTROL Admin]** och klicka sedan på **[!UICONTROL Users & Roles]**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicka på **[!UICONTROL Roles]**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Om användarrollen Web Personalization (WP) redan finns kontrollerar du att den är konfigurerad enligt steg 4.

1. Klicka på **[!UICONTROL New Role]**.

   ![](assets/three-1.png)

1. Ange en [!UICONTROL Role Name] och välj [!UICONTROL Permissions]. Klicka på **[!UICONTROL Create]** (den här rollen måste [gälla för alla arbetsytor](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Markera kryssrutorna _alla_ om du vill ge användare behörighet att komma åt allt i Target och Personalization.

## Användarbehörigheter för [!UICONTROL Web Personalization] och prediktivt innehåll {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Targeting and Personalization]**: Användaren har endast behörighet att visa, om den här behörigheten bara är markerad.

**[!UICONTROL Admin Web Personalization + Predictive]**: Användaren har bara åtkomst till kontoinställningarna och innehållsinställningarna för Personalization och appen Predictive Content. Användare kan visa sidor i programmet men har inte behörighet att skapa, redigera, ta bort eller starta.

**[!UICONTROL Predictive Content Editor]**: Användaren har redigeringsåtkomst till appen Predictive Content. Behörigheten gör att du kan skapa, redigera och ta bort innehållsdelar. Det går inte att aktivera innehåll för prediktiv användning på webben eller i e-post.

**[!UICONTROL Predictive Content Launcher]**: Användaren har åtkomst till alla funktioner för prediktivt innehåll, förutom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera och ta bort och aktivera innehållsdelar.

**[!UICONTROL Web Campaign Editor]**: Användaren har redigeringsåtkomst till alla Web Personalization-funktioner för att skapa, redigera och ta bort, men inte starta webbkampanjer.

**[!UICONTROL Web Campaign Launcher]**: Användaren har åtkomst till alla funktioner i Personalization-appen för webben, förutom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera, ta bort och starta webbkampanjer.

## Tilldela WP-roll till användare {#assign-wp-role-to-user}

1. Gå till **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Välj den användare som du vill ge WP-åtkomst till och klicka på **[!UICONTROL Edit User]**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Välj WP-användarroll för alla arbetsytor.

   ![](assets/seven.png)

1. Nyligen aktiverade användare ser panelen **[!UICONTROL Web Personalization]** i Min Marketo nästa gång de loggar in.

   ![](assets/eight.png)
