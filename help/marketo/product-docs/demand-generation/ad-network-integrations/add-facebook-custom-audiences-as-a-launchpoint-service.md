---
unique-page-id: 4720257
description: Lägg till anpassade målgrupper på Facebook som en LaunchPoint-tjänst - Marketo Docs - produktdokumentation
title: Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Lägg till anpassade Facebook-målgrupper som en LaunchPoint-tjänst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Med den här integreringen kan ni skicka målgruppsdata från Marketo till statiska och smarta listor till Facebook och använda dem som anpassade målgrupper i Facebook-annonskampanjer. Så här ställer du in det.

1. Gå till Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gå till **LaunchPoint**, klicka på **Ny** och välj **Ny tjänst**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Ange ett **visningsnamn** för tjänsten och välj **Facebook-tjänsten Custom Audiences** i **tjänstens** listruta.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öppna en ny flik i samma webbläsare och gå till [www.facebook.com.](http://www.facebook.com./) Logga in på Facebook med det konto du vill använda för integreringen.

   >[!CAUTION]
   >
   >För att Marketto ska kunna skicka målgrupper över flera annonshanterarkonton måste Facebook-användaren som du auktoriserar i följande steg ha tillgång till *alla* dessa konton.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. När du har loggat in på Facebook går du tillbaka till Marketo. Klicka på **Auktorisera**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Du *måste* använda ett Facebook Business Manager-konto för att integreringen av anpassade målgrupper ska fungera. Mer information om hur du konfigurerar ett Business Manager-konto finns i [Facebook-hjälpen](https://www.facebook.com/business/help/1710077379203657).

1. Om du uppmanas till det klickar du på **OK **för att godkänna Marketo-appinstallationen på Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du är nu auktoriserad! Välj ett matchande läge och klicka på **Skapa**.

   >[!NOTE]
   >
   >**Grundläggande matchning** använder endast e-postadresser.**För avancerad matchning** används ytterligare sju fält, vilket ökar matchningsfrekvensen, för mer konvertering. Om ditt företags sekretesspolicy inte tillåter delning av ytterligare fält, eller om dina data inte inkluderar dem, väljer du Grundläggande matchning.

   ![](assets/fb-custom-adv-matching-hands.png)

   Bra jobbat! Nu kan ni gå över till alla statiska eller smarta listor i Marketo och skicka målgruppsdata till Facebook.

   >[!CAUTION]
   >
   >Innan du går ska du se till att [godkänna Facebooks villkor](https://www.facebook.com/ads/manage/customaudiences/tos.php) för anpassade målgrupper i ditt Facebook-konto! Om du inte gör det kommer målgruppsuppdateringarna att misslyckas.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Skapa en anpassad målgrupp i Facebook](../../../product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [Konfigurera Facebook-annonser](../../../product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

>



