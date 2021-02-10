---
unique-page-id: 1147340
description: Skicka e-post från Lead Owner - Marketo Docs - Produktdokumentation
title: Skicka e-post från lead-ägaren
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Skicka e-postmeddelanden från leadägaren {#send-emails-from-the-lead-owner}

Vad händer om du vill skicka ett e-postmeddelande till en lead för leadägaren?  Så här gör du.

1. Leta reda på e-postmeddelandet, markera det och klicka på **Redigera utkast**.

   ![](assets/one.png)

1. Klicka i fältet **Från** (ta bort ett befintligt namn) och klicka på knappen **Infoga token**.

   ![](assets/two.png)

1. Börja skriva `{{lead.Lead Owner` och välj token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Klicka efter den första token, lägg till ett blanksteg och klicka sedan på knappen **Infoga token**.

   ![](assets/five.png)

1. Börja skriva `{{lead.Lead Owner` och välj token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Se till att du har lagt till ett blanksteg mellan för- och efternamnstoken.

1. Klicka i fältet Från e-post (ta bort en befintlig e-postadress) och klicka på knappen Infoga token.

   ![](assets/eight.png)

1. Börja skriva `{{lead.Lead Owner` och välj token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/ten.png)

1. Se till att fälten **Svara till** och **Ämne** är ifyllda. Klart!

   ![](assets/eleven.png)
