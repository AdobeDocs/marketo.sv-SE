---
unique-page-id: 12980661
description: Lägg till Google kundmatchning som en [!DNL LaunchPoint] tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Google kundmatchning som en [!DNL LaunchPoint] tjänst
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 1%

---

# Lägg till Google kundmatchning som en [!DNL LaunchPoint]-tjänst {#add-google-customer-match-as-a-launchpoint-service}

Med den här integreringen kan du skicka en Marketo-målgrupp till Google för målgruppsanpassning med hjälp av [!DNL Google AdWords], samt målinrikta målgrupper på nytt i YouTube, Search och [!DNL Gmail].

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicka på **[!UICONTROL LaunchPoint]**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **[!UICONTROL New]** och sedan **[!UICONTROL New Service]**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Ange en **[!UICONTROL Display Name]** och välj **[!UICONTROL Google Customer Match]** i listrutan **[!UICONTROL Service]**. Klicka på **[!UICONTROL Create]**.

   ![](assets/chooseservice.png)

1. Om du vill ansluta ett [!DNL Google AdWords]-konto klickar du på **[!UICONTROL Authorize]**.

   ![](assets/authorizeaccount-1.png)

1. Google öppnas på en ny flik. Logga in på ditt [!DNL Google AdWords]-konto härifrån.

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera [!DNL AdWords]-konton måste den Google-användare som du auktoriserar i följande steg ha tillgång till _alla_ av dessa konton.

   ![](assets/chooseaccount.png)

1. Granska begärda behörigheter och klicka sedan på **[!UICONTROL Allow]**.

   ![](assets/reviewpermissions.png)

1. Ditt [!DNL Google AdWords]-konto är nu anslutet till Marketo. Klicka på **[!UICONTROL Create]**.

   ![](assets/authorizesuccess.png)

   Häftig! Nu visas Google Matched Audiences som en [!DNL LaunchPoint]-tjänst på fliken Installerade tjänster.

>[!NOTE]
>
>Integreringen av Google kundmatchning kan endast användas för ett chefskonto och alla underkonton i det chefskontot. Flera hanterarkonton stöds inte.
