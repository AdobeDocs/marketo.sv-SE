---
unique-page-id: 3571737
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till alla data som marknadsföringsteamet har. Så här installerar och konfigurerar du den.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

OK, nu är det dags att importera Marketo Sales Insight-lösningen till Microsoft Dynamics.

1. Under **Microsoft Dynamics CRM** klickar du på **Inställningar**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicka på **Anpassningar** under **Inställningar**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Klicka på **Lösningar**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Du bör redan ha installerat och konfigurerat Marketo innan du går vidare

1. Klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **Bläddra** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Hitta och välj den lösning du laddat ned ovan.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Se till att du inte markerar rutan och klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt. Klicka på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till Sales Insight i Dynamics.

>[!NOTE]
>
>Administratörsrättigheter krävs.

1. Logga in på Marketo och gå till avsnittet **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Under avsnittet **Sales Insight** klickar du på **Redigera API-konfiguration**.

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
   >* Prioritet
   >* Akut
   >* Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. Gå tillbaka till Microsoft Dynamics och gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Klicka på **Marketo API-konfiguration** under **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicka på **Ny**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Ange den information du tog från Marketo tidigare och klicka på **Spara**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Ange användaråtkomst {#set-user-access}

Slutligen kan du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Klicka på **Användare**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Markera den eller de användare som du vill ge åtkomst till Sales Insight och klicka på **Hantera roller**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Välj rollen **Marketo Sales Insight** och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Slutligen, för att testa, loggar du in i Dynamics som en användare som har tillgång till Marketo Sales Insight och tittar på ett lead eller en kontakt.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Nu har du låst upp styrkan hos Marketo Sales Insight för ditt säljteam.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
