---
unique-page-id: 7504893
description: "Lägg till [!DNL Google AdWords] som en [!DNL Launchpoint] tjänst med ett hanterarkonto - Marketo Docs - produktdokumentation"
title: "Lägg till [!DNL Google AdWords] som en [!DNL Launchpoint] tjänst med ett hanterarkonto"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Lägg till [!DNL Google AdWords] som en [!DNL Launchpoint]-tjänst med ett hanterarkonto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Länka ditt [!DNL Google AdWords]-konto till Marketo för att automatiskt överföra offlinekonverteringsdata från Marketo till [!DNL Google AdWords]. Sedan kan du från användargränssnittet i [!DNL AdWords] enkelt se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg du vill spåra) efter att du [lagt till anpassade kolumner](https://support.google.com/adwords/answer/3073556){target="_blank"} i [!DNL AdWords]. Den här informationen visas inte i användargränssnittet för Marketo.

Om du har flera [!DNL Google Adwords]-konton kan du använda en [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (tidigare kallad [!DNL My Client Center]) för att integrera dem med Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Alla användare i Marketo Engage har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera ett [fristående [!DNL Google AdWords] konto som en [!DNL Launchpoint] tjänst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Välj **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL New Service]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Ange en **[!UICONTROL Display Name]** och välj **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Välj **[!UICONTROL Authorize Marketo]**.

   >[!NOTE]
   >
   >Se till att logga ut från ditt personliga [!DNL Gmail]-konto och aktivera popup-fönster.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Välj det konto som är associerat med **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Klicka på **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Status visas som **[!UICONTROL Success]**. Välj **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Överför dina offlinekonverteringar från Marketo till [!DNL Google AdWords] **[!UICONTROL Weekly]** eller **[!UICONTROL Daily]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Attributkonvertering till **[!UICONTROL First Click]** eller **[!UICONTROL Last Click]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL First Click] | Offlinekonverteringar kommer att tilldelas den första [!DNL AdWords]-annonsen som en person klickat på under de senaste 90 dagarna |
   | [!UICONTROL Last Click] | Offlinekonverteringar kommer att tilldelas den senaste [!DNL AdWords]-annonsen som en person klickade på |

   >[!NOTE]
   >
   >[Autotaggning](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} måste vara markerad för att den här funktionen ska fungera. Den måste aktiveras inuti [!DNL AdWords].

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Avmarkera konton som du inte vill uppdatera. Klicka på **[!UICONTROL Create]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Se nu den relaterade artikeln nedan för hur du mappar [!DNL AdWords] offlinekonverteringar i din intäktsmodell.

   >[!MORELIKETHIS]
   >
   >[Ange [!DNL Google AdWords] konverteringar i intäktsmodellen med ett hanterarkonto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
