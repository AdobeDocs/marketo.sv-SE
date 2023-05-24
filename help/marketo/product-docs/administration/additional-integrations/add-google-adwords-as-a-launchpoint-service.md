---
unique-page-id: 6095008
description: '"Lägg till [!DNL Google AdWords] som [!DNL LaunchPoint] Service - Marketo Docs - produktdokumentation'
title: "Lägg till [!DNL Google AdWords] som [!DNL LaunchPoint] Tjänst"
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: eb20d804a06bd02b61368e34ad1965a873d2fdf5
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Lägg till [!DNL Google AdWords] som [!DNL LaunchPoint] Tjänst {#add-google-adwords-as-a-launchpoint-service}

Länka [!DNL Google AdWords] till Marketo för att automatiskt överföra konverteringsdata offline från Marketo till [!DNL Google AdWords]. Sedan, från [!DNL AdWords] Gränssnittet gör att du enkelt kan se vilka klick som resulterat i kvalificerade leads, möjligheter och nya kunder (eller vilka intäktssteg du vill spåra) efter att du [lägga till egna kolumner](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Den här informationen visas inte i användargränssnittet för Marketo.

Läs mer om [Google importfunktion för offlinekonvertering](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>Du kan även integrera en [[!DNL Google AdWords] as a [!DNL Launchpoint] tjänst med ett chefskonto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Välj **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Välj **[!UICONTROL New]** och **[!UICONTROL New Service]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Ange [!UICONTROL display name] och markera **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Välj **[!UICONTROL Authorize Marketo]**.

   >[!NOTE]
   >
   >Se till att logga ut från din personliga [!DNL Gmail] och aktivera popup-fönster.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Välj det konto som är kopplat till [!DNL Google AdWords].

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Välj **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. Status visas som **[!UICONTROL Success]**. Välj **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Ladda upp offlinekonverteringar från Marketo till [!DNL Google AdWords] **[!UICONTROL Weekly]** eller **[!UICONTROL Daily]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Attributkonvertering till **[!UICONTROL First Click]** eller **[!UICONTROL Last Click]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL First Click] | Offlinekonverteringar tilldelas den första [!DNL AdWords] och att en person har klickat de senaste 90 dagarna |
   | [!UICONTROL Last Click] | Offlinekonverteringar tilldelas den sista [!DNL AdWords] och att en person klickade |

   >[!NOTE]
   >
   >Använda en konsekvent attribueringsmodell i Marketo och [!DNL AdWords] ger de mest korrekta data.

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Automatisk taggning](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} måste väljas för att den här funktionen ska fungera. Inaktiveringen måste göras inifrån [!DNL AdWords].

Bra! Se den relaterade artikeln nedan för att lära dig hur du mappar [!DNL AdWords] offlinekonverteringar i intäktsmodellen.

>[!MORELIKETHIS]
>
>[Ange [!DNL Google AdWords] Konverteringar i intäktsmodellen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
