---
unique-page-id: 7504893
description: Lägg till Google AdWords som en startpunktstjänst med ett hanterarkonto - Marketo Docs - produktdokumentation
title: Lägg till Google AdWords som en startpunktstjänst med ett hanterarkonto
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Lägg till Google AdWords som en startpunktstjänst med ett hanterarkonto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Länka ditt Google AdWords-konto till Marketo för att automatiskt överföra offlinekonverteringsdata från Marketo till Google AdWords. Sedan kan ni utifrån AdWords-gränssnittet enkelt se vilka klick som resulterat i kvalificerade leads, möjligheter och nya kunder (eller vilka intäktssteg ni vill spåra) efter er  [lägga till egna kolumner](https://support.google.com/adwords/answer/3073556){target="_blank"} i AdWords. Den här informationen visas inte i användargränssnittet för Marketo.

Om du har flera Google Adwords-konton kan du använda en [Google AdWords Manager-konto](https://www.google.com/adwords/manager-accounts/){target="_blank"} (tidigare kallat My Client Center) för att integrera dem med Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera en [fristående Google AdWords-konto som startpunktstjänst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Gå till **Administratör** -avsnitt.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Välj **LaunchPoint**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Klicka på **Nytt** nedrullningsbar meny och välj **Ny tjänst**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Ange ett visningsnamn och välj **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Välj **Auktorisera Marketo**.

   >[!NOTE]
   >
   >Se till att logga ut från ditt personliga Gmail-konto och aktivera popup-fönster.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Välj det konto som är kopplat till **Google AdWords**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Klicka **Acceptera**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Status visas som **Lyckades**. Välj **Nästa**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Ladda upp offlinekonverteringar från Marketo till Google AdWords **Vecka** eller **Dagligen**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Attributkonvertering till **Första klickningen** eller **Sista klickningen**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Typ | Definition |
   |---|---|
   | Första klickningen | Offlinekonverteringar tilldelas de första AdWords och den person som klickat de senaste 90 dagarna |
   | Sista klickningen | Offlinekonverteringar tilldelas de sista AdWords och som en person klickade på |

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} måste väljas för att den här funktionen ska fungera. Den måste aktiveras inuti AdWords.

1. Klicka **Nästa**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Avmarkera konton som du inte vill uppdatera. Klicka **Skapa**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Se nu den relaterade artikeln nedan för hur du mappar AdWords-offlinekonverteringar i din intäktsmodell.

   >[!MORELIKETHIS]
   >
   >[Ange Google AdWords-konverteringar i intäktsmodellen med ett Manager-konto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
