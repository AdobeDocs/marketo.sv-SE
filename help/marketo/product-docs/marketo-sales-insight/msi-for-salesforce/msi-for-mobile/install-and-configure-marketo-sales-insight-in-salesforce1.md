---
unique-page-id: 7511512
description: Installera och konfigurera Marketo Sales Insight i Salesforce1 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Befintliga kunder, [uppgradera ditt MSI-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) innan du fortsätter!

>[!PREREQUISITES]
>
>Om du har Salesforce Enterprise/Unlimited:
>
>* [Steg 1 av 3: Lägg till Marketo-fält i Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en Salesforce-användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Steg 3 av 3: Anslut Marketo och Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Om du har Salesforce Professional:
>
>* [Konfigurera Marketo Sales Insight i Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 includes: Best Bets, Lead Feed, Intressant ögonblick, and Add to Marketo Campaign.

## Aktivera Salesforce1 Mobile App {#enable-the-salesforce1-mobile-app}

1. Klicka på **Konfigurera** och sedan på **Mobile Administration**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Klicka på **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Klicka på **Salesforce1-inställningar**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Klicka på **Aktivera Salesforce1-mobilwebbläsarappen**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Klicka på **Spara**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Välj **Mobiladministration**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Klicka på **Hantera mobil navigeringsmeny**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Välj **Marketo** och **Lägg till** i menyalternativen **Markerade**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Välj **Marketo**, flytta **uppåt** till önskat område och klicka på **Spara**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Dölj föråldrat anpassat Marketo-objekt {#hide-outdated-marketo-custom-object}

1. Klicka på **Konfigurera**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Välj **Hantera användare**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Välj **Profiler**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Klicka för att **redigera** om du vill ha profiler.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Under **Flikinställningar** väljer du _först_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Välj **Dold flik**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Se till att du döljer fliken Marketo för alla profiler du vill använda.

## Anpassa flikar {#customize-tabs}

1. Klicka på **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Klicka på **Anpassa mina flikar**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Välj **Marketo** och **Lägg till** i de markerade flikarna.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Välj **Marketo**, flytta **uppåt** till önskat område och klicka på **Spara**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka på **Konfigurera**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Klicka på **Utskriftsformat**, skriv **Sidlayouter** och klicka på **Sidlayouter** under Leads.

   >[!NOTE]
   >
   >Upprepa stegen för alla sidlayouter som används i organisationen (marknadsföring, försäljning, osv.) för objekten Kontakt, Konto och säljprojekt.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Klicka på **Redigera** för att göra ändringar i lead-layouten.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Klicka på **Visualforce-sidor** och dra sedan **Lead Mobile** till avsnittet Mobilkort.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Ändra höjden till 66 och klicka på **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Klicka på **Fält** och dra **Lägg till i Marketo Campaign** till avsnittet **Marketo Sales Insight**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Skriv&quot;Lägg till i&quot; i Snabbsökning så blir det enkelt att hitta Lägg till i Marketo Campaign.

1. Klicka på **Spara**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Phew! Nu är du klar med installationen av Marketo Sales Insight för Salesforce1! Ge dig själv en klapp på baksidan.

>[!MORELIKETHIS]
>
>* [Bästa val i Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Intressanta stunder i Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Skicka e-post och kampanjer och bevakningslistor från Marketo i Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
