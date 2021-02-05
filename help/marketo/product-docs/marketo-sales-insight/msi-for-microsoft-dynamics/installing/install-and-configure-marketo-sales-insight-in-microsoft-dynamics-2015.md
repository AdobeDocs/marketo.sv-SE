---
unique-page-id: 7513865
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2015 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2015
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till det stora datamängder som marknadsföringsteamet har. Så här installerar och konfigurerar du den i Microsoft Dynamics 2011

>[!PREREQUISITES]
>
>Slutför din [Marketo-Microsoft-integrering](http://docs.marketo.com/x/ZwBd).
>
>[Hämta rätt ](http://docs.marketo.com/x/LoJo) lösning för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

OK, nu är det dags att importera Marketo Sales Insight-lösningen till Microsoft Dynamics. Så här:

1. Klicka på **Inställningar** under Microsoft Dynamics CRM.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicka på **Anpassningar** under INSTÄLLNINGAR.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Klicka på **Lösningar**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Du bör redan ha installerat och konfigurerat Marketo-lösningen innan du går vidare.

1. Klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **Bläddra** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Hitta och välj den lösning du laddat ned ovan.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Lösningen överförs. Du kan visa paketinnehållet om du vill. Klicka på **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Se till att du inte markerar rutan och klicka på **Importera**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen och klicka sedan på **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss knyta din Marketo-instans till Sales Insight i Dynamics. Så här:

>[!NOTE]
>
>Administratörsrättigheter krävs.

1. Logga in på Marketo och gå till **Admin **sektionen.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Under avsnittet Sales Insight klickar du på **Redigera API-konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **Marketo Host**, **API URL** och **API User Id** för användning i ett senare steg. Ange en API-hemlig nyckel och klicka på **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för *både Lead och Contact* för att Sales Insight ska fungera:
   >
   >    
   >    
   >    * Prioritet
   >    * Akut
   >    * Relativa poäng

   >    
   >    
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de fält som saknas. Utför [den här proceduren](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) för att åtgärda detta.

1. Gå tillbaka i Microsoft Dynamics till **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Under **Inställningar** klickar du på **Marketo API Config**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicka på **Nytt**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Ange den information du tog från Marketo tidigare och klicka på **Spara**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Ange användaråtkomst {#set-user-access}

Slutligen måste du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Gå till **Säkerhet**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Klicka på **Användare**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Markera de användare som du vill ge åtkomst till Sales Insight till och klicka på **Hantera roller**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Markera Marketo Sales Insight-rollen och klicka på **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Du har nu låst upp kraften i Marketo Sales Insight för ditt säljteam.

>[!MORELIKETHIS]
>
>[Stjärnor och flamma för lead-/kontaktposter](http://docs.marketo.com/x/BICMAg)

