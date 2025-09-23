---
unique-page-id: 3571800
description: Steg 3 av 3 -Connect Marketo and Salesforce (Professional) - Marketo Docs - produktdokumentation
title: Steg 3 av 3 -Connect Marketo och Salesforce (Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Steg 3 av 3: Anslut Marketo och [!DNL Salesforce] (Professional) {#step-of-connect-marketo-and-salesforce-professional}

I den här artikeln ska du konfigurera Marketo Engage att synkronisera med din konfigurerade Salesforce-instans.

>[!PREREQUISITES]
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## Hämta säkerhetstoken för synkroniserad användare {#retrieve-sync-user-security-token}

>[!TIP]
>
>Om du redan har en säkerhetstoken fortsätter du direkt till Ange synkronisering av användaruppgifter och kudos för förberedelse!

1. Logga in på Salesforce med Marketo Sync User, klicka på synkroniseringsanvändarens namn och sedan **[!UICONTROL My Settings]**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Skriv &quot;reset&quot; i navigeringsfältet och klicka på **[!UICONTROL Reset My Security Token]**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Klicka på **[!UICONTROL Reset Security Token]**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Säkerhetstoken skickas till dig via e-post.

## Ange användarautentiseringsuppgifter för synkronisering {#set-sync-user-credentials}

1. I Marketo går du till **[!UICONTROL Admin]**, väljer **[!UICONTROL CRM]** och klickar på **[!UICONTROL Sync with Salesforce.com]**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >[Dölj alla fält som du inte behöver](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} i Marketo från synkroniseringsanvändaren innan du klickar på **[!UICONTROL Sync Fields]**. När du klickar på Synkronisera fält skapas alla fält som användaren kan se i Marketo permanent och kan inte tas bort.

1. Ange inloggningsuppgifterna för Salesforce Sync-användare som skapades i del 2 av Salesforce-konfigurationen ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) och klicka på **[!UICONTROL Sync Fields]**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Kontrollera **[!UICONTROL Sandbox]** om du synkroniserar en Marketo-sandlåda till en Salesforce-sandlåda.

1. Läs varningen och klicka sedan på **[!UICONTROL Confirm Credentials]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Om du vill titta över [mappningarna och anpassa dem](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"} är detta den enda chansen att göra det! När du klickar på Starta Salesforce Sync är det klart.

## Starta [!DNL Salesforce]-synkronisering {#start-salesforce-sync}

1. Klicka på **[!UICONTROL Start Salesforce Sync]** för att påbörja den beständiga synkroniseringen mellan Marketo och Salesforce.

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

1. I Marketo klickar du på **[!UICONTROL Admin]** och sedan på **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Synkroniseringsstatusen visas längst upp till höger. Den visar ett av tre meddelanden: **[!UICONTROL Last Synced]**, **[!UICONTROL Sync in Progress]** eller **[!UICONTROL Failed]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Nu är du klar med att konfigurera en av de kraftfullaste funktionerna i Marketo!

>[!MORELIKETHIS]
>
>* [Installera Marketo Sales Insight-paketet i Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Konfigurera Marketo Sales Insight i Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
