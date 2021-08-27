---
unique-page-id: 2360366
description: Steg 3 av 3 - Anslut Marketo och Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 - Connect Marketo och Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Steg 3 av 3: Connect Marketo och Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

I den här artikeln konfigurerar du Marketo att synkronisera med din konfigurerade Salesforce-instans.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## Hämta säkerhetstoken för synkroniserad användare {#retrieve-sync-user-security-token}

>[!TIP]
>
>Om du redan har en säkerhetstoken fortsätter du direkt till Ange synkronisering av användaruppgifter och kudos för förberedelse!

1. Logga in i Salesforce med Marketo Sync User, klicka på synkroniseringsanvändarens namn och **Mina inställningar**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Skriv &quot;reset&quot; i snabbsökningen och klicka på **Återställ min säkerhetstoken**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Klicka på **Återställ säkerhetstoken**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Säkerhetstoken skickas till dig via e-post.

## Ange användarautentiseringsuppgifter för synkronisering {#set-sync-user-credentials}

1. I Marketo går du till **Admin**, väljer **CRM** och klickar på **Synkronisera med [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Var noga med att [dölja alla fält som du inte behöver](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) i Marketo från synkroniseringsanvändaren innan du klickar på **Synkronisera fält**. När du klickar på Synkronisera fält skapas alla fält som användaren kan se i Marketo permanent och kan inte tas bort.

1. Ange inloggningsuppgifterna för Salesforce Sync User som skapades i del 2 av Salesforce-konfigurationen ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) eller [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) och klicka på **Synkronisera fält** (markera **Sandbox** endast om du synkroniserar en Marketo-sandlåda till en Salesforce-sandlåda).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Om du ser knappen Logga in i Salesforce i stället för fälten Användarnamn/Lösenord/Token aktiveras din Marketo-prenumeration för OAuth. [se den här artikeln](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). När synkroniseringen börjar med en uppsättning autentiseringsuppgifter är det **ingen växling av Salesforce-autentiseringsuppgifter eller prenumeration**. Om du vill använda grundläggande autentisering kontaktar du din Customer Success Manager.

1. Läs varningen och klicka sedan på **Bekräfta inloggningsuppgifter**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Om du vill titta över [mappningarna och anpassa dem](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md) är detta den enda chansen att göra det! När du klickar på Starta Salesforce-synkronisering är det klart.

## Starta Salesforce-synkronisering {#start-salesforce-sync}

1. Klicka på **Starta Salesforce-synkronisering** för att starta den beständiga Marketo-Salesforce-synkroniseringen.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo avlastar inte automatiskt från en Salesforce-synkronisering eller när du anger leads manuellt.

1. Klicka på **Starta synkronisering**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Tiden det tar att slutföra den inledande synkroniseringen varierar beroende på databasens storlek och komplexitet.

## Verifiera synkronisering {#verify-sync}

Marketo tillhandahåller statusmeddelanden för Salesforce-synkronisering i administrationsområdet. Du kan kontrollera att synkroniseringen fungerar som den ska genom att följa dessa steg.

1. I Marketo klickar du på **Admin** och sedan **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Synkroniseringsstatusen visas i det övre högra hörnet. Den visar ett av tre meddelanden: **Senaste synkronisering**, **Synkronisering pågår** eller **Misslyckades**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Nu är du klar med att konfigurera en av de kraftfullaste funktionerna i Marketo!

>[!MORELIKETHIS]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installera Marketo Sales Insight-paket i Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

