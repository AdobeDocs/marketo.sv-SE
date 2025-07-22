---
unique-page-id: 7513865
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2015 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 2015
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

# Installera och konfigurera [!DNL Marketo Sales Insight] i [!DNL Microsoft Dynamics 2015] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till alla data som marknadsföringsteamet har. Så här installerar och konfigurerar du den i [!DNL Microsoft Dynamics 2015]

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av [!DNL Microsoft Dynamics CRM].

## Importera lösning {#import-solution}

OK, nu är det dags att importera lösningen [!DNL Marketo Sales Insight] till [!DNL Microsoft Dynamics]. Så här:

1. Klicka på [!UICONTROL Microsoft Dynamics CRM] under **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Klicka på [!UICONTROL SETTINGS] under **[!UICONTROL Customizations]**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Klicka på **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Du bör redan ha installerat och konfigurerat Marketo-lösningen innan du går vidare.

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **[!UICONTROL Browse]** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Hitta och välj den lösning du laddat ned ovan.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Se till att du inte markerar rutan och klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt och klicka sedan på **[!UICONTROL Close]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo och Sales Insight {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till [!DNL Sales Insight] i [!DNL Dynamics]. Så här:

>[!NOTE]
>
>Administratörsrättigheter krävs.

1. Logga in på Marketo och gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicka på [!UICONTROL Sales Insight] under avsnittet **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** och **[!UICONTROL API User Id]** för användning i ett senare steg. Ange en API-hemlig nyckel som du väljer och klicka på **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för att *både Lead och Contact* ska fungera: [!DNL Sales Insight]
   >
   >* Prioritet
   >* Akut
   >* Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. Gå tillbaka om [!DNL Microsoft Dynamics], gå till **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Marketo API Config]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Ange informationen som du tog från Marketo tidigare och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Ange användaråtkomst {#set-user-access}

Slutligen måste du ge specifika användare tillgång till Marketo Sales Insight.

1. Gå till **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Gå till **[!UICONTROL Security]**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Markera de användare som du vill ge åtkomst till [!DNL Sales Insight] och klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Välj rollen [!DNL Marketo Sales Insight] och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Om du vill testa loggar du in på [!DNL Dynamics] som en användare som har åtkomst till [!DNL Marketo Sales Insight] och tittar på ett lead eller en kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Du har nu låst upp kraften hos [!DNL Marketo Sales Insight] för ditt säljteam.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
