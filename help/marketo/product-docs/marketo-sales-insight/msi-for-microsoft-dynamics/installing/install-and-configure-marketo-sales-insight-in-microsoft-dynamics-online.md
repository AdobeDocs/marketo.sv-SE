---
unique-page-id: 37355602
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Installera och konfigurera [!DNL Marketo Sales Insight] i [!DNL Microsoft Dynamics Online] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

[!DNL Marketo Sales Insight] är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till den stora mängd data som marknadsföringsteamet har. Så här installerar och konfigurerar du den i [!DNL Microsoft Dynamics Online].

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av [!DNL Microsoft Dynamics CRM].

## Importera lösning {#import-solution}

>[!NOTE]
>
>Om du använder det enhetliga gränssnittet, innan steg 1 nedan, klickar du på inställningsikonen i det övre högra hörnet och väljer **[!UICONTROL Advanced Settings]**.

1. Klicka **[!UICONTROL Settings]** under Microsoft Dynamics CRM.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Klicka på **[!UICONTROL Customizations]** under Inställningar.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Klicka på **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Du bör redan ha installerat och konfigurerat Marketo-lösningen innan du går vidare.

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Klicka på **[!UICONTROL Browse]** i det nya fönstret.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Hitta och installera den lösning du just laddat ned på datorn.

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/seven.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Se till att du inte markerar rutan och klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Hämta loggfilen kostnadsfritt och klicka sedan på **[!UICONTROL Close]**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/eleven.png)

1. Klicka på **[!UICONTROL Publish Customization]**.

   >[!NOTE]
   >
   >Aktivera den globala synkroniseringen [!DNL MS Dynamics].

## Anslut Marketo och [!DNL Sales Insight] {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till [!DNL Sales Insight] i [!DNL Dynamics]. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in i Marketo och gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Klicka på [!UICONTROL Sales Insight] under avsnittet **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Kopiera **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** och **[!UICONTROL API User Id]** för användning i ett senare steg. Ange en API-hemlig nyckel som du väljer och klicka på **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för att _både Lead och Contact_ ska fungera: [!DNL Sales Insight]
   >
   >* Prioritet
   >* Akut
   >* Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. Gå tillbaka om [!DNL Microsoft Dynamics], gå till **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Klicka på **[!UICONTROL Settings]** under **[!UICONTROL Marketo API Config]**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Klicka på **[!UICONTROL New]**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Ange informationen som du tog från Marketo tidigare och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Aktivera synkronisering {#enable-sync}

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/enable-one.png)

1. Välj **[!UICONTROL Microsoft Dynamics]** under Integrering.

   ![](assets/enable-two.png)

1. Klicka på **[!UICONTROL Enable Sync]**.

   ![](assets/enable-three.png)

1. Klicka på **[!UICONTROL Edit]** bredvid [!UICONTROL Field Sync Details].

   ![](assets/enable-four.png)

1. Detta _markerar automatiskt_ MSI-fält som tidigare har inaktiverats ([!UICONTROL Urgency], [!UICONTROL Relative Score] och [!UICONTROL Priority]). Klicka bara på **[!UICONTROL Save]** för att börja synkronisera data.

   ![](assets/enable-five.png)

## Ange användaråtkomst {#set-user-access}

Slutligen måste du ge specifika användare åtkomst till [!DNL Marketo Sales Insight].

1. Gå till **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Gå till **[!UICONTROL Security]**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Markera de användare som du vill ge åtkomst till [!DNL Sales Insight] och klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Välj rollen [!DNL Marketo Sales Insight] och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Och du borde vara klar! Om du vill testa loggar du in på [!DNL Dynamics] som en användare som har åtkomst till [!DNL Marketo Sales Insight] och tittar på ett lead eller en kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
