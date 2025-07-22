---
unique-page-id: 7504163
description: Lägg till [!DNL LinkedIn] matchade målgrupper som en [!DNL LaunchPoint] tjänst - Marketo Docs - produktdokumentation
title: Lägg till [!DNL LinkedIn] matchade målgrupper som en [!DNL LaunchPoint] tjänst
exl-id: 82096b19-aae9-4086-8fb4-defc5481d382
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Lägg till [!DNL LinkedIn] matchade målgrupper som en [!DNL LaunchPoint]-tjänst {#add-linkedin-matched-audiences-as-a-launchpoint-service}

>[!IMPORTANT]
>
>LinkedIn uppgraderar sina Marketing API:er som används av Marketo Engage LinkedIn-integreringar. Dessa ändringar kräver omautentisering av alla LinkedIn LaunchPoint-tjänster i **Admin** > **LaunchPoint** -menyn mellan 7 juni och 15 december 2024 för att undvika avbrott i tjänsten. Mer information finns i [Vanliga frågor om migrering](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Anslut ditt Marketo-konto till [!DNL LinkedIn] matchade målgrupper om du vill använda en statisk lista eller smart lista från Marketo som ett [!DNL LinkedIn] målgruppssegment.

1. Gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Välj **[!UICONTROL LaunchPoint]**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **[!UICONTROL New]** och **[!UICONTROL New Service]**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Ange en **[!UICONTROL Display Name]** och välj **[!UICONTROL LinkedIn Matched Audiences]**. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2018-2-23-14-3a25-3a39.png)

1. Om du vill ansluta ett [!DNL LinkedIn]-konto klickar du på **[!UICONTROL Authorize]**.

   ![](assets/authorizeaccount.png)

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera [!DNL LinkedIn] annonskonton måste den [!DNL LinkedIn]-användare som du auktoriserar i följande steg ha tillgång till *alla* annonskonton i sin Campaign Manager.

1. [!DNL LinkedIn] öppnas på en ny flik. Logga in på ditt [!DNL LinkedIn]-konto härifrån.

   ![](assets/image2018-2-23-14-3a32-3a20.png)

1. Granska begärda behörigheter och klicka sedan på **[!UICONTROL Allow]**.

   ![](assets/li-permissions.png)

1. Ditt [!DNL LinkedIn]-konto är nu anslutet till Marketo. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2018-2-23-14-3a35-3a55.png)

   Häftig! [!DNL LinkedIn] matchade målgrupper visas nu som en [!DNL LaunchPoint]-tjänst på fliken Installerade tjänster.

   ![](assets/bartholomew2.png)

>[!MORELIKETHIS]
>
>[Använd en Marketo-lista eller smart lista som  [!DNL LinkedIn] målgruppssegment](/help/marketo/product-docs/demand-generation/social/social-functions/use-a-marketo-list-or-smart-list-as-a-linkedin-audience-segment.md)
