---
unique-page-id: 27656223
description: Installera Salesforce-anpassning för Professional Edition-kunder - Marketo Docs - produktdokumentation
title: Installera Salesforce-anpassning för Professional Edition-kunder
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Installera Salesforce-anpassning för Professional Edition-kunder {#install-salesforce-customization-for-professional-edition-customers}

Kunder som har Salesforce Professional Edition måste följa dessa steg för att installera anpassningar.

>[!PREREQUISITES]
>
>* Sales Connect Admin måste ansluta sina Salesforce- och Sales Connect-konton.
>* Den Salesforce-instans som används måste ha utrymme för att installera tretton anpassade aktivitetsfält.

## Installation {#installation}

1. I Sales Connect klickar du på kugghjulsikonen i det övre högra hörnet och väljer **Settings**.

   ![](assets/one-4.png)

1. Klicka på **Salesforce** under Administratörsinställningar.

   ![](assets/two-4.png)

1. Kontrollera att du är ansluten till ditt Salesforce-konto.

   >[!CAUTION]
   >
   >Om du är ansluten visas en grön Install-knapp. **DO NOT** click this button, forts to step 4 istället.

1. Logga in på Salesforce-kontot som du är ansluten till och klicka sedan på [den här länken](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Du kommer att skickas till installationssidan för Sales Connect.

   ![](assets/install-package.png)

1. Välj de användare som du vill installera anpassningar för: Endast administratör, alla användare eller specifika profiler.
1. Klicka på knappen **Installera** för att installera anpassning.
1. Logga in på ditt Salesforce-konto för att bekräfta att installationen lyckades.
1. Klicka på **Konfigurera**, sök efter&quot;Installerade paket&quot; i sökfältet och klicka på **Installerade paket**.

   Där ser du Marketo Sales Connect Customizations.

   Om du vill konfigurera Sales Connect i Salesforce-instansen följer du stegen som börjar i avsnittet&quot;CONFIGURING THE SALES ENGAGE SALESFORCE PACKAGE&quot; på sidan 7 i installationshandboken.

   >[!NOTE]
   >
   >Försäljningsengagemanget är det tidigare namnet för Sales Connect.

## Stödlinjer {#guides}

[Installationshandbok för Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Installationshandbok för Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
