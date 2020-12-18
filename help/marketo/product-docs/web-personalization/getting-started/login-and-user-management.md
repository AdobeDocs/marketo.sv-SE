---
unique-page-id: 7513771
description: Inloggning och användarhantering - Marketo Docs - Produktdokumentation
title: Inloggning och användarhantering
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Inloggning och användarhantering {#login-and-user-management}

## Skapa en användarroll för webbanpassning {#create-a-web-personalization-user-role}

1. Gå till avsnittet **Admin** och klicka sedan på **Användare och roller**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicka på **Roller**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Om användarrollen Webbanpassning (WP) redan finns kontrollerar du att den är konfigurerad enligt steg 4.

1. Klicka på **Ny roll**.

   ![](assets/three-1.png)

1. Ange ett rollnamn och välj Behörigheter. Klicka på **Skapa** (den här rollen måste [gälla för alla arbetsytor](http://docs.marketo.com/display/DOCS/Managing+Marketo+Users#ManagingMarketoUsers-CreateUsers)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Om du vill ge användarna behörighet att komma åt allt i Mål och personalisering måste du markera *alla* kryssrutorna.

## Webbpersonalisering och användarbehörigheter för prediktivt innehåll {#web-personalization-and-predictive-content-user-permissions}

**Målinriktning och personalisering**: Användaren har endast behörighet att visa om den här behörigheten bara är markerad.

**Admin Web Personalization + Predictive**: Användaren har bara åtkomst till kontoinställningarna och innehållsinställningarna för appen Webbpersonalisering och Predictive Content. Användare kan visa sidor i programmet men har inte behörighet att skapa, redigera, ta bort eller starta.

**Predictive Content Editor**: Användaren har redigeringsåtkomst till programmet Predictive Content. Behörigheten gör att du kan skapa, redigera och ta bort innehållsdelar. Det går inte att aktivera innehåll för prediktiv användning på webben eller i e-post.

**Förutsägande** innehåll: Användaren har tillgång till alla funktioner för prediktivt innehåll, utom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera och ta bort och aktivera innehållsdelar.

**Webbkampanjredigerare**: Användaren har redigeringsåtkomst till alla webbpersonaliseringsfunktioner för att skapa, redigera och ta bort, men inte starta webbkampanjer.

**Web Campaign Launcher**: Användaren har tillgång till alla funktioner i appen Webbpersonalisering, förutom konto- och innehållsinställningar. Behörigheten ger möjlighet att skapa, redigera, ta bort och starta webbkampanjer.

## Tilldela WP-roll till användare {#assign-wp-role-to-user}

1. Gå till **Användare**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Välj den användare som ska beviljas WP-åtkomst och klicka på **Redigera användare**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Välj WP-användarroll för alla arbetsytor.

   ![](assets/seven.png)

1. Nyligen aktiverade användare ser **Webbanpassning**-panelen på Min marknad nästa gång de loggar in.

   ![](assets/eight.png)
