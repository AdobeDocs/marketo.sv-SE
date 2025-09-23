---
unique-page-id: 2360366
description: Steg 3 av 3 - Anslut Marketo och Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Steg 3 av 3 - Anslut Marketo och Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Steg 3 av 3: Anslut Marketo och [!DNL Salesforce] (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

I den här artikeln konfigurerar du Marketo att synkronisera med den konfigurerade [!DNL Salesforce]-instansen.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en [!DNL Salesforce] användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## Hämta säkerhetstoken för synkroniserad användare {#retrieve-sync-user-security-token}

>[!TIP]
>
>Om du redan har en säkerhetstoken fortsätter du direkt till Ange synkronisering av användaruppgifter och kudos för förberedelse!

1. Logga in på [!DNL Salesforce] med Marketo Sync User, klicka på synkroniseringsanvändarens namn och sedan på **[!UICONTROL My Settings]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Skriv &quot;reset&quot; i snabbsökningen och klicka på **[!UICONTROL Reset My Security Token]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Klicka på **[!UICONTROL Reset Security Token]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Säkerhetstoken skickas till dig via e-post.

## Ange användarautentiseringsuppgifter för synkronisering {#set-sync-user-credentials}

1. I Marketo går du till **[!UICONTROL Admin]**, väljer **CRM** och klickar på **[!UICONTROL Sync with Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >[Dölj alla fält som du inte behöver](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) i Marketo från synkroniseringsanvändaren innan du klickar på **[!UICONTROL Sync Fields]**. När du klickar på [!UICONTROL Sync Fields] skapas alla fält som användaren kan se permanent i Marketo och kan inte tas bort.

1. Ange de [!DNL Salesforce] synkroniseringsuppgifter för användare som skapades i del 2 av [!DNL Salesforce]-konfigurationen ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) eller [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) och klicka på **[!UICONTROL Sync Fields]** (markera bara **[!UICONTROL Sandbox]** om du synkroniserar en Marketo-sandlåda till en [!DNL Salesforce]-sandlåda).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Om du ser en inloggningsknapp för [!DNL Salesforce] i stället för användarnamn/lösenord/token-fält aktiveras din Marketo-prenumeration för OAuth. [se den här artikeln](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Så snart synkroniseringen börjar med en uppsättning autentiseringsuppgifter växlar **inte [!DNL Salesforce]-autentiseringsuppgifter eller prenumeration**. Kontakta din Customer Success Manager om du vill använda grundläggande autentisering.

1. Läs varningen och klicka sedan på **[!UICONTROL Confirm Credentials]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Om du vill titta över [mappningarna och anpassa dem](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md) är detta den enda chansen att göra det! När du klickar på [!UICONTROL Start  Salesforce Sync] är det klart.

## Starta [!DNL Salesforce]-synkronisering {#start-salesforce-sync}

1. Klicka på **[!UICONTROL Start  Salesforce Sync]** för att påbörja den beständiga Marketo-[!DNL Salesforce]-synkroniseringen.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo avduplicerar inte automatiskt mot en [!DNL Salesforce]-synkronisering eller när du anger leads manuellt.

1. Klicka på **[!UICONTROL Start Sync]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Tiden det tar att slutföra den inledande synkroniseringen varierar beroende på databasens storlek och komplexitet.

## Verifiera synkronisering {#verify-sync}

Marketo tillhandahåller statusmeddelanden för synkroniseringen [!DNL Salesforce] i administratörsområdet. Du kan kontrollera att synkroniseringen fungerar som den ska genom att följa dessa steg.

1. I Marketo klickar du på **[!UICONTROL Admin]** och sedan på **[!UICONTROL Salesforce]**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Synkroniseringsstatusen visas längst upp till höger. Den visar ett av tre meddelanden: **[!UICONTROL Last Synced]**, **[!UICONTROL Sync in Progress]** eller **[!UICONTROL Failed]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Nu är du klar med att konfigurera en av de kraftfullaste funktionerna i Marketo!

>[!MORELIKETHIS]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en [!DNL Salesforce] användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installera Marketo Sales Insight Package i [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurera Marketo Sales Insight i [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
