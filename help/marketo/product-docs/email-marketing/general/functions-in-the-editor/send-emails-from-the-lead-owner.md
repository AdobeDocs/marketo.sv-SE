---
unique-page-id: 1147340
description: Skicka e-post från Lead Owner - Marketo Docs - Produktdokumentation
title: Skicka e-post från lead-ägaren
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Skicka e-post från lead-ägaren {#send-emails-from-the-lead-owner}

Vad händer om du vill skicka ett e-postmeddelande till en lead för leadägaren?  Så här gör du.

1. Leta upp e-postmeddelandet, markera det och klicka på **Redigera utkast**.

   ![](assets/one.png)

1. Klicka i fältet **Från** (ta bort ett befintligt namn) och klicka på knappen **Infoga token** .

   ![](assets/two.png)

1. Börja skriva &quot;`{{lead.Lead Owner`&quot; och välj **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Klicka efter den första variabeln, lägg till ett blanksteg och klicka sedan på knappen **Infoga token** .

   ![](assets/five.png)

1. Börja skriva &quot;`{{lead.Lead Owner`&quot; och välj **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Se till att du har lagt till ett blanksteg mellan för- och efternamnstoken.

   Klicka i fältet Från e-post (ta bort en befintlig e-postadress) och klicka på knappen Infoga token.
   ![](assets/eight.png)

1. Börja skriva &quot;`{{lead.Lead Owner`&quot; och välj **`{{lead.Lead Owner Email Address}}`** token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **Infoga**.

   ![](assets/ten.png)

1. Se till att fälten **Svar till** och **Ämne** är ifyllda. Klart!

   ![](assets/eleven.png)

