---
unique-page-id: 2359807
description: Anpassa Lotterimallar - Marketo Docs - Produktdokumentation
title: Anpassa utlottningsstilar
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Anpassa utlottningsstilar {#customize-sweepstakes-styles}

När du [skapar utlottningar](create-sweepstakes.md)kan du anpassa utseendet på landningssidan.

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Gå till Marknadsföringsaktiviteter.

![](assets/login-marketing-activities-1.png)

1. Markera utlottningen och klicka på **Redigera** **utkast**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Gå till **App** **Settings** **>** **Appearance** i Lotteriet.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Redigera texten för anmälningsknappen och förloppslänken.
1. ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Ange anpassade CSS-egenskaper för varje element som du vill anpassa.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exempel på CSS för **Enter-knapp**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>` Exempelbild för **Enter-knappen**:
   `<pre>background:url(http://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Om du använder en bild med text i den måste du komma ihåg att ta bort texten från fältet **Enter** **Button **under Text ovan.

1. När du gör varje ändring visas resultatet i förhandsvisningen för Visa och redigera.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Testa knappen i flera olika webbläsare, inklusive äldre versioner.

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >
   >Nästa steg är att lägga till e-postmeddelanden om [anmälan och uppfyllelse av avhandlingar](../../../../product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).

