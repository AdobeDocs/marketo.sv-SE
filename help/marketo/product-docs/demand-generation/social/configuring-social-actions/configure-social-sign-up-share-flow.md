---
unique-page-id: 2950530
description: Konfigurera Socialt registreringsflöde/Dela flöde - Marketo Docs - Produktdokumentation
title: Konfigurera flöde för social registrering/delning
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---


# Konfigurera socialt registreringsflöde/delningsflöde {#configure-social-sign-up-share-flow}

När du skapar en social app kan du konfigurera de val av sociala nätverk och uppmaningar som en användare stöter på när de registrerar sig.

## Välj nätverk för delning {#select-networks-for-sharing}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera programmet och klicka på **Redigera utkast**.

   ![](assets/image2014-9-22-13-3a57-3a43.png)

1. Klicka på **Registreringsflöde** > **Sociala nätverk** i redigeraren för sociala appar.

   ![](assets/three.png)

1. Markera (eller avmarkera) de nätverk som en person kan dela till.

   ![](assets/four.png)

## Konfigurera Facebook-meddelandet {#configure-the-facebook-message}

1. Gå till **Registreringsflöde** > **Dela meddelanden**.

   ![](assets/five.png)

1. Konfigurera meddelandet som ska visas i Facebook-inlägg.

   ![](assets/image2014-9-22-13-3a58-3a54.png)

   >[!NOTE]
   >
   >I en videodelning genereras miniatyrbilden automatiskt.

   Om du väljer **Lägg till dynamiskt innehåll** läggs värdena för sidans **OpenGraph**-taggar (log:title, og:caption och og:description) och miniatyrbilden automatiskt till Facebook-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt innehåll** anger du titel, bildtext, beskrivning och överför en bild. Se de två nästa stegen.

1. I fönstret Visa och redigera klickar du på **Visa redigeringar** och redigerar delningsprompten och meddelandet som ska visas i Facebook-inlägg.

   >[!TIP]
   >
   >Mer information finns i [Redigera inställningar för Facebook Rich Post](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >URL:en för resursen [läggs automatiskt till i alla delningsmeddelanden.](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)

1. Om du väljer **Lägg till statiskt innehåll** ovan redigerar du titeln, beskrivningen och beskrivningen och överför en anpassad bild (från [**Marketo Images och Files**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   Se [Lägg till bilder och filer i Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

1. Klicka på **Nästa**.

Om du väljer värden för sidans taggar (log:title, og:caption och og:description) läggs miniatyrbilden automatiskt till i Facebook-inlägg. Se nästa steg.

## Konfigurera Twitter-meddelandet {#configure-the-twitter-message}

1. Redigera delningsprompten och meddelandet som ska visas på Twitter-tweetar.

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >Använd {html_title} i tweettexten för att visa sidans titel automatiskt.

1. Klicka på **Nästa**.

## Konfigurera LinkedIn-meddelandet {#configure-the-linkedin-message}

1. Konfigurera meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   Om du väljer **Lägg till dynamiskt innehåll** läggs värdena för sidtaggarna (rubrik och beskrivning) och miniatyrbilden automatiskt till i LinkedIn-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt innehåll** anger du titel, bildtext och beskrivning och överför en bild. Se de två nästa stegen.

1. I fönstret **Visa och redigera** klickar du på **Visa redigeringar** och redigerar delningsprompten och meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >Använd {html_title} i din inläggstext för att visa sidans rubrik automatiskt.

1. Om du väljer **Lägg till statiskt innehåll** ovan redigerar du titeln och beskrivningen och överför en anpassad bild (från [**Marketo Images och Files**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

>[!MORELIKETHIS]
>
>Sedan kan du klicka på **Slutför** > **Godkänn och stäng** och placera din sociala app på en landningssida. Du kan också konfigurera [personhämtning](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md) eller [frågan om att dela om](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md).
