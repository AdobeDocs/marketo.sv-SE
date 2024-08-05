---
unique-page-id: 2950530
description: Konfigurera Socialt registreringsflöde/Dela flöde - Marketo Docs - Produktdokumentation
title: Konfigurera flöde för social registrering/delning
exl-id: 521187d1-2228-42e7-a87b-3b20a45adb03
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Konfigurera flöde för social registrering/delning {#configure-social-sign-up-share-flow}

När du skapar en social app kan du konfigurera de val av sociala nätverk och uppmaningar som en användare stöter på när de registrerar sig.

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Nya resurser kan inte längre skapas. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Välj nätverk för delning {#select-networks-for-sharing}

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera appen och klicka på **Redigera utkast**.

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

   Om du väljer **Lägg till dynamiskt innehåll** läggs värdena för sidans **OpenGraph** -taggar (log:title, og:caption och og:description) och miniatyrbilden automatiskt till i Facebook-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt innehåll** anger du titeln, bildtexten, beskrivningen och överför en bild. Se de två nästa stegen.

1. I fönstret Visa och redigera klickar du på **Visa redigeringar** och redigerar delningsprompten och meddelandet som ska visas i Facebook-inlägg.

   >[!TIP]
   >
   >Mer information finns i [Redigera inställningar för Facebook Rich Post](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >URL:en för [resursen](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) läggs automatiskt till i alla delningsmeddelanden.

1. Om du väljer **Lägg till statiskt innehåll** ovan redigerar du titeln, bildtexten och beskrivningen och överför en anpassad bild (från dina [**Marketo-bilder och filer**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   Se [Lägg till bilder och filer i Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

1. Klicka på **Nästa**.

Om du väljer värden för sidans taggar (log:title, og:caption och og:description) läggs miniatyrbilden automatiskt till i Facebook-inlägg. Se nästa steg.

## Konfigurera Twitterna {#configure-the-twitter-message}

1. Redigera delningsprompten och meddelandet som ska visas i Twitter tweets.

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >Använd {html_title} i tweettexten för att visa sidans rubrik automatiskt.

1. Klicka på **Nästa**.

## Konfigurera LinkedIn-meddelandet {#configure-the-linkedin-message}

1. Konfigurera meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   Om du väljer **Lägg till dynamiskt innehåll** läggs värdena för sidtaggarna (rubrik och beskrivning) och miniatyrbilden till automatiskt i LinkedIn-inlägg. Se nästa steg.

   Om du väljer **Lägg till statiskt innehåll** anger du titel, bildtext och beskrivning och överför en bild. Se de två nästa stegen.

1. I fönstret **Visa och redigera** klickar du på **Visa redigeringar** och redigerar delningsprompten och meddelandet som ska visas i LinkedIn-inlägg.

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >Använd {html_title} i din inläggstext för att visa sidans rubrik automatiskt.

1. Om du väljer **Lägg till statiskt innehåll** ovan redigerar du titeln och beskrivningen och överför en anpassad bild (från dina [**Marketo-bilder och filer**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>Om du överför en bild visas den inte här förrän du stänger och öppnar redigeraren för sociala appar igen.

>[!MORELIKETHIS]
>
>Sedan kan du klicka på **Slutför** > **Godkänn och stäng** och placera din sociala app på en landningssida. Du kan också konfigurera [Personhämtning](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md) eller uppmaningen [Dela igen](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md).
