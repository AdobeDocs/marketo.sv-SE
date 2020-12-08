---
unique-page-id: 7504893
description: Lägg till Google AdWords som en startpunktstjänst med ett Manager-konto - Marketo Docs - Produktdokumentation
title: Lägg till Google AdWords som en startpunktstjänst med ett hanterarkonto
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Lägg till Google AdWords som en startpunktstjänst med ett hanterarkonto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Länka ditt Google AdWords-konto till Marketo för att automatiskt överföra konverteringsdata offline från Marketo till Google AdWords. Sedan kan ni från gränssnittet för AdWords enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg ni vill spåra) efter att ni har [lagt till anpassade kolumner](https://support.google.com/adwords/answer/3073556) i AdWords. Den här informationen visas inte i Marketo-gränssnittet.

Om du har flera Google Adwords-konton kan du använda ett [Google AdWords Manager-konto](https://www.google.com/adwords/manager-accounts/) (tidigare kallat My Client Center) för att integrera dem med Marketo.

Läs mer om [Googles importfunktion](https://support.google.com/adwords/answer/2998031?hl=en)för offlinekonvertering.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera ett [fristående Google AdWords-konto som en startpunktstjänst](add-google-adwords-as-a-launchpoint-service.md).

1. Gå till avsnittet **Admin** .

   ![](assets/login-admin-1.png)

1. Välj **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **Ny** och **Ny tjänst**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Ange ett visningsnamn och välj **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Välj **Authorize Marketo**.

   >[!NOTE]
   >
   >Se till att logga ut från ditt personliga Gmail-konto och aktivera popup-fönster.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Välj det konto som är kopplat till **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Välj **Acceptera**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Status visas som **Slutfört**. Välj **Nästa**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Ladda upp dina offlinekonverteringar från Marketo till Google AdWords **Weekly **eller **Daily**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Attributkonvertering till **första klickningen** eller **sista klicket**.

   | Typ | Definition |
   |---|---|
   | Första klickningen | Offlinekonverteringar tilldelas de första AdWords och den person som klickat de senaste 90 dagarna |
   | Sista klickningen | Offlinekonverteringar tilldelas de sista AdWords och som en person klickade på |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en) måste vara markerat för att den här funktionen ska fungera. Den måste aktiveras inuti AdWords.

1. Klicka på **Nästa**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Avmarkera konton som du inte vill uppdatera. Klicka på **Skapa**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Yippee! Se nu den relaterade artikeln nedan för hur du mappar AdWords-offlinekonverteringar i din intäktsmodell.

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >    
   >    
   >    * [Ange Google AdWords-konverteringar i intäktsmodellen med ett Manager-konto](../../../product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)


