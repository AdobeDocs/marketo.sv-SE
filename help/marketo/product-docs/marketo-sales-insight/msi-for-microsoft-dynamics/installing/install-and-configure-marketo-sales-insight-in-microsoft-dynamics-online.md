---
unique-page-id: 37355602
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till alla data som marknadsföringsteamet har. Så här installerar och konfigurerar du den i Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

>[!NOTE]
>
>Om du använder det enhetliga gränssnittet, innan steg 1 nedan, klickar du på ikonen Inställningar i det övre högra hörnet och väljer **Avancerade inställningar**.

1. Klicka på **Inställningar** under Microsoft Dynamics CRM.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicka på **Anpassningar** under Inställningar.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicka på **Lösningar**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Du bör redan ha installerat och konfigurerat Marketo-lösningen innan du går vidare.

1. Klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicka på **Bläddra** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Hitta och installera den lösning du just laddat ned på datorn.

1. Klicka på **Nästa**.

   ![](assets/seven.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Se till att du inte markerar rutan och klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Hämta loggfilen kostnadsfritt och klicka sedan på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/eleven.png)

1. Klicka på **Publish Customization**.

   >[!NOTE]
   >
   >Se till att aktivera den globala MS Dynamics-synkroniseringen.

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till Sales Insight i Dynamics. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in i Marketo och gå till avsnittet **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicka på **Redigera API-konfiguration** under avsnittet Sales Insight.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopiera **Marketo Host**, **API URL** och **API User Id** för användning i ett senare steg. Ange en valfri API-hemlig nyckel och klicka på **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Klicka på **Marketo API-konfiguration** under **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicka på **Ny**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Ange den information du tog från Marketo tidigare och klicka på **Spara**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **Admin** i Marketo.

   ![](assets/enable-one.png)

1. Under Integrering väljer du **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Klicka på **Aktivera synkronisering**.

   ![](assets/enable-three.png)

1. Klicka på **Redigera** bredvid Fältsynkroniseringsinformation.

   ![](assets/enable-four.png)

1. Detta _markerar automatiskt_ MSI-fält som tidigare har inaktiverats (trängsel, relativ poäng och prioritet). Klicka bara på **Spara** för att börja synkronisera data.

   ![](assets/enable-five.png)

## Ange användaråtkomst {#set-user-access}

Slutligen måste du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Gå till **Säkerhet**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicka på **Användare**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Markera de användare som du vill ge åtkomst till Sales Insight och klicka på **Hantera roller**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Välj rollen Marketo Sales Insight och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
