---
unique-page-id: 42762794
description: Använda gruppåtgärder i Salesforce Classic - Marketo Docs - produktdokumentation
title: Använda gruppåtgärder i Salesforce Classic
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---


# Använda gruppåtgärder i Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Lär dig hur du utför satsvisa åtgärder, som att lägga till leads till en kampanj, skicka ett e-postmeddelande eller skicka leads från Salesforce till Sales Connect.

>[!PREREQUISITES]
>
>Uppdatera till den senaste versionen av paketet Sales Connect och installera gruppåtgärdsknapparna i din lead-/kontaktvy. [Klicka här för instruktioner](http://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Innan du följer de angivna stegen måste du kontrollera att du är inloggad på ditt Marketo Sales Connect-konto.

## Massutskick {#bulk-email}

1. Klicka på fliken **Leads** i Salesforce och sedan på knappen **Gå**.

   ![](assets/one-5.png)

1. Välj önskade leads och klicka på knappen **E-post med MSC (Classic)**.

   ![](assets/two-5.png)

1. Ett MSC-e-postmeddelande visas. Den innehåller följande funktioner:

   a. Fältet &quot;Till&quot; visar &quot;Alla kvitton&quot; - motsvarar listan med leads som du har valt i Leadlistvyn\
   b. Den här listan visas i den vänstra panelen, med namnet&quot;Massdisposition&quot; - du kan lägga till/ta bort mottagare här\
   c. Du kan välja en mall eller skapa ett eget e-postmeddelande\
   d. Du kan förhandsgranska dynamiska fält som ska fyllas i i e-postmeddelandet\
   e. Du kan skicka e-postmeddelandet direkt eller schemalägga att skicka det vid ett senare tillfälle

   ![](assets/three-4.png)

## Lägg till i kampanj {#add-to-campaign}

1. Klicka på fliken **Leads** i Salesforce och sedan på knappen **Gå**.

   ![](assets/four-3.png)

1. Välj önskade leads och klicka på knappen **Lägg till i MSC Campaign (Classic)**.

   ![](assets/five-3.png)

1. Popup-fönstret Lägg till personer i din kampanj visas. Klicka på **Nästa** och gå igenom det typiska kampanjflödet för att utlösa en MSC-kampanj.

   ![](assets/six.png)

## Push to Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Klicka på fliken **Leads** i Salesforce och sedan på knappen **Gå**.

   ![](assets/seven-1.png)

1. Välj önskade leads och klicka på knappen **Skicka till MSC (Classic)**.

   ![](assets/eight-1.png)

1. En ny flik med namnet&quot;Salesforce Bridge&quot; öppnas. Klicka på knappen **Gå till grupp →**.

   ![](assets/nine-1.png)

1. Du kommer att skickas till ditt MSC-konto där du kan se en grupp som har skapats med datum-/tidsstämpel. Du får ett meddelande när synkroniseringen är klar och gruppen kommer att inkludera leads som synkroniseras från Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>Du kan även använda gruppåtgärder i kontaktlistvyn genom att följa samma steg.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Skicka e-post via gruppe-post](http://docs.marketo.com/x/KAQ6Ag)
>* [Disponera massutskick med Markera och skicka](http://docs.marketo.com/display/public/DOCS/Composing+Bulk+Emails+with+Select+and+Send#ComposingBulkEmailswithSelectandSend-SendingEmails)

>



