---
unique-page-id: 2359807
description: Anpassa Lotterimallar - Marketo Docs - Produktdokumentation
title: Anpassa utlottningsstilar
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Anpassa utlottningsstilar {#customize-sweepstakes-styles}

När du [skapa utlottningar](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)kan du anpassa utseendet på landningssidan.

>[!AVAILABILITY]
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

1. Gå till **Marknadsföringsaktiviteter**.

![](assets/login-marketing-activities-1.png)

1. Markera utlottningen och klicka **Redigera utkast**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. I Lotteriet går du till **Appinställningar** > **Utseende**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Redigera texten för anmälningsknappen och förloppslänken.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Ange anpassade CSS-egenskaper för varje element som du vill anpassa.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exempel på CSS för **Ange knapp**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exempelbild för **Ange knapp**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Om du använder en bild med text på den måste du komma ihåg att ta bort texten från **Ange knapp** under Text ovan.

1. När du gör varje ändring visas resultatet i förhandsvisningen för Visa och redigera.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testa knappen i flera olika webbläsare, inklusive äldre versioner.

   >[!MORELIKETHIS]
   >
   >Nästa steg är att lägga till [e-postmeddelanden om registrering och fullgörande av dina utlottningar](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
