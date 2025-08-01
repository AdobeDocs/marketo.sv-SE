---
unique-page-id: 42762794
description: Använda gruppåtgärder i [!DNL Salesforce] Classic - Marketo Docs - produktdokumentation
title: Använda gruppåtgärder i [!DNL Salesforce] Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Använda gruppåtgärder i [!DNL Salesforce] Classic {#using-bulk-actions-in-salesforce-classic}

Lär dig hur du utför massåtgärder, som att lägga till leads till en kampanj, skicka ett massmeddelande eller skicka leads från [!DNL Salesforce] till [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Uppdatera till den senaste versionen av paketet [!DNL Sales Connect] och installera gruppåtgärdsknapparna i din lead-/kontaktvy. [Klicka här för instruktioner](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Kontrollera att du är inloggad på ditt Marketo Sales Connect-konto innan du följer instruktionerna.

## Massutskick {#bulk-email}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och sedan på knappen **[!UICONTROL Go]**.

   ![](assets/one-5.png)

1. Välj önskade leads och klicka på knappen **[!UICONTROL Email with MSC (Classic)]**.

   ![](assets/two-5.png)

1. Ett MSC-e-postmeddelande visas. Den innehåller följande funktioner:

   a. Fältet [!UICONTROL To] visar [!UICONTROL All Recipients] - detta motsvarar listan med leads som du har valt i Lead List-vyn
b. Den här listan visas på den vänstra panelen med namnet [!UICONTROL Bulk Compose] - du kan lägga till/ta bort mottagare här
c. Du kan välja en mall eller skapa en egen e-postadress
d. Du kan förhandsgranska dynamiska fält som ska fyllas i i ditt e-postmeddelande
e. Du kan skicka e-postmeddelandet direkt eller schemalägga att skicka det senare

   ![](assets/three-4.png)

## Lägg till i kampanj {#add-to-campaign}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och sedan på knappen **[!UICONTROL Go]**.

   ![](assets/four-3.png)

1. Välj önskade leads och klicka på knappen **[!UICONTROL Add to MSC Campaign (Classic)]**.

   ![](assets/five-3.png)

1. Ett [!UICONTROL Add People to Your Campaign]-popup-fönster visas. Klicka på **[!UICONTROL Next]** och gå igenom det typiska kampanjflödet för att utlösa en MSC-kampanj.

   ![](assets/six.png)

## Skicka till Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och sedan på knappen **[!UICONTROL Go]**.

   ![](assets/seven-1.png)

1. Välj önskade leads och klicka på knappen **[!UICONTROL Push to MSC (Classic)]**.

   ![](assets/eight-1.png)

1. En ny flik med namnet [!UICONTROL Salesforce Bridge] öppnas. Klicka på knappen **[!UICONTROL Proceed to Group →]**.

   ![](assets/nine-1.png)

1. Du kommer att skickas till ditt MSC-konto där du kan se en grupp som har skapats med datum-/tidsstämpel. Du får ett meddelande när synkroniseringen är klar och gruppen kommer att innehålla leads som synkroniseras från [!DNL Salesforce].

   ![](assets/ten.png)

>[!NOTE]
>
>Du kan även använda gruppåtgärder i kontaktlistvyn genom att följa samma steg.

>[!MORELIKETHIS]
>
>* [Skickar e-postmeddelanden via gruppe-post](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Disponera massutskick med Markera och skicka](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
