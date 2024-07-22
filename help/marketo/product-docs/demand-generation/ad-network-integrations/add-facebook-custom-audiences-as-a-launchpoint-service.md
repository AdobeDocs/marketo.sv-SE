---
unique-page-id: 4720257
description: Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst - Marketo Docs - produktdokumentation
title: Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Med den här integreringen kan ni skicka målgruppsdata från statiska och smarta listor från Marketo Engage till Facebook och använda dem som anpassade målgrupper i Facebook annonskampanjer. Så här ställer du in det.

1. Gå till Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **[!UICONTROL LaunchPoint]**, klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Service]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange en **[!UICONTROL Display Name]** för tjänsten och välj tjänsten **[!UICONTROL Facebook Custom Audiences]** i listrutan **[!UICONTROL Service]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öppna en ny flik i samma webbläsare och gå till [facebook.com](https://www.facebook.com/){target="_blank"}. Logga in på Facebook med det konto du vill använda för integreringen.

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera annonshanterarkonton måste den Facebook-användare som du auktoriserar i följande steg ha tillgång till *alla* av dessa konton.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo. Klicka på **[!UICONTROL Authorize]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Du _måste_ använda ett Facebook Business Manager-konto för att din anpassade målgruppsintegrering ska fungera. Mer information om hur du konfigurerar ett Business Manager-konto finns i [Facebook-hjälpen](https://www.facebook.com/business/help/1710077379203657){target="_blank"}.

1. Om du uppmanas till det klickar du på **[!UICONTROL OK]** för att godkänna Marketo-appinstallationen i Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du är nu auktoriserad! Välj ett matchande läge och klicka på **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >**Grundläggande matchning** använder endast e-postadresser. **Avancerad matchning** använder ytterligare sju fält, vilket ökar matchningsfrekvensen, för mer konvertering. Om ditt företags sekretesspolicy inte tillåter delning av ytterligare fält, eller om dina data inte inkluderar dem, väljer du Grundläggande matchning.

   ![](assets/fb-custom-adv-matching-hands.png)

   Snyggt jobb! Nu kan du gå över till en statisk lista eller Smart List i Marketo och skicka målgruppsdata till Facebook.

   >[!CAUTION]
   >
   >Innan du går ska du [Acceptera Facebook anpassade målgruppsvillkor](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} i ditt Facebook-konto! Om du inte gör det kommer målgruppsuppdateringarna att misslyckas.

>[!MORELIKETHIS]
>
>* [Skapa en anpassad målgrupp i Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [Konfigurera Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
