---
unique-page-id: 42762825
description: Använda gruppåtgärder i Salesforce Lightning - Marketo Docs - Produktdokumentation
title: Använda gruppåtgärder i Salesforce Lightning
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Använda gruppåtgärder i Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Lär dig hur du utför satsvisa åtgärder, som att lägga till leads till en kampanj, skicka ett e-postmeddelande eller skicka leads från Salesforce till Sales Connect.

>[!PREREQUISITES]
>
>Uppdatera till den senaste versionen av paketet Sales Connect och installera gruppåtgärdsknapparna i din lead-/kontaktvy. [Klicka här för instruktioner](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Innan du följer stegen nedan kontrollerar du att du är inloggad på ditt Marketo Sales Connect-konto.

## Massutskick {#bulk-email}

1. Klicka på fliken **Leads** i Salesforce och välj sedan en lista med önskade leads.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Om du redan är med i listan måste du köra den igen genom att välja den i listrutan för att se till att MSC-gruppåtgärdsknapparna visas. Det här är Salesforce-beteende som inte kan ändras.

1. Klicka på pilen i listrutan (längst till höger på skärmen) och välj **E-post med MSC**.

   ![](assets/two-6.png)

1. Ett MSC-e-postmeddelande visas. Den innehåller följande funktioner:

   a. Fältet &quot;Till&quot; visar &quot;Alla kvitton&quot; - motsvarar listan med leads som du har valt i Leadlistvyn\
   b. Den här listan visas i den vänstra panelen, med namnet&quot;Massdisposition&quot; - du kan lägga till/ta bort mottagare här\
   c. Du kan välja en mall eller skapa ett eget e-postmeddelande\
   d. Du kan skicka e-postmeddelandet direkt eller schemalägga att skicka det vid ett senare tillfälle

   ![](assets/three-5.png)

## Lägg till i kampanj {#add-to-campaign}

1. Klicka på fliken **Leads** i Salesforce och välj sedan en lista med önskade leads.

   ![](assets/four-4.png)

1. Klicka på pilen i listrutan (längst till höger på skärmen) och välj **Lägg till i MSC Campaign**.

   ![](assets/five-4.png)

1. Popup-fönstret Lägg till personer i din kampanj visas. Klicka på **Nästa** och gå igenom det typiska kampanjflödet för att utlösa en MSC-kampanj.

   ![](assets/six-1.png)

## Push to Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Klicka på fliken **Leads** i Salesforce och välj sedan en lista med önskade leads.

   ![](assets/seven-2.png)

1. Klicka på listrutan med pilar (längst till höger på skärmen) och välj **Skicka till MSC**.

   ![](assets/eight-2.png)

1. En ny flik med namnet&quot;Salesforce Bridge&quot; öppnas. Klicka på knappen **Gå till grupp→** .

   ![](assets/nine-2.png)

1. Du kommer att skickas till ditt MSC-konto där du kan se en grupp som har skapats med datum-/tidsstämpel. Du får ett meddelande när synkroniseringen är klar och gruppen kommer att inkludera leads som synkroniseras från Salesforce.

   ![](assets/ten-1.png)

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



