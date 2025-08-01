---
unique-page-id: 27656223
description: Installera [!DNL Salesforce] Anpassning för Professional Edition-kunder - Marketo Docs - Produktdokumentation
title: Installera [!DNL Salesforce] anpassning för Professional Edition-kunder
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Installera anpassning av [!DNL Salesforce] för Professional Edition-kunder {#install-salesforce-customization-for-professional-edition-customers}

Kunder med [!DNL Salesforce] Professional Edition måste följa dessa steg för att installera anpassning.

>[!PREREQUISITES]
>
>* [!DNL Sales Connect] Admin måste ansluta sina [!DNL Salesforce]- och [!DNL Sales Connect]-konton.
>* [!DNL Salesforce]-instansen som används måste ha utrymme för att installera tretton anpassade aktivitetsfält.

## Installation {#installation}

1. I [!DNL Sales Connect] klickar du på kugghjulsikonen i det övre högra hörnet och väljer **[!UICONTROL Settings]**.

   ![](assets/one-4.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL Salesforce]**.

   ![](assets/two-4.png)

1. Kontrollera att du är ansluten till ditt [!DNL Salesforce]-konto.

   >[!CAUTION]
   >
   >Om du är ansluten visas den gröna knappen [!UICONTROL Install]. **DO NOT** click this button, forts to step 4 istället.

1. Logga in på det [!DNL Salesforce]-konto som du är ansluten till och klicka sedan på [den här länken](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Du skickas till installationssidan för [!DNL Sales Connect].

   ![](assets/install-package.png)

1. Välj de användare som du vill installera anpassningar för: Endast administratör, alla användare eller specifika profiler.
1. Klicka på knappen **[!UICONTROL Install]** för att installera anpassning.
1. Logga in på ditt [!DNL Salesforce]-konto för att bekräfta att installationen lyckades.
1. Klicka på **[!UICONTROL Setup]**, sök efter Installerade paket i sökfältet och klicka på **[!UICONTROL Installed Packages]**.

   Där ser du Marketo Sales Connect Customizations.

   Om du vill konfigurera [!DNL Sales Connect] i din [!DNL Salesforce]-instans följer du stegen som börjar i avsnittet&quot;CONFIGURING THE SALES ENGAGE SALESFORCE PACKAGE&quot; på sidan 7 i installationshandboken.

   >[!NOTE]
   >
   >[!DNL Sales Engage] är det tidigare namnet för [!DNL Sales Connect].

## Användarhandböcker {#guides}

[Installationshandbok för Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Installationshandbok för Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
