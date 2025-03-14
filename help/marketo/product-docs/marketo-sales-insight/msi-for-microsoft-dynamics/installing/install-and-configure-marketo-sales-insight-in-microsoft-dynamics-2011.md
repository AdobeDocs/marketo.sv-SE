---
unique-page-id: 3571735
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2011 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för ert säljteam. Här följer den stegvisa instruktionen om hur du installerar och konfigurerar den i Microsoft Dynamics 2011 On-Premises.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

1. Logga in på Microsoft Dynamics CRM. Klicka på **Inställningar** i den nedre vänstra menyn.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Välj **Lösningar** i trädet.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicka på **Importera** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Du bör redan ha [installerat och konfigurerat](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo-lösningen innan du går vidare.

1. Klicka på **Bläddra**. Välj den Marketo Sales Insight-lösning som du [hämtade](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Klicka på **Nästa**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifiera informationen om lösningen och klicka på **Nästa**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Kontrollera att alternativet SDK-meddelande är markerat. Klicka på **Nästa**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Vänta nu tills importen är klar.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicka på **Stäng**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight visas nu i lösningslistan. Ja!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Välj Marketo Sales Insight och klicka på **Publish All Customizations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo och Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och klicka på **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Under avsnittet **Sales Insight** klickar du på **Redigera API-konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **Marketo Host**, **API URL** och **API User Id** för användning i ett senare steg. Ange en **API-hemlig nyckel** som du väljer och klicka på **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för _både lead och kontakt_ för att Sales Insight ska fungera:
   >
   >* Prioritet
   >* Akut
   >* Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. Gå tillbaka till Dynamics och välj **Inställningar**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Välj **Marketo API-konfiguration** i trädet.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicka på **Standardkonfiguration**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Ange den information du tog från Marketo tidigare.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicka på **Spara**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Ange användaråtkomst {#set-user-access}

Konfigurera användarroller för att ge specifika användare åtkomst till Sales Insight.

1. Välj **Inställningar**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Välj **Administration** i trädet.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicka på **Användare**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Markera de användare som du vill ge åtkomst till och klicka på **Hantera roller**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Välj rollen **Marketo Sales Insight** och klicka på **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Och det är allt! Alla användare har tillgång till det här avsnittet med säljinsikter i vyn för lead-/kontaktinformation.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Grattis. Nu har du släppt loss kraften i Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
