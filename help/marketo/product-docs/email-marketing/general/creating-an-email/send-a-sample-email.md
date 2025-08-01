---
unique-page-id: 1147352
description: Skicka ett exempelmejl - Marketo Docs - produktdokumentation
title: Skicka ett exempelmeddelande
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Skicka ett exempelmeddelande {#send-a-sample-email}

Det går snabbt och enkelt att skicka exempel på e-postmeddelanden. Mer information om hur du skickar e-post med dynamiskt innehåll finns i [Förhandsgranska ett e-postmeddelande med dynamiskt innehåll](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Du måste ha behörigheten **Åtkomstdatabas - Kör enstaka flödesåtgärder** för att kunna skicka exempelmeddelanden.

## Skicka ett exempelmeddelande {#send-a-sample-email-1}

1. Hitta och välj din e-postadress. Klicka på listrutan **[!UICONTROL Email Actions]** och välj **[!UICONTROL Send Sample]**.
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >Mina token matchar det värde som är lämpligt för e-postprogrammet.

1. Ange en eller flera e-postadresser för leverans. Om du har flera e-postadresser avgränsar du dem med kommatecken. Klicka på **[!UICONTROL Send]** när du är klar.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Om du anger flera e-postadresser visas alla för alla mottagare. Den första som anges är huvudmottagaren och varje efterföljande e-postadress blir en CC-mottagare.

   >[!TIP]
   >
   >Om du vill matcha tokens som en viss person väljer du den personen i listrutan **person** i steg 2.

## Skicka ett exempelmeddelande när du redigerar {#send-a-sample-email-while-editing}

1. Leta reda på din e-postadress, markera den och klicka på fliken **[!UICONTROL Edit Draft]**.

   ![](assets/three-281-29.jpg)

1. Klicka på **[!UICONTROL Email Actions]** och välj **[!UICONTROL Send Sample]**.

   ![](assets/four.png)

1. Ange en e-postadress för leverans och klicka på **[!UICONTROL Send]**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Utlösarfältet gäller endast för dem som använder [e-postskript](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting).

## Skicka ett exempelmeddelande baserat på ett segment {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Använd segmentering i din e-post](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Leta reda på din e-postadress, markera den och klicka på fliken **[!UICONTROL Edit Draft]**.

   ![](assets/three-281-29.jpg)

1. Klicka på **[!UICONTROL Preview]**.

   ![](assets/1.png)

1. Klicka på listrutan **[!UICONTROL View By]** och välj **[!UICONTROL Segmentation]**.

   ![](assets/2.png)

1. En listruta med tillgängliga segmenteringar visas. Klicka på den och välj en.

   ![](assets/3.png)

1. Använd pilarna för att bläddra igenom alternativen (i det här fallet har ämnesraden dynamiskt ändrats).

   ![](assets/4.png)

1. Klicka på **[!UICONTROL Send Sample]** om du vill få ett test-e-postmeddelande om ditt segment.

   ![](assets/5.png)

   >[!TIP]
   >
   >Du kan också skicka ett exempelmejl baserat på ett segment i redigeringsläget för e-postmeddelandet. Klicka på listrutan **[!UICONTROL Email Actions]**, markera **[!UICONTROL Send Sample]** och välj sedan ditt segment.

Det är mycket viktigt att ta prov på ditt innehåll innan en kampanj lanseras. Mät två gånger, en gång!
