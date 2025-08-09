---
unique-page-id: 42762825
description: Använda gruppåtgärder i Salesforce Lightning - Marketo Docs - produktdokumentation
title: Använda gruppåtgärder i Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Använda gruppåtgärder i [!DNL Salesforce Lightning] {#using-bulk-actions-in-salesforce-lightning}

Lär dig hur du utför massåtgärder, som att lägga till leads till en kampanj, skicka ett massmeddelande eller skicka leads från [!DNL Salesforce] till [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Uppdatera till den senaste versionen av paketet [!DNL Sales Connect] och installera gruppåtgärdsknapparna i din lead-/kontaktvy.
>* [Instruktioner på engelska](assets/sf-guide-for-lightning-en.pdf)
>* [Instruktioner på japanska](assets/sf-guide-for-lightning-ja.pdf)

>[!NOTE]
>
>Kontrollera att du är inloggad på ditt [!DNL Marketo Sales Connect]-konto innan du följer stegen nedan.

## Massutskick {#bulk-email}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och välj sedan en lista med önskade leads.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Om du redan är med i listan måste du köra den igen genom att välja den i listrutan för att se till att MSC-gruppåtgärdsknapparna visas. Det här är [!DNL Salesforce]-beteendet som inte kan ändras.

1. Klicka på listrutan med pilar (längst till höger på skärmen) och välj **[!UICONTROL Email with MSC]**.

   ![](assets/two-6.png)

1. Ett MSC-e-postmeddelande visas. Den innehåller följande funktioner:

   a. Fältet [!UICONTROL To] visar&quot;Alla kvitton&quot; - det motsvarar listan med leads som du har valt i Lead List-vyn
b. Den här listan visas i den vänstra panelen, med namnet&quot;Massdisposition&quot; - du kan lägga till/ta bort mottagare här
c. Du kan välja en mall eller skapa en egen e-postadress
d. Du kan skicka e-postmeddelandet direkt eller schemalägga att skicka det senare

   ![](assets/three-5.png)

## Lägg till i kampanj {#add-to-campaign}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och välj sedan en lista med önskade leads.

   ![](assets/four-4.png)

1. Klicka på listrutan med pilar (längst till höger på skärmen) och välj **[!UICONTROL Add to MSC Campaign]**.

   ![](assets/five-4.png)

1. Ett [!UICONTROL Add People to Your Campaign]-popup-fönster visas. Klicka på **[!UICONTROL Next]** och gå igenom det typiska kampanjflödet för att utlösa en MSC-kampanj.

   ![](assets/six-1.png)

## Skjut till [!DNL Marketo Sales Connect] {#push-to-marketo-sales-connect}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Leads]** och välj sedan en lista med önskade leads.

   ![](assets/seven-2.png)

1. Klicka på listrutan med pilar (längst till höger på skärmen) och välj **[!UICONTROL Push to MSC]**.

   ![](assets/eight-2.png)

1. En ny flik med namnet [!DNL Salesforce] Bridge öppnas. Klicka på knappen **[!UICONTROL Proceed to Group]→**.

   ![](assets/nine-2.png)

1. Du kommer att skickas till ditt MSC-konto där du kan se en grupp som har skapats med datum-/tidsstämpel. Du får ett meddelande när synkroniseringen är klar och gruppen kommer att innehålla leads som synkroniseras från [!DNL Salesforce].

   ![](assets/ten-1.png)

>[!NOTE]
>
>Du kan även använda gruppåtgärder i kontaktlistvyn genom att följa samma steg.

>[!MORELIKETHIS]
>
>* [Skickar e-postmeddelanden via gruppe-post](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Disponera massutskick med Markera och skicka](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
