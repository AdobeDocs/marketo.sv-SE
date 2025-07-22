---
unique-page-id: 7511512
description: Installera och konfigurera Marketo Sales Insight i Salesforce1 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 4%

---

# Installera och konfigurera [!DNL Marketo Sales Insight] i [!DNL Salesforce1] {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Befintliga kunder, [uppgradera ditt MSI-paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) innan du fortsätter!

>[!PREREQUISITES]
>
>Om du har Salesforce Enterprise/Unlimited:
>
>* [Steg 1 av 3: Lägg till Marketo-fält i [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Steg 2 av 3: Skapa en [!DNL Salesforce] användare för Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Steg 3 av 3: Anslut Marketo och [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Konfigurera [!DNL Marketo Sales Insight] i [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Om du har Salesforce Professional:
>
>* [Konfigurera Marketo Sales Insight i Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>[!DNL Marketo Sales Insight] i [!DNL Salesforce1] innehåller: [!DNLBest Bets], lead feed, Intressant ögonblick och Add to Marketo Campaign.

## Aktivera mobilappen [!DNL Salesforce1] {#enable-the-salesforce1-mobile-app}

1. Klicka på **[!DNL Setup]** och sedan på **[!DNL Mobile Administration]**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Klicka på **[!UICONTROL Salesforce1]**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Klicka på **[!UICONTROL Salesforce1 Settings]**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Klicka på **[!UICONTROL Enable the Salesforce1 mobile browser app]**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Välj **[!UICONTROL Mobile Administration]**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Klicka på **[!UICONTROL Manage the mobile navigation menu]**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Välj **[!UICONTROL Marketo]** och **[!UICONTROL Add]** till menyalternativen på **[!UICONTROL Selected]**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Välj **[!UICONTROL Marketo]**, flytta **[!UICONTROL Up]** till önskat område och klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Dölj föråldrat anpassat Marketo-objekt {#hide-outdated-marketo-custom-object}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Välj **[!UICONTROL Manage Users]**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Välj **[!UICONTROL Profiles]**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Klicka för att **[!UICONTROL Edit]** om du vill ha profiler.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Under **[!UICONTROL Tab Settings]** väljer du _first_ **[!UICONTROL Marketo]**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Välj **[!UICONTROL Tab Hidden]**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Se till att du döljer fliken Marketo för alla profiler du vill använda.

## Anpassa flikar {#customize-tabs}

1. Klicka på **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Klicka på **[!UICONTROL Customize My Tabs]**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Markera **[!UICONTROL Marketo]** och **[!UICONTROL Add]** den på de markerade flikarna.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Välj **[!UICONTROL Marketo]**, flytta **[!UICONTROL Up]** till önskat område och klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Anpassa sidlayouter {#customize-page-layouts}

1. Klicka på **[!UICONTROL Setup]**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Klicka på **[!UICONTROL Setup]**, skriv **[!UICONTROL Page Layouts]** och klicka på **[!UICONTROL Page Layouts]** under Leads.

   >[!NOTE]
   >
   >Upprepa stegen för varje sidlayout som din organisation använder (marknadsföring, försäljning osv.) för objekten Kontakt, Konto och Möjlighet.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Klicka på **[!UICONTROL Edit]** om du vill ändra lead-layouten.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Klicka på **[!UICONTROL Visualforce Pages]** och dra sedan **[!UICONTROL Lead Mobile]** till avsnittet Mobilkort.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Ändra höjden till 66 och klicka på **[!UICONTROL OK]**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Klicka på **[!UICONTROL Fields]** och dra **[!UICONTROL Add to Marketo Campaign]** till avsnittet **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Skriv&quot;Lägg till i&quot; i Snabbsökning så blir det enkelt att hitta Lägg till i Marketo Campaign.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Phew! Du har nu installerat [!DNL Marketo Sales Insight] för [!DNL Salesforce1]! Ge dig själv en klapp på baksidan.

>[!MORELIKETHIS]
>
>* [[!DNL Best Bets] in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Intressanta stunder i [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Skicka Marketo-åtgärder för e-post och kampanj och bevakning i [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
