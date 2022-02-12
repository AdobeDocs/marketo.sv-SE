---
description: Inställningar för inloggningshantering - Marketo Docs - produktdokumentation
title: Inställningar för inloggningshantering
hide: true
hidefromtoc: true
source-git-commit: e3d175d9f6131ec9798c4047ccf79858c254c745
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Inställningar för inloggningshantering {#login-management-settings}

Inställningarna för inloggningshantering gör att administratörer kan ange autentiseringsinställningar för användare av Sales Insight-åtgärder på global nivå.

>[!NOTE]
>
>Som standard markeras alternativet Endast Salesforce för instanser av Sales Insight Actions. Vi rekommenderar den här inställningen så att användare kan [automatisk inloggning](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) från Salesforce.

## Uppdatera inställningar för inloggningshantering {#update-login-management-settings}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Följ de här stegen för att uppdatera dina inställningar för inloggningshantering.

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/login-management-settings-1.png)

1. Under Administratörsinställningar klickar du på **Allmänt**.

   ![](assets/login-management-settings-2.png)

1. Bläddra ned till inloggningshanteringskortet och välj önskad inställning (i det här exemplet väljer vi endast Salesforce). Klicka **Spara** när det är klart.

   ![](assets/login-management-settings-3.png)

## Vanliga frågor om enbart Salesforce {#salesforce-only-faq}

Endast Salesforce innebär att användare bara kan autentisera sig för att använda Sales Insight-åtgärder med Salesforce. Det är standardvalet för instanser av Sales Insight Actions och rekommenderas eftersom användaren kan autentisera utan att behöva hantera användarnamn och lösenord.

### Hur aktiverar en ny användare till min instans sitt konto när&quot;Endast Salesforce&quot; har valts? {#activate-when-salesforce-only-is-selected}

När du klickar på **Komma igång** i e-postmeddelandet med en inbjudan skickas nya användare till en kontoaktiveringsskärm där de måste ansluta sin Salesforce-instans för att aktivera sitt konto för Sales Insight Actions.

![](assets/login-management-settings-4.png)

### Vilka autentiseringsmetoder får mina användare autentisera med när&quot;Endast Salesforce&quot; har valts? {#what-authentication-methods}

När användaren navigerar till inloggningsskärmen anger han/hon först sin e-postadress. Sedan klickar de på Salesforce One Click Login, där de kan autentisera med det Salesforce-konto de är inloggade på.

>[!NOTE]
>
>Detta gäller endast användare som navigerar direkt till inloggningsskärmen. Användare som använder åtgärder från Salesforce loggas in med [Automatisk inloggning](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Hur hanteras användarautentisering för åtgärder när en användare öppnar en åtgärdsfunktion från Salesforce och&quot;Endast Salesforce&quot; har valts? {#how-is-user-authentication-handled}

När en användare klickar på en av åtgärderna (Samtal, E-post, Kampanj, Uppgifter, Kampanjlista osv.) använder vi deras SFDC-autentisering för att automatiskt logga in dem på deras konto för Sales Insight Actions. Vi anropar den här autentiseringen [Automatisk inloggning](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Vanliga frågor om alla inloggningsmetoder {#all-login-methods-faq}

### Hur aktiverar en ny användare till min instans sitt konto när Alla inloggningsmetoder har valts? {#activate-when-all-login-methods-is-selected}

När en ny användare bjuds in till en instans får de ett e-postmeddelande om kontoaktivering. De klickar på knappen &quot;Kom igång&quot; som sedan tar dem till en sida där de ombeds att skapa och bekräfta ett lösenord. När detta är skapat aktiveras deras konto och tas via introduktionsarbetsflödet.

![](assets/login-management-settings-6.png)

### Vilka användare av min instans får logga in med när Alla inloggningsmetoder har valts? {#what-are-users-allowed-to-log-in-with-all-login}

När du använder vår inloggningssida anger användarna först sin e-postadress. Därefter skickas de till en sida som ger dem alla inloggningsalternativ (användarnamn/lösenord, SFDC, Gmail, SSO) att autentisera med.
