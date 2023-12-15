---
unique-page-id: 12980661
description: Lägg till Google kundmatchning som en LaunchPoint-tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Google kundmatchning som en LaunchPoint-tjänst
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Lägg till Google kundmatchning som en LaunchPoint-tjänst {#add-google-customer-match-as-a-launchpoint-service}

Med den här integreringen kan ni skicka en Marketo Engage-målgrupp till Google för målgruppsanpassning med hjälp av Google AdWords, samt målinrikta om målgrupper i YouTube, Search och Gmail.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Klicka på **[!UICONTROL LaunchPoint]**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **[!UICONTROL New]** sedan **[!UICONTROL New Service]**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Ange en **[!UICONTROL Display Name]** och markera **[!UICONTROL Google Customer Match]** från **[!UICONTROL Service]** nedrullningsbar meny. Klicka på **[!UICONTROL Create]**.

   ![](assets/chooseservice.png)

1. Om du vill ansluta ett Google AdWords-konto klickar du på **[!UICONTROL Authorize]**.

   ![](assets/authorizeaccount-1.png)

1. Google öppnas på en ny flik. Logga in på ditt Google AdWords-konto härifrån.

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera AdWords-konton måste den Google-användare som du godkänner i följande steg ha tillgång till _alla_ av dessa konton.

   ![](assets/chooseaccount.png)

1. Granska begärda behörigheter och klicka sedan på **[!UICONTROL Allow]**.

   ![](assets/reviewpermissions.png)

1. Ditt Google AdWords-konto är nu anslutet till Marketo. Klicka på **[!UICONTROL Create]**.

   ![](assets/authorizesuccess.png)

   Häftig! Nu visas Google Matched Audiences som en LaunchPoint-tjänst på fliken Installerade tjänster.

>[!NOTE]
>
>Integreringen av Google kundmatchning kan endast användas för ett chefskonto och alla underkonton i det chefskontot. Flera hanterarkonton stöds inte.
