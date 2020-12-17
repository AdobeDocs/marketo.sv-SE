---
unique-page-id: 2359424
description: Avisera säljaren - Marketo Docs - Produktdokumentation
title: Meddela säljaren
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Avisera säljaren {#alert-the-sales-rep}

## Uppdrag: Meddela säljaren när en person fyller i ett formulär på din webbplats {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Om du automatiskt vill skicka varningsmeddelanden till säljarna behöver du bara ett varningsmeddelande och en e-postkampanj. Så här gör du.

>[!PREREQUISITES]
>
>[Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Steg 1: Skapa ett varningsmeddelande {#step-create-an-alert-email}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/one-5.png)

1. Välj **Mitt program** som du skapade på [landningssidan med ett snabbfönster i formatet](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) och klicka sedan på **Nytt** på **Ny lokal resurs**.

   ![](assets/two-6.png)

1. Klicka på **E-post**.

   ![](assets/three-5.png)

1. **Ange e-** postnamnet&quot;Min e-postavisering&quot;, välj en mall och klicka på  **Skapa**.

   ![](assets/four-4.png)

1. Ange **Från namn**, **Från e-post**, **Svar till** och **Ämne** som du vill att ditt säljteam ska se.

   ![](assets/five-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/six-5.png)

1. Skriv e-postinnehållet.

   ![](assets/seven-6.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på ikonen **Infoga token**.

   ![](assets/eight-4.png)

1. Sök efter och välj `{{SP_Send_Alert_Info}}` **Token** och klicka på **Infoga**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en speciell token för varningsmeddelanden. Mer information finns i [Använd Skicka aviseringsinformationstoken](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md).

1. Klicka på **Spara**.

   ![](assets/ten-5.png)

1. Stäng fliken/fönstret för e-postredigeraren.

   ![](assets/eleven-5.png)

1. Under **E-poståtgärder** klickar du på **Godkänn**.

   ![](assets/twelve-4.png)

## Steg 2: Skapa en varningsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** som har skapats tidigare och klicka sedan på **Ny smart kampanj** under &lt;a2/>Ny **på &lt;a4/>Ny smart kampanj**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Ge** kampanjen namnet&quot;Min aviseringskampanj&quot; och klicka på  **Skapa**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Under fliken **Smart List** letar du upp och drar utlösaren **Fyll i formulär** till arbetsytan.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Under fliken **Flöde** söker du efter och drar flödesåtgärden **Skicka varning** till arbetsytan.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Välj **Min aviseringse-postadress** som skapades tidigare och lämna **Skicka till** som **Säljare**.

   ![](assets/eighteen-1.png)

1. Skriv din e-postadress i fältet **Till andra e-postmeddelanden**.

   ![](assets/nineteen-2.png)

1. Gå till fliken **Schema** och klicka på knappen **Aktivera**.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Ange **kvalificeringsreglerna** till **varje gång** (genom att redigera Smart Campaign) så att samma person kan utlösa varningar flera gånger.

1. Klicka på **Aktivera** på bekräftelseskärmen.

   ![](assets/twenty-one-1.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Välj landningssida och klicka på **Visa godkänd sida**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Glöm inte att godkänna landningssidor. de lever inte förrän de godkänts.

1. Fyll i formuläret och klicka på **Skicka**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på fliken **Personinformation** i Markför att se kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 7: Anpassa ett e-postmeddelande](personalize-an-email.md)

[Uppdrag 9: Uppdatera lead-data ►](update-person-data.md)
