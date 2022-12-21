---
unique-page-id: 4720257
description: Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst - Marketo Docs - produktdokumentation
title: Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Med den här integreringen kan ni skicka målgruppsdata från Marketo statiska och smarta listor till Facebook som kan användas som anpassade målgrupper i Facebook Ad Campaigns. Så här ställer du in det.

1. Gå till Marketo **Administratör**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Nytt** och markera **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange **Visningsnamn** för tjänsten och väljer **Facebook Custom Auditions** från **Tjänst** nedrullningsbar meny.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öppna en ny flik i samma webbläsare och gå till [facebook.com](https://www.facebook.com/). Logga in på Facebook med det konto du vill använda för integreringen.

   >[!CAUTION]
   >
   >För att Marketo ska kunna skicka målgrupper över flera annonshanterarkonton måste den Facebook-användare som du auktoriserar i följande steg ha tillgång till *alla* av dessa konton.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo. Klicka **Auktorisera**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Du _måste_ använda ett Facebook Business Manager-konto för att er anpassade målgruppsintegrering ska fungera. Mer information om hur du skapar ett Business Manager-konto finns i [Hjälp om facebook](https://www.facebook.com/business/help/1710077379203657).

1. Om du uppmanas till det klickar du på **OK** för att acceptera Marketo-appinstallationen i Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du är nu auktoriserad! Välj ett matchande läge och klicka på **Skapa**.

   >[!NOTE]
   >
   >**Grundläggande matchning** använder endast e-postadresser. **Avancerad matchning** använder ytterligare sju fält, vilket ökar matchningsfrekvensen, för mer konvertering. Om ditt företags sekretesspolicy inte tillåter delning av ytterligare fält, eller om dina data inte inkluderar dem, väljer du Grundläggande matchning.

   ![](assets/fb-custom-adv-matching-hands.png)

   Bra jobbat! Nu kan du gå till vilken statisk eller smart lista som helst i Marketo och skicka målgruppsdata till Facebook.

   >[!CAUTION]
   >
   >Innan du går, var noga med att [Acceptera Facebook anpassade målgruppsvillkor](https://www.facebook.com/ads/manage/customaudiences/tos.php) på ditt Facebook-konto! Om du inte gör det kommer målgruppsuppdateringarna att misslyckas.

>[!MORELIKETHIS]
>
>* [Skapa en anpassad målgrupp i Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Konfigurera Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

