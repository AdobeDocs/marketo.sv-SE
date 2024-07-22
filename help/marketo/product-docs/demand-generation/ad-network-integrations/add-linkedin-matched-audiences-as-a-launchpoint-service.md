---
unique-page-id: 7504163
description: Lägg till LinkedIn Matched Audiences som en LaunchPoint-tjänst - Marketo Docs - produktdokumentation
title: Lägg till LinkedIn Matched Audiences som en LaunchPoint-tjänst
exl-id: 82096b19-aae9-4086-8fb4-defc5481d382
feature: Integrations
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Lägg till LinkedIn Matched Audiences som en LaunchPoint-tjänst {#add-linkedin-matched-audiences-as-a-launchpoint-service}

>[!IMPORTANT]
>
>LinkedIn uppgraderar sina Marketing API:er som används av integreringar med Marketo Engage LinkedIn. Dessa ändringar kräver omautentisering av alla LinkedIn LaunchPoint-tjänster på **Admin** > **LaunchPoint** -menyn mellan 7 juni och 15 december 2024 för att undvika avbrott i tjänsten. Mer information finns i [Vanliga frågor om migrering](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Koppla ditt Marketo Engage-konto till LinkedIn Matched Audiences för att använda en statisk lista från Marketo eller Smart List som ett LinkedIn-målgruppssegment.

1. Gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Välj **[!UICONTROL LaunchPoint]**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Välj **[!UICONTROL New]** och **[!UICONTROL New Service]**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Ange en **[!UICONTROL Display Name]** och välj **[!UICONTROL LinkedIn Matched Audiences]**. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2018-2-23-14-3a25-3a39.png)

1. Klicka på **[!UICONTROL Authorize]** om du vill ansluta ett LinkedIn-konto.

   ![](assets/authorizeaccount.png)

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera LinkedIn annonskonton måste den LinkedIn-användare som du auktoriserar i följande steg ha tillgång till *alla* av dessa annonskonton i sin Campaign Manager.

1. LinkedIn öppnas på en ny flik. Logga in på ditt LinkedIn-konto härifrån.

   ![](assets/image2018-2-23-14-3a32-3a20.png)

1. Granska begärda behörigheter och klicka sedan på **[!UICONTROL Allow]**.

   ![](assets/li-permissions.png)

1. Ditt LinkedIn-konto är nu anslutet till Marketo. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2018-2-23-14-3a35-3a55.png)

   Häftig! Nu visas LinkedIn Matched Audiences som en LaunchPoint-tjänst på fliken Installerade tjänster.

   ![](assets/bartholomew2.png)

>[!MORELIKETHIS]
>
>[Använd en Marketo-lista eller smart lista som ett målgruppssegment i LinkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/use-a-marketo-list-or-smart-list-as-a-linkedin-audience-segment.md){target="_blank"}
