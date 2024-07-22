---
unique-page-id: 2950549
description: Konfigurera socialt rekommenderat flöde - Marketo Docs - produktdokumentation
title: Konfigurera socialt rekommenderat flöde
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Konfigurera socialt rekommenderat flöde {#configure-social-recommend-flow}

När du skapar en social app kan du konfigurera de val av sociala nätverk och uppmaningar som en användare stöter på när de registrerar sig.

## Välj nätverk för delning {#select-networks-for-sharing}

>[!NOTE]
>
>Detta liknar mycket [att konfigurera flödet för social registrering/delning](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md), men det gäller delningslänkarna _under_ i den sociala appen.

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Markera appen och klicka på **Redigera utkast**.

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. Gå till **Rekommendera flöde** > **Sociala nätverk** i redigeraren för sociala appar.

   ![](assets/recommendedflow.png)

1. Välj de nätverk som en användare kan dela till.

   ![](assets/socialnetworkschoose.png)

## Konfigurera Facebook-meddelandet {#configure-the-facebook-message}

1. Konfigurera meddelandet som ska visas i Facebook-inlägg.

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >I en videodelning genereras miniatyrbilden automatiskt.

   Om du väljer **Lägg till dynamiskt innehåll** läggs värdena för sidans OpenGraph-taggar (log:title, og:caption och og:description) och miniatyrbilden automatiskt till i Facebook-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt innehåll** anger du titel, bildtext och beskrivning och överför en bild. Se de två nästa stegen.

1. Klicka på **Visa redigeringar** i Visa och redigera-fönstret för att anpassa delningsprompten och meddelandet som ska visas i Facebook-inlägg.

   >[!TIP]
   >
   >Mer information finns i [Redigera inställningar för Facebook Rich Post](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >URL:en för [resursen](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) läggs automatiskt till i alla delningsmeddelanden.

1. Om du väljer **Lägg till statiskt innehåll** ovan redigerar du titeln, bildtexten och beskrivningen och överför en anpassad bild (från dina Marketo-bilder och -filer).

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   Se [Lägg till bilder och filer i Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

1. Klicka på **Nästa**.

Om du väljer det här alternativet läggs värdena för sidans OpenGraph-taggar (log:title, og:caption och og:description) och miniatyrbilden automatiskt till i Facebook-inlägg. Se nästa steg.

## Konfigurera Twitterna {#configure-the-twitter-message}

1. Klicka för att redigera delningsprompten och meddelandet som visas i Twitter tweets.

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >Använd {html_title} i tweettexten för att visa sidans rubrik automatiskt.

1. Klicka på **Nästa**.

## Konfigurera LinkedIn-meddelandet {#configure-the-linkedin-message}

1. Konfigurera meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   Om du väljer **Lägg till dynamiskt**-innehåll läggs värdena för sidtaggarna (rubrik och beskrivning) och miniatyrbilden till automatiskt i LinkedIn-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt** innehåll anger du rubrik, bildtext och beskrivning och överför en bild. Se de två nästa stegen.

1. I fönstret **Visa och redigera** klickar du på **Visa redigeringar** och redigerar delningsprompten och meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >Använd {html_title} i din inläggstext för att visa sidans rubrik automatiskt.

1. Om du väljer **Lägg till statiskt**-innehåll ovan redigerar du titeln och beskrivningen och överför en anpassad bild (från dina Marketo-bilder och -filer).

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   Se [Lägg till bilder och filer i Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

1. Klicka på **Nästa**.

## Konfigurera bekräftelsemeddelandet {#configure-the-confirmation-message}

1. Redigera texten i delningsbekräftelsen.

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. Klicka på **Slutför** > **Godkänn** och **Stäng**.

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>Nästa steg är att [lägga till din videoresurs](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md) eller [omröstning](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md) på en landningssida, Facebook eller på din egen webbplats.
