---
unique-page-id: 3571739
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---


# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till det stora datamängder som marknadsföringsteamet har. Så här installerar och konfigurerar du.

>[!PREREQUISITES]
>
>Slutför din [Marketo-Microsoft-integrering](http://docs.marketo.com/x/E4A2).
>
>[Hämta rätt ](http://docs.marketo.com/x/LoJo) lösning för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

1. Logga in på [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Klicka på menyn ![—](assets/image2015-3-16-16-1-13.png) och välj **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Klicka på menyn ![—](assets/image2015-5-13-10-5-8.png). I listrutan väljer du **Inställningar** och sedan **Lösningar**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Du bör redan ha [installerat och konfigurerat Marketo-lösningen](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) innan du går vidare.

   Klicka på Importera.
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **Bläddra** i det nya fönstret. Välj den [Marketo Sales Insight-lösning som du hämtade i steg 1](#msi). Klicka på **Nästa**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Lösningen överförs. Du kan visa paketinnehållet om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Se till att du inte markerar rutan **och klickar på** Importera **.**

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt. Klicka på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Klicka på **Publicera alla anpassningar**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss knyta din Marketo-instans till Sales Insight i Dynamics. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och gå till avsnittet **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicka på **Redigera API-konfiguration** under **Sales Insight**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **Marketo Host**, **API URL** och **API användar-ID** för användning i ett senare steg. Ange en **API-hemlig nyckel** och klicka på **SPARA**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för *både Lead och Contact* för att Sales Insight ska fungera:
   >
   > * Prioritet
   > * Akut
   > * Relativa poäng

   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de fält som saknas. Utför [den här proceduren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) för att åtgärda detta.

1. I Microsoft Dynamics klickar du på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) bredvid Inställningar och väljer sedan **Marketo API Config** i listrutan.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Klicka på **Standardkonfiguration**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Ange den information som du kopierade från Marketo tidigare.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Klicka på ikonen ![](assets/image2015-5-13-16-3a8-3a51.png) längst ned till höger för att spara ändringarna.

## Ange användaråtkomst {#set-user-access}

Du måste ge användarna behörighet att använda Sales Insight.

1. Klicka på menyn ![](assets/image2015-5-13-10-3a5-3a8.png). I listrutan väljer du **Inställningar** och sedan **Säkerhet**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Klicka på **Användare**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Markera den eller de användare som du vill ge åtkomst till Sales Insight till och klicka på **Hantera roller**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Välj rollen **Marketo Sales Insight** och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Du har nu låst upp kraften i Marketo Sales Insight för ditt säljteam.

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Stjärnor och flamma för lead-/kontaktposter](http://docs.marketo.com/x/BICMAg)