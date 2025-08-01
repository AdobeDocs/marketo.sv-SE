---
description: Inloggningshanteringsinställningar - Marketo Docs - produktdokumentation
title: Inställningar för inloggningshantering
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Inställningar för inloggningshantering {#login-management-settings}

Inställningarna för inloggningshantering gör att administratörer kan ange autentiseringsinställningar för användare av Sales Insight-åtgärder på global nivå.

>[!NOTE]
>
>Som standard markeras alternativet [!UICONTROL Salesforce Only] för [!DNL Sales Insight Actions] instanser. Vi rekommenderar den här inställningen så att användare kan [logga in automatiskt](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) från [!DNL Salesforce].

## Uppdatera inställningar för inloggningshantering {#update-login-management-settings}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Följ de här stegen för att uppdatera dina inställningar för inloggningshantering.

1. Klicka på kugghjulsikonen och välj **[!UICONTROL Settings]**.

   ![](assets/login-management-settings-1.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL General]**.

   ![](assets/login-management-settings-2.png)

1. Bläddra ned till [!UICONTROL Login Management]-kortet och välj önskad inställning (i det här exemplet väljer vi endast Salesforce). Klicka på **[!UICONTROL Save]** när du är klar.

   ![](assets/login-management-settings-3.png)

## Vanliga frågor om endast Salesforce {#salesforce-only-faq}

Salesforce betyder bara att användare bara kan autentisera för att använda [!DNL Sales Insight Actions] med [!DNL Salesforce]. Det är standardvalet för [!DNL Sales Insight Actions] instanser och rekommenderas eftersom användare kan autentisera sömlöst utan att behöva hantera användarnamn och lösenord.

### Hur aktiverar en ny användare till min instans sitt konto när [!UICONTROL Salesforce Only] har valts? {#activate-when-salesforce-only-is-selected}

När du klickar på knappen **[!UICONTROL Getting Started]** i e-postmeddelandet med en inbjudan skickas nya användare till en kontoaktiveringsskärm där de måste ansluta sin Salesforce-instans för att aktivera sitt [!DNL Sales Insight Actions]-konto.

![](assets/login-management-settings-4.png)

### Vilka autentiseringsmetoder får mina användare autentisera med när [!UICONTROL Salesforce Only] väljs? {#what-authentication-methods}

När användaren navigerar till inloggningsskärmen anger han/hon först sin e-postadress. Sedan klickar de på Salesforce One Click [!UICONTROL Login] där de kan autentisera med det Salesforce-konto de är inloggade på.

>[!NOTE]
>
>Detta gäller endast användare som navigerar direkt till inloggningsskärmen. Användare som använder åtgärder från [!DNL Salesforce] loggas in med [Automatisk inloggning](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Hur hanteras användarautentisering för funktionsmakron när en användare öppnar en funktionsmakron från Salesforce och&quot;Endast Salesforce&quot; har valts? {#how-is-user-authentication-handled}

När en användare klickar på en av åtgärderna (samtal, e-post, kampanj, uppgifter, kampanjlista osv.) använder vi deras SFDC-autentisering för att automatiskt logga in dem på deras [!DNL Sales Insight Actions]-konto. Den här autentiseringen anropas [vid automatisk inloggning](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Vanliga frågor om alla inloggningsmetoder {#all-login-methods-faq}

### Hur aktiverar en ny användare till min instans sitt konto när Alla inloggningsmetoder har valts? {#activate-when-all-login-methods-is-selected}

När en ny användare bjuds in till en instans får de ett e-postmeddelande om kontoaktivering. De klickar på knappen &quot;Kom igång&quot; som sedan tar dem till en sida där de ombeds att skapa och bekräfta ett lösenord. När detta är skapat aktiveras deras konto och tas via introduktionsarbetsflödet.

![](assets/login-management-settings-6.png)

### Vilka användare av min instans får logga in med när [!UICONTROL All Login Methods] har valts? {#what-are-users-allowed-to-log-in-with-all-login}

När du använder vår inloggningssida anger användarna först sin e-postadress. Därefter skickas de till en sida som ger dem alla inloggningsalternativ (användarnamn/lösenord, SFDC, Gmail, SSO) att autentisera med.
