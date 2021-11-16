---
unique-page-id: 6095008
description: Lägg till Google AdWords som en LaunchPoint-tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Google AdWords som en LaunchPoint-tjänst
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Lägg till Google AdWords som en LaunchPoint-tjänst {#add-google-adwords-as-a-launchpoint-service}

Länka ditt Google AdWords-konto till Marketo för att automatiskt överföra offlinekonverteringsdata från Marketo till Google AdWords. Sedan kan ni utifrån AdWords-gränssnittet enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg ni vill spåra) efter att ni gjort det [lägga till egna kolumner](https://support.google.com/adwords/answer/3073556) i AdWords. Den här informationen visas inte i användargränssnittet för Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din Customer Success Manager för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera en [Google AdWords as a Launchpoint service with a manager account](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Gå till **Administratör** -avsnitt.

   ![](assets/login-admin.png)

1. Välj **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **Nytt** och **Ny tjänst**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Ange ett visningsnamn och välj **Google AdWords**.

   ![](assets/new-service-google.png)

1. Välj **Auktorisera Marketo**.

   >[!NOTE]
   >
   >Se till att logga ut från ditt personliga Gmail-konto och aktivera popup-fönster.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Välj det konto som är kopplat till Google AdWords.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Välj **Acceptera**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Status visas som **Lyckades**. Välj **Nästa**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Ladda upp offlinekonverteringar från Marketo till Google AdWords **Vecka** eller **Dagligen**.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Attributkonvertering till **Första klickningen** eller **Sista klickningen**.

   | Typ | Definition |
   |---|---|
   | Första klickningen | Offlinekonverteringar tilldelas de första AdWords och den person som klickat de senaste 90 dagarna |
   | Sista klickningen | Offlinekonverteringar tilldelas de sista AdWords och som en person klickade på |

   >[!NOTE]
   >
   >En konsekvent attribueringsmodell i Marketo och AdWords ger den mest korrekta informationen.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Klicka **Skapa**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en) måste väljas för att den här funktionen ska fungera. Inaktiveringen måste göras i AdWords.

Bra! Se den relaterade artikeln nedan för att lära dig hur du mappar AdWords-offlinekonverteringar i din intäktsmodell.

>[!MORELIKETHIS]
>
>[Ange Google AdWords-konverteringar i intäktsmodellen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
