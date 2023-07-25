---
unique-page-id: 1147352
description: Skicka ett exempelmejl - Marketo Docs - produktdokumentation
title: Skicka ett exempelmeddelande
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Skicka ett exempelmeddelande {#send-a-sample-email}

Det går snabbt och enkelt att skicka exempel på e-postmeddelanden. Information om hur du skickar ett e-postmeddelande med dynamiskt innehåll finns i [Förhandsgranska ett e-postmeddelande med dynamiskt innehåll](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Du måste ha **Access Database - Run Single Flow Actions** behörighet att skicka exempelmeddelanden.

## Skicka ett exempelmeddelande {#send-a-sample-email-1}

1. Hitta och välj din e-postadress. Klicka på **E-poståtgärder** nedrullningsbar meny och välj **Skicka exempel**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >Mina token matchar värdet som passar e-postprogrammet.

1. Ange en eller flera e-postadresser för leverans. Om du har flera e-postadresser avgränsar du dem med kommatecken. Klicka **Skicka** när det är klart.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Om du anger flera e-postadresser visas alla för alla mottagare. Den första som anges är huvudmottagaren och varje efterföljande e-postadress blir en CC-mottagare.

   >[!TIP]
   >
   >Om du vill lösa tokens som en viss person väljer du den personen i **listruta för person** i steg 2.

## Skicka ett exempelmeddelande när du redigerar {#send-a-sample-email-while-editing}

1. Leta upp e-postmeddelandet, markera det och klicka på **Redigera utkast** -fliken.

   ![](assets/three-281-29.jpg)

1. Klicka **E-poståtgärder**, markera **Skicka exempel**.

   ![](assets/four.png)

1. Ange en e-postadress för leverans och klicka på **Skicka**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Utlösarfältet gäller bara för de som använder [e-postskript](https://developers.marketo.com/documentation/velocity-script/).

## Skicka ett exempelmeddelande baserat på ett segment {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Använd segmentering i e-postmeddelanden](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Leta upp e-postmeddelandet, markera det och klicka på **Redigera utkast** -fliken.

   ![](assets/three-281-29.jpg)

1. Klicka **Förhandsgranska**.

   ![](assets/1.png)

1. Klicka på **Visa efter** nedrullningsbar meny och välj **Segmentering**.

   ![](assets/2.png)

1. En listruta med tillgängliga segmenteringar visas. Klicka på den och välj en.

   ![](assets/3.png)

1. Använd pilarna för att bläddra igenom alternativen (i det här fallet har ämnesraden dynamiskt ändrats).

   ![](assets/4.png)

1. Klicka **Skicka exempel** om du vill få ett test-e-postmeddelande om ditt segment.

   ![](assets/5.png)

   >[!TIP]
   >
   >Du kan också skicka ett exempelmejl baserat på ett segment i redigeringsläget för e-postmeddelandet. Klicka på **E-poståtgärder** nedrullningsbar meny, välja **Skicka exempel** väljer du sedan ditt segment.

Det är mycket viktigt att ta prov på ditt innehåll innan en kampanj lanseras. Mät två gånger, en gång!
