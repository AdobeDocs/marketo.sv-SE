---
unique-page-id: 6095008
description: Lägg till Google AdWords som en LaunchPoint-tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Google AdWords som en LaunchPoint-tjänst
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: 457b4aadac47b0a8614c3e6025d2e1ae287b5ecc
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Lägg till Google AdWords som en LaunchPoint-tjänst {#add-google-adwords-as-a-launchpoint-service}

Länka ditt Google AdWords-konto till Marketo för att automatiskt överföra offlinekonverteringsdata från Marketo till Google AdWords. Sedan kan ni utifrån AdWords-gränssnittet enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg ni vill spåra) efter att ni gjort det [lägga till egna kolumner](https://support.google.com/adwords/answer/3073556){target=&quot;_blank&quot;} i AdWords. Den här informationen visas inte i användargränssnittet för Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en){target=&quot;_blank&quot;}.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din Customer Success Manager för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera en [Google AdWords as a Launchpoint service with a manager account](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target=&quot;_blank&quot;}.

1. Gå till **Administratör** -avsnitt.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Välj **LaunchPoint**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Välj **Nytt** och **Ny tjänst**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Ange ett visningsnamn och välj **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Välj **Auktorisera Marketo**.

   >[!NOTE]
   >
   >Se till att logga ut från ditt personliga Gmail-konto och aktivera popup-fönster.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Välj det konto som är kopplat till Google AdWords.

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Välj **Acceptera**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. Status visas som **Lyckades**. Välj **Nästa**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Ladda upp offlinekonverteringar från Marketo till Google AdWords **Vecka** eller **Dagligen**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Attributkonvertering till **Första klickningen** eller **Sista klickningen**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Typ | Definition |
   |---|---|
   | Första klickningen | Offlinekonverteringar tilldelas de första AdWords och den person som klickat de senaste 90 dagarna |
   | Sista klickningen | Offlinekonverteringar tilldelas de sista AdWords och som en person klickade på |

   >[!NOTE]
   >
   >En konsekvent attribueringsmodell i Marketo och AdWords ger den mest korrekta informationen.

1. Klicka **Skapa**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en){target=&quot;_blank&quot;} måste väljas för att den här funktionen ska fungera. Inaktiveringen måste göras i AdWords.

Bra! Se den relaterade artikeln nedan för att lära dig hur du mappar AdWords-offlinekonverteringar i din intäktsmodell.

>[!MORELIKETHIS]
>
>[Ange Google AdWords-konverteringar i intäktsmodellen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target=&quot;_blank&quot;}
