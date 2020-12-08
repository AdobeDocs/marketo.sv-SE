---
unique-page-id: 2359424
description: Avisera säljaren - Marketo Docs - Produktdokumentation
title: Meddela säljaren
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Meddela säljaren {#alert-the-sales-rep}

## Uppdrag: Meddela säljaren när en person fyller i ett formulär på din webbplats {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Om du automatiskt vill skicka varningsmeddelanden till säljarna behöver du bara ett varningsmeddelande och en e-postkampanj. Så här gör du.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Förutsättningar**
>
>* [Landningssida med ett formulär](landing-page-with-a-form.md)

>



## Steg 1: Skapa ett e-postmeddelande {#step-create-an-alert-email}

1. Gå till området **Marknadsföringsaktiviteter** .

   ![](assets/one-5.png)

1. Välj **Mitt program** som du skapade på [landningssidan med en snabb vinst i form](landing-page-with-a-form.md) och klicka sedan på **Ny lokal resurs** under **Nytt**.

   ![](assets/two-6.png)

1. Klicka på **E-post**.

   ![](assets/three-5.png)

1. **Namnge** e-postmeddelandet&quot;Min e-postavisering&quot;, välj en mall och klicka på **Skapa**.

   ![](assets/four-4.png)

1. Ange **Från namn**, **Från e-post**, **Svar till** och **Ämne** som du vill att ditt säljteam ska se.

   ![](assets/five-5.png)

1. Dubbelklicka om du vill redigera e-posttexten.

   ![](assets/six-5.png)

1. Skriv e-postinnehållet.

   ![](assets/seven-6.png)

1. Placera markören där du vill infoga personens kontaktinformation och klicka på ikonen **Infoga token** .

   ![](assets/eight-4.png)

1. Sök efter och markera `{{SP_Send_Alert_Info}}`**Token** och klicka på **Infoga**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} är en speciell token för varningsmeddelanden. Mer information finns i [Använda informationstoken](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) för skicka-varning.

1. Klicka på **Spara**.

   ![](assets/ten-5.png)

1. Stäng fliken/fönstret för e-postredigeraren.

   ![](assets/eleven-5.png)

1. Klicka på **Godkänn under** E-poståtgärder ****.

   ![](assets/twelve-4.png)

## Steg 2: Skapa en aviseringsutlösarkampanj {#step-create-an-alert-trigger-campaign}

1. Välj **Mitt program** som skapats tidigare och klicka sedan på **Ny smart kampanj** under **Nytt **.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Namnge** kampanjen&quot;Min aviseringskampanj&quot; och klicka på **Skapa**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Under fliken **Smart lista** söker du efter och drar utlösaren för **Fyll i formulär** till arbetsytan.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Markera formuläret som vi skapade tidigare.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Under fliken **Flöde** söker du efter och drar åtgärden **Skicka varningsmeddelande** till arbetsytan.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Välj **Min e-postavisering** som skapades tidigare och lämna **Skicka till** som **försäljningsägare**.

   ![](assets/eighteen-1.png)

1. Skriv din e-postadress i fältet **Till andra e-postmeddelanden** .

   ![](assets/nineteen-2.png)

1. Gå till fliken **Schema** och klicka på knappen **Aktivera **.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >Ställ in **kvalificeringsreglerna** på **varje gång** (genom att redigera Smart Campaign) så att samma person kan utlösa varningar flera gånger.

1. Klicka på **Aktivera** på bekräftelseskärmen.

   ![](assets/twenty-one-1.png)

## Steg 3: Testa det! {#step-test-it-out}

1. Markera landningssidan och klicka på **Visa godkänd sida**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >
   >Glöm inte att godkänna landningssidor. de lever inte förrän de godkänts.

1. Fyll i formuläret och klicka på **Skicka**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Du bör få ditt e-postmeddelande inom kort. När du har verifierat att allt fungerar som det ska tar du bort din e-postadress från sändningsaviseringsflödet (se steg 2.7 ovan).

   >[!NOTE]
   >
   >Klicka på fliken **Personinformation** i Markering för att se kontaktinformationen.

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 7: Anpassa ett e-postuppdrag](personalize-an-email.md) [9: Uppdatera lead-data ►](update-person-data.md)