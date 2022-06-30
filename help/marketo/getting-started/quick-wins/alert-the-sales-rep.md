---
unique-page-id: 2359424
description: Meddela säljaren - Marketo Docs - produktdokumentation
title: Meddela säljaren
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '405'
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

   ![](assets/one-5.png)

1. Välj **Mitt program** som du skapade i [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} snabbvinn, sedan under **Nytt** klicka **Ny lokal resurs**.

   ![](assets/two-6.png)

1. Klicka **E-post**.

   ![](assets/three-5.png)

1. **Namn** e-postmeddelandet&quot;Min e-postavisering&quot; väljer du en mall och klickar på **Skapa**.

   ![](assets/four-4.png)

1. Ange **Från namn**, **Från e-post**, **Svar till** och **Ämne** som du vill att ditt säljteam ska se.

   ![](assets/five-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/six-5.png)

1. Skriv e-postinnehållet.

   ![](assets/seven-6.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på **Infoga token** ikon.

   ![](assets/eight-4.png)

1. Sök och välj `{{SP_Send_Alert_Info}}` **Token** och klicka **Infoga**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en särskild token för varningsmeddelanden. Se [Använda Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;} om du vill veta mer.

1. Klicka **Spara**.

   ![](assets/ten-5.png)

1. Stäng fliken/fönstret för e-postredigeraren.

   ![](assets/eleven-5.png)

1. Under **E-poståtgärder** klicka **Godkänn**.

   ![](assets/twelve-4.png)

## Steg 2: Skapa en aviseringsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** tidigare skapat, sedan under **Nytt** klicka **Ny smart kampanj**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Namn** kampanjen&quot;My Alert Campaign&quot; och klicka på **Skapa**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Under **Smart List** -fliken, söka efter och dra **Fyller i formulär** till arbetsytan.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Under **Flöde** -fliken, söka efter och dra **Skicka avisering** flödesåtgärd till arbetsytan.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Välj **Min e-postavisering** skapade tidigare och lämnade **Skicka till** as **Försäljningsägare**.

   ![](assets/eighteen-1.png)

1. Skriv din e-postadress i **Till andra e-postmeddelanden** fält.

   ![](assets/nineteen-2.png)

1. Gå till **Schema** och klicka på **Aktivera** -knappen.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Ange **Kvalificeringsregler** till **varje gång** (genom att redigera Smart Campaign) så att samma person kan utlösa varningar flera gånger.

1. Klicka **Aktivera** på bekräftelseskärmen.

   ![](assets/twenty-one-1.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Välj landningssida och klicka på **Visa godkänd sida**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Glöm inte att godkänna landningssidor. de lever inte förrän de godkänts.

1. Fyll i formuläret och klicka **Skicka**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på **Personinformation** i Marketo för att se kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 7: Anpassa ett e-postmeddelande](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Uppdrag 9: Uppdatera persondata ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
