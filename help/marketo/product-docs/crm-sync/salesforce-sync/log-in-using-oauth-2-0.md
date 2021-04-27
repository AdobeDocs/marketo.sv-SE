---
description: Logga in med OAuth 2.0 - Marketo Docs - produktdokumentation
title: Logga in med OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Logga in med OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce använder OAuth-protokollet för att tillåta användare av program att på ett säkert sätt få åtkomst till (autentisera programmet med OAuth 2.0) data utan att behöva visa inloggningsuppgifter. Nedan beskrivs de steg som ska utföras för att ansluta och synkronisera Marketo säkert med Salesforce.

## Konfigurera ansluten app {#set-up-connected-app}

1. Gå till Appar, App Manager och klicka på **Ny ansluten app** under Konfigurera i Salesforce.

   ![](assets/setting-up-oauth-2-1.png)

1. Fyll i informationen och klicka på **Spara**.

   ![](assets/setting-up-oauth-2-2.png)

1. Klicka i kryssrutan **Aktivera OAuth-inställningar**. Ange `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect` för återanrops-URL. Markera alla tillgängliga OAuth-scope och klicka på **Lägg till**.

   ![](assets/setting-up-oauth-2-3.png)

1. Klicka på **Spara**.

   ![](assets/setting-up-oauth-2-4.png)

1. Klicka på **Fortsätt**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copy the Consumer Key and Consumer Secret.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Spara informationen om konsumentnyckel och hemlighet för senare användning i Marketo.

## Konfigurera Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* API-åtkomst måste vara aktiverat för Salesforce Sync User (om du är Salesforce Professional Edition-användare är den åtkomsten inte tillgänglig som standard - kontakta din Salesforce Account Executive).
>* Marketo Sync-användare måste skapas i Salesforce.
>* För befintliga kunder är funktionen&quot;Aktivera OAuth för SFDC-synkronisering&quot; aktiverad i kundens prenumeration.
>* Popup-blockerare är inaktiverade.
>* Ansluten app skapas och vi har konsumentnyckeln och konsumenthemligheten tillgängliga för användning.


>[!CAUTION]
>
>Se till att du döljer alla fält som du inte behöver i Marketo för synkroniseringsanvändaren innan du klickar på **Synkronisera fält**. När du klickar på Synkronisera fält skapas alla fält som användaren kan se i SFDC permanent i Marketo och kan inte tas bort.

1. I avsnittet Marketo Admin klickar du på **CRM** och sedan på **Synkronisera med Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Lägg till information om konsumentnyckel och hemlighet som du tidigare spelat in och klicka på och **Spara**.

   ![](assets/setting-up-oauth-2-8.png)

1. Klicka på knappen **Logga in med Salesforce** på synkroniseringssidan för Marketo Salesforce.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Om du ser fält för användarnamn/lösenord/token och inte en inloggningsknapp för Salesforce aktiveras din Marketo-prenumeration för grundläggande autentisering. Se [Konfigurera Marketo med grundläggande autentisering](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). När synkroniseringen börjar med en uppsättning inloggningsuppgifter sker ingen växling av inloggningsuppgifter eller prenumeration för Salesforce. Om du vill använda Oauth 2.0 kontaktar du din Customer Success Manager.

1. Ett popup-fönster med inloggningssidan för Salesforce visas. Ange dina Marketo Sync-användaruppgifter och logga in.

   ![](assets/setting-up-oauth-2-10.png)

1. Ange verifieringskoden som du fick via e-post (skickas av Salesforce) och klicka på **Verifiera**.

   ![](assets/setting-up-oauth-2-11.png)

1. När verifieringen är klar visas åtkomstsidan och begär åtkomst. Klicka på **Tillåt**.

   ![](assets/setting-up-oauth-2-12.png)

1. Om några minuter visas ett popup-fönster i Marketo. Klicka på **Bekräfta inloggningsuppgifter**.

   ![](assets/setting-up-oauth-2-13.png)

1. När fältsynkroniseringen är klar klickar du på **Starta Salesforce-synkronisering**.

   ![](assets/setting-up-oauth-2-14.png)

1. Klicka på **Starta synkronisering**.

   ![](assets/setting-up-oauth-2-15.png)

Din synkronisering mellan Marketo och Salesforce pågår nu.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installera Marketo Sales Insight-paket i Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

