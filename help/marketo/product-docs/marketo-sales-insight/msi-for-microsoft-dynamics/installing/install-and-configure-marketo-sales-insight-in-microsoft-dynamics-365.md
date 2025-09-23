---
unique-page-id: 3571739
description: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365 - Marketo Docs - produktdokumentation
title: Installera och konfigurera Marketo Sales Insight i Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 2%

---

# Installera och konfigurera [!DNL Marketo Sales Insight] i [!DNL Microsoft Dynamics 365] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] är ett fantastiskt verktyg för att ge säljteamet ett&quot;fönster&quot; till den stora mängd data som marknadsföringsteamet har. Så här installerar och konfigurerar du.

>[!PREREQUISITES]
>
>Komplettera integreringen mellan Marketo och Microsoft.
>
>[Hämta rätt lösning](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) för din version av [!DNL Microsoft Dynamics CRM].

## Importera lösning {#import-solution}

1. Logga in på [[!DNL Microsoft Office 365]](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Klicka på menyn ![—](assets/image2015-3-16-16-1-13.png) och välj **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Klicka på menyn ![—](assets/image2015-5-13-10-5-8.png). I listrutan väljer du **[!DNL Settings]** och sedan **[!DNL Solutions]**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Du bör redan ha [installerat och konfigurerat Marketo-lösningen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) innan du går vidare.

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Klicka på **[!UICONTROL Browse]** i det nya fönstret. Välj den [Marketo Sales Insight-lösning som du hämtade i steg 1](#msi). Klicka på **[!UICONTROL Next]**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. Lösningen kommer att överföras. Du kan visa paketets innehåll om du vill. Klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Lämna rutan **[!UICONTROL checked]** och klicka på **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Hämta loggfilen kostnadsfritt. Klicka på **[!UICONTROL Close]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Häftig! Du borde se lösningen nu. Uppdatera skärmen om den inte finns där.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Klicka på **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Anslut Marketo och [!DNL Sales Insight] {#connect-marketo-and-sales-insight}

Låt oss binda din Marketo-instans till [!DNL Sales Insight] i [!DNL Dynamics]. Så här:

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Logga in på Marketo och gå till avsnittet **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Klicka på **[!UICONTROL Sales Insight]** Redigera API-konfiguration **under avsnittet**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Kopiera **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** och **[!UICONTROL API User Id]** för användning i ett senare steg. Ange en **[!UICONTROL API Secret Key]** och klicka på **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Använd inte ett et-tecken (&amp;) i API-hemlig nyckel.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Följande fält måste synkroniseras med Marketo för att _både Lead och Contact_ ska fungera: [!DNL Sales Insight]
   >
   > * Prioritet
   > * Akut
   > * Relativa poäng
   >
   >Om något av dessa fält saknas visas ett felmeddelande i Marketo med namnet på de saknade fälten. Utför [den här proceduren](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md) om du vill åtgärda det.

1. Gå tillbaka i [!DNL Microsoft Dynamics], klicka på ikonen ![](assets/image2015-5-13-15-3a49-3a19.png) intill [!UICONTROL Settings] och välj sedan **[!UICONTROL Marketo API Config]** i listrutan.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Klicka på **[!UICONTROL Default Configuration]**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Ange den information som du kopierade från Marketo tidigare.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Klicka på ikonen ![](assets/image2015-5-13-16-3a8-3a51.png) längst ned till höger för att spara ändringarna.

## Ange användaråtkomst {#set-user-access}

Du måste ge användarna behörighet att använda [!DNL Sales Insight].

1. Klicka på menyn ![](assets/image2015-5-13-10-3a5-3a8.png). I listrutan väljer du **[!UICONTROL Settings]** och sedan **[!UICONTROL Security]**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Klicka på **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Markera de användare som du vill ge åtkomst till [!DNL Sales Insight] och klicka på **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Välj rollen **[!UICONTROL Marketo Sales Insight]** och klicka på **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Och du borde vara klar! Om du vill testa loggar du in på [!DNL Dynamics] som en användare som har åtkomst till [!DNL Marketo Sales Insight] och tittar på ett lead eller en kontakt.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Du har nu låst upp kraften hos [!DNL Marketo Sales Insight] för ditt säljteam.

>[!MORELIKETHIS]
>
>[Konfigurera stjärnor och flamma för lead-/kontaktposter](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
