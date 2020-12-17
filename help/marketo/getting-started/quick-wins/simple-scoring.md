---
unique-page-id: 2359414
description: Enkel poängsättning - Marketo Docs - Produktdokumentation
title: Enkel poängsättning
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Enkel poängsättning {#simple-scoring}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](get-set-up-and-add-a-person.md)
>* [Landningssida med ett formulär](landing-page-with-a-form.md)


## Steg 1: Skapa en poängkampanj {#step-create-a-scoring-campaign}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Högerklicka på mappen **Learning** och klicka på **Ny kampanjmapp**.

   ![](assets/two-2.png)

1. Namnge kampanjmappen Scoring.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Om du redan har en bedömningsmapp ger du den ett annat namn, till exempel Betygsättning 1. Mappnamn måste vara unika.

1. Högerklicka sedan på den nya **betygsmappen** och välj **Ny smart kampanj**.

   ![](assets/four.png)

1. **Ge** kampanjen namnet&quot;Change Score&quot; och klicka på  **Create**.

   ![](assets/five-1.png)

1. Klicka på fliken **Smart lista**.

   ![](assets/six-1.png)

   Vi vill att den här kampanjen ska köras när en person fyller i ditt **formulär för testbegäran**.

1. Hitta och dra utlösaren **Fyller i formulär** till den vänstra arbetsytan.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Välj **Mitt formulär**.

   >[!NOTE]
   >
   >Om du har slutfört [landningssidan med ett snabbfönster i form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) bör du ha formuläret. Om du har använt ett annat namn för formuläret väljer du det.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Klicka på fliken **Flöde**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Dra flödesåtgärden **Ändra bakgrundsmusik** till den vänstra arbetsytan.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Du kan skriva vilket värde som helst som ska läggas till i personens poäng. Vi anger &quot;+5&quot; i fältet **Ändra**.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Bra poängsättningskampanjer är avgörande för att leverera högkvalitativa säljare. Läs [**The Definitive Guide to Lead Scoring**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Klicka på fliken **Schema** och **Aktivera**.

   ![](assets/twelve-1.png)

1. Klicka på **Aktivera** på bekräftelseskärmen.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>När kampanjen är aktiv körs den varje gång en person fyller i formuläret. Kampanjen fortsätter att löpa tills den har inaktiverats.

## Steg 2: Fyll i formuläret {#step-fill-out-the-form}

1. Välj landningssidan som du skapade på [landningssidan med ett snabbt Win-formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/fourteen-1.png)

1. Klicka på **Visa godkänd sida**. Landningssidan öppnas på en ny flik.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Fyll i formuläret med ditt förnamn, efternamn och e-postadress och klicka sedan på **Skicka**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Använd samma namn och e-postadress som du använde när du först angav dig själv som en person för att tillämpa poängökningen &quot;+5&quot;.

## Steg 3: Visa personinformation {#step-view-the-person-info}

1. Gå till området Databas.

   ![](assets/db-2.png)

1. Sök efter den e-postadress som du använde när du fyllde i formuläret.

   ![](assets/eighteen.png)

1. Dubbelklicka på personen.

   ![](assets/nineteen.png)

Personuppgifterna öppnas på en ny flik eller i ett nytt fönster. Se hur poängen ökade med 5 poäng för att fylla i formuläret!

![](assets/twenty.png)

**Grattis!** Du har skapat en poängsättningskampanj.
[◄ uppdrag 2: Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Uppdrag 4: Automatiskt svar via e-post ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
