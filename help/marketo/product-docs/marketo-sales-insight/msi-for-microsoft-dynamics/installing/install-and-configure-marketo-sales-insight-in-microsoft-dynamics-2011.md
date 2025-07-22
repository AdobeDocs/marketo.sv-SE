---
unique-page-id: 3571735
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2011 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 2%

---

# Installera och konfigurera [!DNL Marketo Sales Insight] i [!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] är ett fantastiskt verktyg för ditt säljteam. Här följer en steg-för-steg-instruktion om hur du installerar och konfigurerar den i [!DNL Microsoft Dynamics 2011] lokal.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av [!DNL Microsoft Dynamics] CRM.

## Importera lösning {#import-solution}

1. Logga in på [!DNL Microsoft Dynamics] CRM. Klicka på **[!UICONTROL Settings]** i den nedre vänstra menyn.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Välj **[!UICONTROL Solutions]** i trädet.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Klicka på **Importera** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Du bör redan ha [installerat och konfigurerat](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo-lösningen innan du går vidare.

1. Klicka på **[!UICONTROL Browse]**. Välj den [!DNL Marketo Sales Insight]-lösning du [hämtade](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifiera informationen om lösningen och klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Kontrollera att meddelandealternativet för SDK är markerat. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Vänta nu tills importen är klar.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Klicka på **[!UICONTROL Close]**.

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] visas nu i lösningslistan. Ja!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Välj [!DNL Marketo Sales Insight] och klicka på **Publicera alla anpassningar** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo och Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och klicka på **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicka på **[!UICONTROL Sales Insight]** under avsnittet **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** och **[!UICONTROL API User Id]** för användning i ett senare steg. Ange en **[!UICONTROL API Secret Key]** och klicka på **[!UICONTROL Save]**.

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

1. Gå tillbaka till Dynamics, välj **[!UICONTROL Settings]**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Välj **[!UICONTROL Marketo API Config]** i trädet.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Klicka på **[!UICONTROL Default Configuration]**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Ange den information du tog från Marketo tidigare.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Ange användaråtkomst {#set-user-access}

Konfigurera användarroller för att ge specifika användare åtkomst till [!DNL Sales Insight].

1. Välj **[!UICONTROL Settings]**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Välj **[!UICONTROL Administration]** i trädet.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Markera de användare som du vill ge åtkomst till och klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Välj rollen **[!UICONTROL Marketo Sales Insight]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Och det är allt! Alla användare har tillgång till det här avsnittet med säljinsikter i vyn för lead-/kontaktinformation.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Grattis. Du har nu frigjort kraften hos [!DNL Marketo Sales Insight].

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
