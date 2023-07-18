---
description: Ställ in en Sales Insight Actions Sandbox - Marketo Docs - Product Documentation
title: Ställ in en säkerhetssandlåda för Sales Insight Actions
source-git-commit: 15c3124a53ce55810b598c43e29e21321534c81f
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Ställ in en säkerhetssandlåda för Sales Insight Actions {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions är ett webbaserat program som integreras med Salesforce-användargränssnittet via [Marketo Sales Insight-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Det kallas ibland&quot;Marketo Sales&quot; eller&quot;Actions&quot;.

Om du har en Marketo-sandlåda kan du aktivera en Actions-instans som ska användas med din sandlåda i testsyfte.

När du konfigurerar en Actions-instans måste du bestämma om den ska konfigureras för att fungera med Salesforce-sandlådan eller Salesforce-produktion. Det beror på att Salesforce använder olika slutpunkter för varje, och att Åtgärder använder anslutningen till Salesforce för att aktivera och autentisera användare.

Följ stegen nedan för att få en Actions-instans konfigurerad att fungera med din Salesforce-sandlådeinstans.

>[!NOTE]
>
>Du kan lära dig mer om hur användarna [aktivera sin åtgärdsplats](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. You can also learn about how users will [authenticate with Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Additionally, if you prefer to have users authenticate with email and password, you can learn more about this in our [Login Management settings article](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Begär att en åtgärdsinstans ska etableras i din Marketo-sandlåda {#request=an-actions-instance}

Sales Insight-åtgärder är inte aktiverade för Marketo Sandbox-instanser om det inte begärs. Kontakta kontoteamet (din kontoansvarige) på Adobe för att skicka en begäran.

## Ange ditt åtgärdskonto för Marketo Sandbox {#provision-your-actions-account}

När Åtgärder har aktiverats för Marketo Sandbox måste du följa stegen nedan för att aktivera den nya instansen.

1. Logga in på din Marketo Sandbox-instans.

1. Navigera till **Administratör**.

1. Välj **Försäljningsinsikter**.

1. Välj **Åtgärdskonfiguration**.

   >[!IMPORTANT]
   >
   >En e-postadress kan bara användas för en åtgärdsinstans i både sandbox- och Production-instanser. Om du är administratör och behöver ha tillgång till flera instanser i Production och Sandbox måste du använda olika e-postadresser för var och en av dem.

1. I provisioneringskortet väljer du den användare du vill bjuda in till instansen Sales Insight Actions.

## Aktivera åtgärdsinstansen {#activate-your-actions-instance}

Din Actions-instans måste aktiveras med ett Salesforce-produktionskonto. När den har aktiverats kan den växlas till ett Salesforce-sandlådekonto.

1. Leta reda på inbjudan som skickats.

1. Klicka på **Kom igång** Länk.

1. Aktivera med Salesforce Production-instansen.

1. Följ instruktionerna för att konfigurera kontot. Mer information finns i [Artikeln om användarintroduktion](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Förbered åtgärdsinstansen så att den är kompatibel med din Salesforce-sandlådeinstans {#prepare-your-actions-instance}

Åtgärder kräver att du först aktiverar en ny instans med en Salesforce-produktionsanvändare. När den har aktiverats kan du använda följande steg för att förbereda din instans så att den blir Salesforce Sandbox-kompatibel.

1. Uppdatera inloggningsinställningarna till Alla inloggningsmetoder, så att du kan logga in med ett användarnamn och lösenord om det behövs. Om du vill kan du växla tillbaka till&quot;Endast Salesforce&quot; när allt har konfigurerats. [Se hur man gör detta här](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Koppla från Salesforce-produktion och anslut till din Salesforce-sandlåda. [Se hur du ansluter här](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. I steg 3 väljer du&quot;Sandbox&quot; i stället för&quot;Salesforce&quot;. Om du redan är ansluten bör du se ett alternativ för att koppla från på fliken Salesforce-anslutningar och -anpassningar.

>[!NOTE]
>
>Om du har en anpassad domän för din Salesforce-instans rekommenderar vi att du loggar in på din Salesforce-instans innan du ansluter till Salesforce eller loggar in på Åtgärder.

## Begär att din åtgärdsinstans ska konverteras så att den är kompatibel med din Salesforce-sandlåda {#request-your-actions-instance-be-converted}

1. Kontakt [Stöd för Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} för att begära att din nya instans av Sales Insight Actions konfigureras som kompatibel med Salesforce Sandbox.

1. Testa att allt är korrekt konfigurerat genom att försöka logga in med knappen&quot;Logga in med Salesforce&quot; på toutapp.com/login.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Om du stöter på problem kan du begära en lösenordsåterställning och använda ett lösenord för att återfå åtkomsten till ditt konto.

Nu är din instans klar att användas med din Salesforce-sandlådeinstans. Om du vill använda [Automatisk inloggning för Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} from Salesforce, you can switch back to "Salesforce Only" in your [Login Management settings](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Koppla ditt konto för Sales Insight Actions till Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Handbok om User Onboarding för Sales Insight Actions](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Automatisk inloggning från Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Inställningar för inloggningshantering](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
