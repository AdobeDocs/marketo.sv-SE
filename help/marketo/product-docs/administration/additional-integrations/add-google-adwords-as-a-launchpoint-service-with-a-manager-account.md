---
unique-page-id: 7504893
description: "Lägg till [!DNL Google AdWords] som [!DNL Launchpoint] Service med ett Manager-konto - Marketo Docs - produktdokumentation"
title: "Lägg till [!DNL Google AdWords] som [!DNL Launchpoint] Service med ett hanterarkonto"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: eb20d804a06bd02b61368e34ad1965a873d2fdf5
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 1%

---

# Lägg till [!DNL Google AdWords] som [!DNL Launchpoint] Tjänst med ett chefskonto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Länka [!DNL Google AdWords] till Marketo för att automatiskt överföra konverteringsdata offline från Marketo till [!DNL Google AdWords]. Sedan, från [!DNL AdWords] Gränssnittet gör att du enkelt kan se vilka klick som resulterat i kvalificerade leads, affärsmöjligheter och nya kunder (eller vilka intäktssteg du vill spåra) efter att du  [lägga till egna kolumner](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Den här informationen visas inte i användargränssnittet för Marketo.

Om du har flera [!DNL Google Adwords] konton kan du använda [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (tidigare känt som [!DNL My Client Center]) för att integrera dem med Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera en [fristående [!DNL Google AdWords] konto som [!DNL Launchpoint] service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Välj **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Klicka på **[!UICONTROL New]** nedrullningsbar meny och välj **[!UICONTROL New Service]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Ange **[!UICONTROL Display Name]** och markera **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Välj **[!UICONTROL Authorize Marketo]**.

   >[!NOTE]
   >
   >Se till att logga ut från din personliga [!DNL Gmail] och aktivera popup-fönster.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Välj det konto som är kopplat till **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Klicka på **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Status visas som **[!UICONTROL Success]**. Välj **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Ladda upp offlinekonverteringar från Marketo till [!DNL Google AdWords] **[!UICONTROL Weekly]** eller **[!UICONTROL Daily]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Attributkonvertering till **[!UICONTROL First Click]** eller **[!UICONTROL Last Click]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL First Click] | Offlinekonverteringar tilldelas den första [!DNL AdWords] och att en person har klickat de senaste 90 dagarna |
   | [!UICONTROL Last Click] | Offlinekonverteringar tilldelas den sista [!DNL AdWords] och att en person klickade |

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} måste väljas för att den här funktionen ska fungera. Den måste aktiveras inuti [!DNL AdWords].

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Avmarkera konton som du inte vill uppdatera. Klicka på **[!UICONTROL Create]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Se artikeln nedan för mer information om hur du mappar [!DNL AdWords] offlinekonverteringar i intäktsmodellen.

   >[!MORELIKETHIS]
   >
   >[Ange [!DNL Google AdWords] Konverteringar i intäktsmodellen med ett chefskonto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
