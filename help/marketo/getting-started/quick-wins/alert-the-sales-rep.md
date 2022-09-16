---
unique-page-id: 2359424
description: Meddela säljaren - Marketo Docs - produktdokumentation
title: Meddela säljaren
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 1127928b43762086ed4d157719ff80d6c3de9ee3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Meddela säljaren {#alert-the-sales-rep}

## Uppdrag: Meddela säljaren när en person fyller i ett formulär på din webbplats {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Om du automatiskt vill skicka varningsmeddelanden till säljarna behöver du bara ett varningsmeddelande och en e-postkampanj. Så här gör du.

>[!PREREQUISITES]
>
>[Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## Steg 1: Skapa ett e-postmeddelande {#step-create-an-alert-email}

1. Gå till **Marknadsföringsaktiviteter** område.

   ![](assets/alert-the-sales-rep-1.png)

1. Välj **Mitt program** som du skapade i [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} snabbvinn, sedan under **Nytt** klicka **Ny lokal resurs**.

   ![](assets/alert-the-sales-rep-2.png)

1. Klicka **E-post**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Namn** e-postmeddelandet&quot;Min e-postavisering&quot; väljer du en mall och klickar på **Skapa**.

   ![](assets/alert-the-sales-rep-4.png)

1. Ange **Från namn**, **Från e-post**, **Svar till** och **Ämne** som du vill att ditt säljteam ska se.

   ![](assets/alert-the-sales-rep-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/alert-the-sales-rep-6.png)

1. Skriv e-postinnehållet.

   ![](assets/alert-the-sales-rep-7.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på **Infoga token** ikon.

   ![](assets/alert-the-sales-rep-8.png)

1. Sök och välj `{{SP_Send_Alert_Info}}` **Token** och klicka **Infoga**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en särskild token för varningsmeddelanden. Se [Använda Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;} om du vill veta mer.

1. Klicka **Spara**.

   ![](assets/alert-the-sales-rep-10.png)

1. Klicka på **E-poståtgärder** nedrullningsbar meny och välj **Godkänn och stäng**.

   ![](assets/alert-the-sales-rep-11.png)

## Steg 2: Skapa en aviseringsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** tidigare skapat, sedan under **Nytt** klicka **Ny smart kampanj**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Namn** kampanjen&quot;My Alert Campaign&quot; och klicka på **Skapa**.

   ![](assets/alert-the-sales-rep-13.png)

1. Under **Smart List** -fliken, söka efter och dra **Fyller i formulär** till arbetsytan.

   ![](assets/alert-the-sales-rep-14.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/alert-the-sales-rep-15.png)

1. Under **Flöde** -fliken, söka efter och dra **Skicka avisering** flödesåtgärd till arbetsytan.

   ![](assets/alert-the-sales-rep-16.png)

1. Välj **Min e-postavisering** skapade tidigare och lämnade **Skicka till** as **Försäljningsägare**.

   ![](assets/alert-the-sales-rep-17.png)

1. Skriv din e-postadress i **Till andra e-postmeddelanden** fält.

   ![](assets/alert-the-sales-rep-18.png)

1. Gå till **Schema** och klicka på **Aktivera** -knappen.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Ange **Kvalificeringsregler** till **varje gång** (genom att redigera Smart Campaign) så att samma person kan utlösa varningar flera gånger.

1. Klicka **Aktivera** på bekräftelseskärmen.

   ![](assets/alert-the-sales-rep-20.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Välj landningssida och klicka på **Visa godkänd sida**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Glöm inte att godkänna landningssidor. de lever inte förrän de godkänts.

1. Fyll i formuläret och klicka **Skicka**.

   ![](assets/alert-the-sales-22.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på **Personinformation** i Marketo för att se kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 7: Anpassa ett e-postmeddelande](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Uppdrag 9: Uppdatera persondata ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
