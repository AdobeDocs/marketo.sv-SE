---
unique-page-id: 2359416
description: Automatiskt svar via e-post - Marketo Docs - produktdokumentation
title: Automatiskt svar för e-post
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Automatiskt svar för e-post {#email-auto-response}

## Uppdrag: Skicka ett tackmeddelande när en person fyller i ett formulär {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Konfigurera och lägga till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)


## Steg 1: Skapa ett e-postmeddelande {#step-create-an-email}

1. Gå till området Marknadsföringsaktiviteter.

   ![](assets/one-2.png)

1. Välj Mitt program på den vänstra menyn, klicka på listrutan Ny lokal resurs och välj Ny lokal resurs.

   ![](assets/two-3.png)

1. Klicka på E-post.

   ![](assets/three-2.png)

1. Ge e-postmeddelandet namnet&quot;Autosvar e-post&quot;, välj en mall och klicka på Skapa.

   ![](assets/four-1.png)

   En e-postredigerare öppnas i ett nytt fönster eller på en ny flik. Om popup-fönster är blockerade klickar du på **Redigera utkast** på resurssammanfattningssidan för att komma åt e-postmeddelandet.

1. Ange en ämnesrad och dubbelklicka sedan på det redigerbara området i e-postmeddelandet.

   ![](assets/five-2.png)

   _En textredigerare öppnas ovanpå e-postredigeraren._

1. Markera befintligt e-postinnehåll.

   ![](assets/six-2.png)

1. Skriv ditt e-postinnehåll och klicka på Spara.

   ![](assets/seven-2.png)

1. Dina ändringar sparas automatiskt. Stäng fliken/fönstret för e-postredigeraren.

   ![](assets/eight-1.png)

1. Välj ditt nya e-postmeddelande. Klicka på Godkänn under E-poståtgärder.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Steg 2: Skapa en smart kampanj {#step-create-a-smart-campaign}

1. Högerklicka på **Mitt program** och klicka på **Ny smart kampanj**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Ge** den smarta kampanjen namnet&quot;Automatisk svarskampanj&quot; och klicka på  **Skapa**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Gå till fliken **Smart lista**.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Vi konfigurerar kampanjen så att den körs när en person fyller i formuläret som du skapade på [**landningssidan med ett formulär**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

1. Hitta och dra utlösaren **Fyller i formulär** till den vänstra arbetsytan.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Välj **Mitt formulär** i listrutan. Klicka på fliken **Flöde**.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Dra flödesåtgärden **Skicka e-post** till den vänstra arbetsytan.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Välj din **e-postadress för automatiskt svar** och gå till fliken **Schemalägg**.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Klicka på **Redigera**.

   ![](assets/8.png)

1. Välj **varje gång** och klicka på **Spara**.

   ![](assets/9.png)

1. Klicka på **Aktivera**.

   ![](assets/10.png)

1. Klicka på **Aktivera** på bekräftelseskärmen.

   ![](assets/11.png)

>[!NOTE]
>
>När kampanjen är aktiv körs den varje gång en person fyller i det angivna formuläret. Kampanjen fortsätter att löpa tills den har inaktiverats.

## Steg 3: Fyll i formuläret {#step-fill-out-the-form}

1. Välj **Min sida**. Detta skapades på [landningssidan med en snabb vinst i form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Klicka på **Visa godkänd sida**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Landningssidan&quot;Prova utan kostnad&quot; öppnas på en ny flik.

1. Fyll i formuläret med ditt förnamn, efternamn och e-postadress och klicka sedan på **Skicka**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Se till att du använder din faktiska e-postadress så att du kan få e-postmeddelandet.

## Uppdraget är klart {#mission-complete}

Inom bara några minuter visas e-postmeddelandet om automatiskt svar i din inkorg. Bra jobbat!

<br> 

[◄ 3: Enkel poängsättning](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Uppdrag 5: Importera en lista med leads ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
