---
unique-page-id: 42762794
description: Använda gruppåtgärder i Salesforce Classic - Marketo Docs - produktdokumentation
title: Använda gruppåtgärder i Salesforce Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Använda gruppåtgärder i Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Lär dig hur du utför satsvisa åtgärder, som att lägga till leads till en kampanj, skicka ett e-postmeddelande eller skicka leads från Salesforce till Sales Connect.

>[!PREREQUISITES]
>
>Uppdatera till den senaste versionen av paketet Sales Connect och installera gruppåtgärdsknapparna i din lead-/kontaktvy. [Klicka här för instruktioner](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Kontrollera att du är inloggad på ditt Marketo Sales Connect-konto innan du följer instruktionerna.

## Massutskick {#bulk-email}

1. I Salesforce klickar du på **Leads** -fliken och sedan **Gå** -knappen.

   ![](assets/one-5.png)

1. Välj önskade leads och klicka på **E-post med MSC (Classic)** -knappen.

   ![](assets/two-5.png)

1. Ett MSC-e-postmeddelande visas. Den innehåller följande funktioner:

   a. Fältet &quot;Till&quot; visar &quot;Alla kvitton&quot; - motsvarar listan med leads som du har valt i Leadlistvyn\
   b. Den här listan visas i den vänstra panelen, med namnet&quot;Massdisposition&quot; - du kan lägga till/ta bort mottagare här\
   c. Du kan välja en mall eller skapa ett eget e-postmeddelande\
   d. Du kan förhandsgranska dynamiska fält som ska fyllas i i e-postmeddelandet\
   e. Du kan skicka e-postmeddelandet direkt eller schemalägga att skicka det vid ett senare tillfälle

   ![](assets/three-4.png)

## Lägg till i kampanj {#add-to-campaign}

1. I Salesforce klickar du på **Leads** -fliken och sedan **Gå** -knappen.

   ![](assets/four-3.png)

1. Välj önskade leads och klicka på **Lägg till i MSC Campaign (Classic)** -knappen.

   ![](assets/five-3.png)

1. Popup-fönstret Lägg till personer i din kampanj visas. Klicka **Nästa** och gå igenom det typiska kampanjflödet för att utlösa en MSC-kampanj.

   ![](assets/six.png)

## Skicka till Marketo Sales Connect {#push-to-marketo-sales-connect}

1. I Salesforce klickar du på **Leads** -fliken och sedan **Gå** -knappen.

   ![](assets/seven-1.png)

1. Välj önskade leads och klicka på **Skicka till MSC (klassisk)** -knappen.

   ![](assets/eight-1.png)

1. En ny flik med namnet&quot;Salesforce Bridge&quot; öppnas. Klicka på **Gå till grupp →** -knappen.

   ![](assets/nine-1.png)

1. Du kommer att skickas till ditt MSC-konto där du kan se en grupp som har skapats med datum-/tidsstämpel. Du får ett meddelande när synkroniseringen är klar och gruppen kommer att inkludera leads som synkroniseras från Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>Du kan även använda gruppåtgärder i kontaktlistvyn genom att följa samma steg.

>[!MORELIKETHIS]
>
>* [Skicka e-post via gruppe-post](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Disponera massutskick med Markera och skicka](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

