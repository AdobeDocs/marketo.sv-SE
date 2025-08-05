---
unique-page-id: 4720257
description: Lägg till [!DNL Facebook] anpassade målgrupper som en [!DNL LaunchPoint] tjänst - Marketo Docs - produktdokumentation
title: Lägg till  [!DNL Facebook] anpassade målgrupper som en [!DNL LaunchPoint] tjänst
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Lägg till [!DNL Facebook] anpassade målgrupper som en [!DNL LaunchPoint]-tjänst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Med den här integreringen kan du skicka målgruppsdata från Marketo statiska och smarta listor till [!DNL Facebook] som kan användas som anpassade målgrupper i [!DNL Facebook] annonskampanjer. Så här ställer du in det.

1. Gå till Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **[!UICONTROL LaunchPoint]**, klicka på **[!UICONTROL New]** och välj **[!UICONTROL New Service]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange en **[!UICONTROL Display Name]** för tjänsten och välj tjänsten **[!UICONTROL Facebook Custom Audiences]** i listrutan **[!UICONTROL Service]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öppna en ny flik i samma webbläsare och gå till [facebook.com](https://www.facebook.com/). Logga in på [!DNL Facebook] med det konto som du vill använda för integreringen.

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera annonshanterarkonton måste den [!DNL Facebook]-användare som du auktoriserar i följande steg ha tillgång till *alla* av dessa konton.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på [!DNL Facebook] går du tillbaka till Marketo. Klicka på **[!UICONTROL Authorize]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Du *måste* använda ett [!DNL Facebook] Business Manager-konto för att integreringen av anpassade målgrupper ska fungera. Mer information om hur du konfigurerar ett Business Manager-konto finns i [[!DNL Facebook] hjälpen](https://www.facebook.com/business/help/1710077379203657).

1. Om du uppmanas till det klickar du på **[!UICONTROL OK]** för att godkänna Marketo-programinstallationen i [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du är nu auktoriserad! Välj ett matchande läge och klicka på **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >**[!UICONTROL Basic Matching]** använder bara e-postadresser. **[!UICONTROL Advanced Matching]** använder ytterligare sju fält, vilket ökar matchningsfrekvensen, för mer konvertering. Om ditt företags sekretesspolicy inte tillåter delning av ytterligare fält, eller om dina data inte inkluderar dem, väljer du [!UICONTROL Basic Matching].

   ![](assets/fb-custom-adv-matching-hands.png)

   Snyggt jobb! Du kan nu gå till en statisk eller smart lista i Marketo och skicka målgruppsdata till [!DNL Facebook].

   >[!CAUTION]
   >
   >Innan du går ska du se till att [acceptera  [!DNL Facebook]s anpassade målgruppsvillkor](https://www.facebook.com/ads/manage/customaudiences/tos.php) i ditt [!DNL Facebook]-konto! Om du inte gör det kommer målgruppsuppdateringarna att misslyckas.

>[!MORELIKETHIS]
>
>* [Skapa en anpassad målgrupp i [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Konfigurera [!DNL Facebook] Leadannonser](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
