---
unique-page-id: 37355602
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---


# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till det stora datamängder som marknadsföringsteamet har. Så här installerar och konfigurerar du den i Microsoft Dynamics Online.

>[!NOTE]
>
>**Förutsättningar**
>
>Slutför er [Marketo-Microsoft-integrering](http://docs.marketo.com/x/E4A2).
>
>[Hämta rätt lösning](http://docs.marketo.com/x/LoJo) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

>[!NOTE]
>
>Om du använder det enhetliga gränssnittet, innan steg 1 nedan, klickar du på ikonen Inställningar i det övre högra hörnet och väljer **Avancerade inställningar**.

1. Klicka på **Inställningar** under Microsoft Dynamics CRM.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicka på **Anpassningar** under INSTÄLLNINGAR.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicka på **Lösningar**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Du bör redan ha installerat och konfigurerat Marketo-lösningen innan du går vidare.

1. Klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicka på **Bläddra** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Hitta och installera den lösning du just laddat ned på datorn.
1. Klicka på **Nästa**.

   ![](assets/seven.png)

1. Lösningen överförs. Du kan visa paketinnehållet om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Se till att du inte markerar rutan och klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Hämta loggfilen utan kostnad och klicka sedan på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/eleven.png)

1. Klicka på **Publicera anpassning**.

   >[!NOTE]
   >
   >Se till att aktivera den globala MS Dynamics-synkroniseringen.

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss knyta din Marketo-instans till Sales Insight i Dynamics. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och gå till **Admin **sektionen.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicka på **Redigera API-konfiguration** under Sales Insight.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopiera **Marketo Host**, **API URL** och **API User Id** för användning i ett senare steg. Ange en API-hemlig nyckel och klicka på **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för att *både Lead och Contact* for Sales Insight ska fungera:
   >
   >    
   >    
   >    * Prioritet
   >    * Akut
   >    * Relativa poäng

   >    
   >    
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de fält som saknas. Utför [den här proceduren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)för att åtgärda detta.

1. Gå tillbaka till Microsoft Dynamics, gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Under **Inställningar** klickar du på **Marketo API Config**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicka på **Nytt**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Ange den information du tog från Marketo tidigare och klicka på **Spara**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Aktivera synkronisering {#enable-sync}

1. I Marketo klickar du på **Admin**.

   ![](assets/enable-one.png)

1. Välj **Microsoft Dynamics** under Integrering.

   ![](assets/enable-two.png)

1. Klicka på **Aktivera synkronisering**.

   ![](assets/enable-three.png)

1. Klicka på **Redigera** bredvid Fältsynkroniseringsinformation.

   ![](assets/enable-four.png)

1. Detta väljer *automatiskt* MSI-fält som tidigare har inaktiverats (Urnummer, Relativ poäng och Prioritet). Klicka bara på **Spara** för att börja synkronisera data.

   ![](assets/enable-five.png)

## Ange användaråtkomst {#set-user-access}

Slutligen måste du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Gå till **Säkerhet**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicka på **Användare**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Markera de användare som du vill ge tillgång till Sales Insight och klicka på **Hantera roller**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Markera Marketo Sales Insight-rollen och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Stjärnor och flamma för lead-/kontaktposter](http://docs.marketo.com/x/BICMAg)

