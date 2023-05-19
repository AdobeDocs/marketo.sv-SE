---
unique-page-id: 2359424
description: Meddela säljaren - Marketo Docs - produktdokumentation
title: Meddela säljaren
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Meddela säljaren {#alert-the-sales-rep}

## Uppdrag: Meddela säljaren när en person fyller i ett formulär på din webbplats {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Om du automatiskt vill skicka varningsmeddelanden till säljarna behöver du bara ett varningsmeddelande och en e-postkampanj. Så här gör du.

>[!PREREQUISITES]
>
>[Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Steg 1: Skapa ett e-postmeddelande {#step-create-an-alert-email}

1. Gå till **[!UICONTROL Marketing Activities]** område.

   ![](assets/alert-the-sales-rep-1.png)

1. Välj **Mitt program** som du skapade i [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} snabbvinn, sedan under **[!UICONTROL New]** klicka **[!UICONTROL New Local Asset]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Klicka på **[!UICONTROL Email]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Namn** e-postmeddelandet&quot;Min e-postavisering&quot; väljer du en mall och klickar på **[!UICONTROL Create]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Ange **Från namn**, **Från e-post**, **[!UICONTROL Reply-to]** och **[!UICONTROL Subject]** som du vill att ditt säljteam ska se.

   ![](assets/alert-the-sales-rep-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/alert-the-sales-rep-6.png)

1. Skriv e-postinnehållet.

   ![](assets/alert-the-sales-rep-7.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på **Infoga token** ikon.

   ![](assets/alert-the-sales-rep-8.png)

1. Sök och välj `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** och klicka **[!UICONTROL Insert]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en särskild token för varningsmeddelanden. Se [Använda Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} om du vill veta mer.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Klicka på **[!UICONTROL Email Actions]** nedrullningsbar meny och välj **[!UICONTROL Approve and Close]**.

   ![](assets/alert-the-sales-rep-11.png)

## Steg 2: Skapa en aviseringsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** tidigare skapat, sedan under **[!UICONTROL New]** klicka **[!UICONTROL New Smart Campaign]**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Namn** kampanjen&quot;My Alert Campaign&quot; och klicka på **[!UICONTROL Create]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Under **[!UICONTROL Smart List]** -fliken, söka efter och dra **[!UICONTROL Fills Out Form]** till arbetsytan.

   ![](assets/alert-the-sales-rep-14.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/alert-the-sales-rep-15.png)

1. Under **[!UICONTROL Flow]** -fliken, söka efter och dra **[!UICONTROL Send Alert]** flödesåtgärd till arbetsytan.

   ![](assets/alert-the-sales-rep-16.png)

1. Välj **[!UICONTROL My Alert Email]** skapade tidigare och lämnade **[!UICONTROL Send To]** as **[!UICONTROL Sales Owner]**.

   ![](assets/alert-the-sales-rep-17.png)

1. Skriv din e-postadress i **[!UICONTROL To Other Emails]** fält.

   ![](assets/alert-the-sales-rep-18.png)

1. Gå till **[!UICONTROL Schedule]** och klicka på **[!UICONTROL Activate]** -knappen.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Ange **[!UICONTROL Qualification Rules]** till **[!UICONTROL every time]** (genom att redigera Smart Campaign) så att samma person kan utlösa varningar flera gånger.

1. Klicka **[!UICONTROL Activate]** på bekräftelseskärmen.

   ![](assets/alert-the-sales-rep-20.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Välj landningssida och klicka på **[!UICONTROL View Approved Page]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Glöm inte att godkänna landningssidor. de lever inte förrän de godkänts.

1. Fyll i formuläret och klicka **[!UICONTROL Submit]**.

   ![](assets/alert-the-sales-22.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på **[!UICONTROL Person Info]** i Marketo för att se kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 7: Anpassa ett e-postmeddelande](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Uppdrag 9: Uppdatera persondata ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
