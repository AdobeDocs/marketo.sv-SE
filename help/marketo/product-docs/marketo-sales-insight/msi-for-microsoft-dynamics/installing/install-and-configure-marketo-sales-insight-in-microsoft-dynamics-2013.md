---
unique-page-id: 3571737
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till alla data som marknadsföringsteamet har. Så här installerar och konfigurerar du den.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Ladda ned rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av Microsoft Dynamics CRM.

## Importera lösning {#import-solution}

OK, nu är det dags att importera Marketo Sales Insight-lösningen till Microsoft Dynamics.

1. Under **Microsoft Dynamics CRM** klicka **Inställningar**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Under **Inställningar**, klicka **Anpassningar**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Klicka **Lösningar**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Du bör redan ha installerat och konfigurerat Marketo innan du går vidare

1. Klicka **Importera**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **Bläddra**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Hitta och välj den lösning du laddat ned ovan.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicka **Nästa**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Lösningen överförs. Du kan visa paketinnehållet om du vill. Klicka **Nästa**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Se till att du inte markerar rutan och klicka **Importera**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt. Klicka **Stäng**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till Sales Insight i Dynamics.

>[!NOTE]
>
>Administratörsrättigheter krävs.

1. Logga in på Marketo och gå till **Administratör** -avsnitt.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Under **Försäljningsinsikter** avsnittsklicka **Redigera API-konfiguration**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **Marketo Host**, **API-URL** och **API-användar-ID** för användning i ett senare steg. Ange en **API-hemlig nyckel** efter eget val och klicka **Spara**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för _både lead och kontakt_ för Sales Insight att arbeta:
   >
   >* Prioritet
   >* Akut
   >* Relativa poäng

   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Åtgärda problemet genom att utföra [detta förfarande](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Tillbaka i Microsoft Dynamics, gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Under **Inställningar**, klicka **Marketo API Config**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicka **Nytt**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Ange den information du tog från Marketo tidigare och klicka på **Spara**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Ange användaråtkomst {#set-user-access}

Slutligen kan du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **Inställningar**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Klicka **Användare**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Välj den eller de användare som du vill ge tillgång till Sales Insight till och klicka på **Hantera roller**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Välj **Marketo Sales Insight** roll och klicka **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Slutligen, för att testa, logga in i Dynamics som en användare som har tillgång till Marketo Sales Insight och titta på en lead eller kontakt.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Nu har du låst upp styrkan hos Marketo Sales Insight för ditt säljteam.

>[!MORELIKETHIS]
>
>[Stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
