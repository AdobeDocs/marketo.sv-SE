---
unique-page-id: 1147340
description: Skicka e-post från huvudägaren - Marketo Docs - Produktdokumentation
title: Skicka e-post från lead-ägaren
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Skicka e-post från lead-ägaren {#send-emails-from-the-lead-owner}

Vad händer om du vill skicka ett e-postmeddelande till en lead för leadägaren?  Så här gör du.

1. Leta reda på din e-postadress, markera den och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/one.png)

1. Klicka i fältet **[!UICONTROL From]** (ta bort ett befintligt namn) och klicka på knappen **Infoga token** .

   ![](assets/two.png)

1. Börja skriva `{{lead.Lead Owner` och välj **`{{lead.Lead Owner First Name}}`**-token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **[!UICONTROL Insert]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Klicka efter den första token, lägg till ett blanksteg och klicka sedan på knappen **Infoga token** .

   ![](assets/five.png)

1. Börja skriva `{{lead.Lead Owner` och välj **`{{lead.Lead Owner Last Name}}`**-token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **[!UICONTROL Insert]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Se till att du har lagt till ett blanksteg mellan för- och efternamnstoken.

1. Klicka i fältet **[!UICONTROL From Address]** (ta bort en befintlig e-postadress) och klicka på knappen **Infoga token** .

   ![](assets/eight.png)

1. Börja skriva `{{lead.Lead Owner` och välj **`{{lead.Lead Owner Email Address}}`**-token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Ange ett standardvärde om leadet ännu inte har någon lead-ägare och klicka på **[!UICONTROL Insert]**.

   ![](assets/ten.png)

1. Kontrollera att fälten **[!UICONTROL Reply-to]** och **[!UICONTROL Subject]** är ifyllda, och att du är klar!

   ![](assets/eleven.png)
