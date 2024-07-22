---
unique-page-id: 7513771
description: Inloggning och användarhantering - Marketo Docs - produktdokumentation
title: Inloggning och användarhantering
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Inloggning och användarhantering {#login-and-user-management}

## Skapa en Personalization-användarroll för webben {#create-a-web-personalization-user-role}

1. Gå till avsnittet **Admin** och klicka sedan på **Användare och roller**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicka på **Roller**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Om användarrollen Web Personalization (WP) redan finns kontrollerar du att den är konfigurerad enligt steg 4.

1. Klicka på **Ny roll**.

   ![](assets/three-1.png)

1. Ange ett rollnamn och välj Behörigheter. Klicka på **Skapa** (den här rollen måste [gälla för alla arbetsytor](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Markera kryssrutorna _alla_ om du vill ge användare behörighet att komma åt allt i Target och Personalization.

## Användarbehörigheter för Personalization och prediktivt innehåll {#web-personalization-and-predictive-content-user-permissions}

**Målgrupp och Personalization**: Användaren har endast behörighet att visa, om den här behörigheten bara är markerad.

**Admin Web Personalization + Predictive**: Användaren har bara tillgång till kontoinställningarna och innehållsinställningarna för Web Personalization och prediktiv innehållsapp. Användare kan visa sidor i programmet men har inte behörighet att skapa, redigera, ta bort eller starta.

**Predictive Content Editor**: Användaren har redigeringsåtkomst till programmet Predictive Content. Behörigheten gör att du kan skapa, redigera och ta bort innehållsdelar. Det går inte att aktivera innehåll för prediktiv användning på webben eller i e-post.

**Startprogram för prediktivt innehåll**: Användaren har tillgång till alla funktioner för prediktivt innehåll, utom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera och ta bort och aktivera innehållsdelar.

**Webbkampanjredigerare**: Användaren har redigeringsåtkomst till alla Web Personalization-funktioner för att skapa, redigera och ta bort, men inte starta webbkampanjer.

**Startprogram för webbkampanjer**: Användaren har tillgång till alla funktioner i Personalization-appen för webben, utom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera, ta bort och starta webbkampanjer.

## Tilldela WP-roll till användare {#assign-wp-role-to-user}

1. Gå till **Användare**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Välj den användare som du vill ge WP-åtkomst till och klicka på **Redigera användare**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Välj WP-användarroll för alla arbetsytor.

   ![](assets/seven.png)

1. Nyligen aktiverade användare ser panelen **Web Personalization** i Min Marketo nästa gång de loggar in.

   ![](assets/eight.png)
