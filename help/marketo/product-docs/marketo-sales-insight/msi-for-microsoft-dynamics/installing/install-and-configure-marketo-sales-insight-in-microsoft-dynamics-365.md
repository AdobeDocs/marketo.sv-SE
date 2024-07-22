---
unique-page-id: 3571739
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till alla data som marknadsföringsteamet har. Så här installerar och konfigurerar du.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

1. Logga in på [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Klicka på menyn ![—](assets/image2015-3-16-16-1-13.png) och välj **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Klicka på menyn ![—](assets/image2015-5-13-10-5-8.png). I listrutan väljer du **Inställningar** och sedan **Lösningar**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Du bör redan ha [installerat och konfigurerat Marketo-lösningen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) innan du går vidare.

1. Klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **Bläddra** i det nya fönstret. Välj den [Marketo Sales Insight-lösning som du hämtade i steg 1](#msi). Klicka på **Nästa**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Lämna rutan **checked** och klicka på **Import**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt. Klicka på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Klicka på **Publish Alla anpassningar**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till Sales Insight i Dynamics. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och gå till avsnittet **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicka på **Redigera API-konfiguration** under avsnittet **Sales Insight**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **Marketo Host**, **API URL** och **API User Id** för användning i ett senare steg. Ange en **API-hemlig nyckel** som du väljer och klicka på **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för _både lead och kontakt_ för att Sales Insight ska fungera:
   >
   > * Prioritet
   > * Akut
   > * Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. I Microsoft Dynamics klickar du på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) bredvid Inställningar och väljer sedan **Marketo API Config** i listrutan.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Klicka på **Standardkonfiguration**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Ange den information som du kopierade från Marketo tidigare.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Klicka på ikonen ![](assets/image2015-5-13-16-3a8-3a51.png) längst ned till höger för att spara ändringarna.

## Ange användaråtkomst {#set-user-access}

Du måste ge användarna behörighet att använda Sales Insight.

1. Klicka på menyn ![](assets/image2015-5-13-10-3a5-3a8.png). I listrutan väljer du **Inställningar** och sedan **Dokumentskydd**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Klicka på **Användare**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Markera den eller de användare som du vill ge åtkomst till Sales Insight och klicka på **Hantera roller**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Välj rollen **Marketo Sales Insight** och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Nu har du låst upp styrkan hos Marketo Sales Insight för ditt säljteam.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
