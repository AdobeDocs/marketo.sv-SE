---
unique-page-id: 2359424
description: Meddela säljaren - Marketo Docs - produktdokumentation
title: Meddela säljaren
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Meddela säljaren {#alert-the-sales-rep}

## Uppgift: Meddela säljaren när en person fyller i ett formulär på din webbplats {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Om du automatiskt vill skicka varningsmeddelanden till säljarna behöver du bara ett varningsmeddelande och en e-postkampanj. Så här gör du.

>[!PREREQUISITES]
>
>[Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Steg 1: Skapa ett e-postmeddelande {#step-create-an-alert-email}

1. Gå till området **[!UICONTROL Marketing Activities]**.

   ![](assets/alert-the-sales-rep-1.png)

1. Välj **Mitt program** som du skapade på [landningssidan med en snabbvinst i form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} och klicka sedan på **[!UICONTROL New]** under **[!UICONTROL New Local Asset]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Namnge** e-postmeddelandet&quot;Min e-postavisering&quot;, välj en mall och klicka på **[!UICONTROL Create]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Ange **Från namn**, **Från e-post**, **[!UICONTROL Reply-to]** och **[!UICONTROL Subject]** som du vill att ditt säljteam ska se.

   ![](assets/alert-the-sales-rep-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/alert-the-sales-rep-6.png)

1. Skriv e-postinnehållet.

   ![](assets/alert-the-sales-rep-7.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på ikonen **Infoga token** .

   ![](assets/alert-the-sales-rep-8.png)

1. Sök efter och markera `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** och klicka på **[!UICONTROL Insert]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en särskild token för varningsmeddelanden. Mer information finns i [Använd informationstoken för skicka-varning](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"}.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Klicka på listrutan **[!UICONTROL Email Actions]** och välj **[!UICONTROL Approve and Close]**.

   ![](assets/alert-the-sales-rep-11.png)

## Steg 2: Skapa en aviseringsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** som skapades tidigare och klicka sedan på **[!UICONTROL New]** **[!UICONTROL New Smart Campaign]** under .

   ![](assets/alert-the-sales-rep-12.png)

1. **Namnge** kampanjen&quot;Min aviseringskampanj&quot; och klicka på **[!UICONTROL Create]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Under fliken **[!UICONTROL Smart List]** letar du upp och drar utlösaren **[!UICONTROL Fills Out Form]** till arbetsytan.

   ![](assets/alert-the-sales-rep-14.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/alert-the-sales-rep-15.png)

1. Under fliken **[!UICONTROL Flow]** söker du efter och drar flödesåtgärden **[!UICONTROL Send Alert]** till arbetsytan.

   ![](assets/alert-the-sales-rep-16.png)

1. Välj **[!UICONTROL My Alert Email]** som skapades tidigare och lämna **[!UICONTROL Send To]** som **[!UICONTROL Sales Owner]**.

   ![](assets/alert-the-sales-rep-17.png)

1. Skriv din e-postadress i fältet **[!UICONTROL To Other Emails]**.

   ![](assets/alert-the-sales-rep-18.png)

1. Gå till fliken **[!UICONTROL Schedule]** och klicka på knappen **[!UICONTROL Activate]**.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Ange **[!UICONTROL Qualification Rules]** till **[!UICONTROL every time]** (genom att redigera den smarta kampanjen) så att samma person kan utlösa varningar flera gånger.

1. Klicka på **[!UICONTROL Activate]** på bekräftelseskärmen.

   ![](assets/alert-the-sales-rep-20.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Välj din landningssida och klicka på **[!UICONTROL View Approved Page]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Glöm inte att godkänna landningssidor. De publiceras inte förrän de godkänts.

1. Fyll i formuläret och klicka på **[!UICONTROL Submit]**.

   ![](assets/alert-the-sales-22.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på fliken **[!UICONTROL Person Info]** i Marketo för att visa kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ Mission 7: Anpassa ett e-postmeddelande](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Uppgift 9: Uppdatera persondata ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
