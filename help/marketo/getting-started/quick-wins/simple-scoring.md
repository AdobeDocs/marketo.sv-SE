---
unique-page-id: 2359414
description: Enkel poängsättning - Marketo Docs - produktdokumentation
title: Enkel poängsättning
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Enkel poängsättning {#simple-scoring}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Steg 1: Skapa en resultatkampanj {#step-create-a-scoring-campaign}

1. Gå till **Marknadsföringsaktiviteter** område.

   ![](assets/ma-1.png)

1. Högerklicka på **Utbildning** mapp och klicka på **Ny kampanjmapp**.

   ![](assets/two-2.png)

1. Namnge kampanjmappen Scoring.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Om du redan har en bedömningsmapp ger du den ett annat namn, till exempel Betygsättning 1. Mappnamn måste vara unika.

1. Högerklicka sedan på det nya **Poäng** mapp och markera **Ny smart kampanj**.

   ![](assets/four.png)

1. **Namn** kampanjen&quot;Change Score&quot; och klicka på **Skapa**.

   ![](assets/five-1.png)

1. Klicka på **Smart List** -fliken.

   ![](assets/six-1.png)

   Vi vill att den här kampanjen ska köras när en person fyller i din **Formulär för testbegäran**.

1. Sök och dra **Fyller i formulär** till vänster på arbetsytan.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Välj **Mitt formulär**.

   >[!NOTE]
   >
   >Om du har slutfört [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} snabbwin bör ha formuläret. Om du har använt ett annat namn för formuläret väljer du det.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Klicka på **Flöde** -fliken.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Dra **Ändra poäng** flöda åtgärd till den vänstra arbetsytan.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Du kan skriva vilket värde som helst som ska läggas till i personens poäng. Vi skriver &quot;+5&quot; i **Ändra** fält.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Bra poängsättningskampanjer är avgörande för att leverera högkvalitativa säljare. Läs [**The Definitive Guide to Lead Scoring**](https://www.marketo.com/definitive-guides/lead-scoring/){target=&quot;_blank&quot;}.

1. Klicka på **Schema** -fliken och **Aktivera** -knappen.

   ![](assets/twelve-1.png)

1. Klicka **Aktivera** på bekräftelseskärmen.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>När kampanjen är aktiv körs den varje gång en person fyller i formuläret. Kampanjen fortsätter att löpa tills den har inaktiverats.

## Steg 2: Fyll i formuläret {#step-fill-out-the-form}

1. Välj den landningssida du skapade i dialogrutan [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} snabb vinst.

   ![](assets/fourteen-1.png)

1. Klicka **Visa godkänd sida**. Landningssidan öppnas på en ny flik.

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

## Uppdraget är klart! {#mission-complete}

<br> 

[◄ uppdrag 2: Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Uppdrag 4: Automatiskt svar via e-post ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
