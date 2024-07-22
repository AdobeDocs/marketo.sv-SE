---
unique-page-id: 2359416
description: Automatiskt svar via e-post - Marketo Docs - produktdokumentation
title: Automatiskt svar för e-post
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Automatiskt svar för e-post {#email-auto-response}

## Uppdrag: Skicka ett e-postmeddelande när en person fyller i ett formulär {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Konfigurera och lägg till en person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Landningssida med ett formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Steg 1: Skapa ett e-postmeddelande {#step-create-an-email}

1. Gå till området **[!UICONTROL Marketing Activities]**.

   ![](assets/email-auto-response-1.png)

1. Välj programmet på den vänstra menyn, klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL New Local Asset]**.

   ![](assets/email-auto-response-2.png)

1. Välj **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Ge e-postmeddelandet namnet&quot;Automatiskt svar e-post&quot;, välj en mall och klicka på **[!UICONTROL Create]**.

   ![](assets/email-auto-response-4.png)

   En e-postredigerare öppnas i ett nytt fönster eller på en ny flik. Om popup-fönster blockeras klickar du på **[!UICONTROL Edit Draft]** på resurssammanfattningssidan för att komma åt e-postmeddelandet.

1. Ange en ämnesrad och dubbelklicka sedan på det redigerbara området i e-postmeddelandet.

   ![](assets/email-auto-response-5.png)

   _En RTF-redigerare öppnas ovanpå e-postredigeraren._

1. Markera befintligt e-postinnehåll.

   ![](assets/email-auto-response-6.png)

1. Skriv ditt e-postinnehåll och klicka på **[!UICONTROL Save]**.

   ![](assets/email-auto-response-7.png)

1. Klicka på listrutan **[!UICONTROL Email Actions]** och välj **[!UICONTROL Approve and Close]**.

   ![](assets/email-auto-response-8.png)

## Steg 2: Skapa en smart kampanj {#step-create-a-smart-campaign}

1. Välj ditt program, klicka på listrutan **[!UICONTROL New]** och välj **[!UICONTROL New Smart Campaign]**.

   ![](assets/email-auto-response-9.png)

1. **Namnge** den smarta kampanjen&quot;Automatisk svarskampanj&quot; och klicka på **[!UICONTROL Create]**.

   ![](assets/email-auto-response-10.png)

1. Gå till fliken **[!UICONTROL Smart List]**.

   ![](assets/email-auto-response-11.png)

   Vi konfigurerar den här kampanjen så att den körs när en person fyller i formuläret som du skapade på [**landningssidan med ett formulär**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Hitta och dra **[!UICONTROL Fills Out Form]**-utlösaren till arbetsytan.

   ![](assets/email-auto-response-12.png)

1. Välj **[!UICONTROL My Form]** i listrutan. Klicka sedan på fliken **[!UICONTROL Flow]**.

   ![](assets/email-auto-response-13.png)

1. Dra flödesåtgärden **[!UICONTROL Send Email]** till den vänstra arbetsytan.

   ![](assets/email-auto-response-14.png)

1. Välj din **e-postadress för automatiskt svar**. Klicka sedan på fliken **[!UICONTROL Schedule]**.

   ![](assets/email-auto-response-15.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/email-auto-response-16.png)

1. Markera **[!UICONTROL every time]** och klicka på **[!UICONTROL Save]**.

   ![](assets/email-auto-response-17.png)

1. Klicka på **[!UICONTROL Activate]**.

   ![](assets/email-auto-response-18.png)

1. Klicka på **[!UICONTROL Activate]** på bekräftelseskärmen.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>När kampanjen är aktiv körs den varje gång en person fyller i det angivna formuläret. Kampanjen fortsätter att löpa tills den har inaktiverats.

## Steg 3: Fyll i formuläret {#step-fill-out-the-form}

1. Välj **Min sida** (den skapades i [landningssidan med ett snabbt Win-fönster för formulär](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}) och klicka på **[!UICONTROL Preview]**.

   ![](assets/email-auto-response-20.png)

   _Startsidan för&quot;kostnadsfri provversion&quot; öppnas på en ny flik._

1. Fyll i formuläret med ditt förnamn, efternamn och e-postadress och klicka sedan på **[!UICONTROL Submit]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Se till att du använder din faktiska e-postadress så att du kan få e-postmeddelandet.

## Uppdraget är slutfört {#mission-complete}

Inom bara några minuter visas e-postmeddelandet om automatiskt svar i din inkorg. Snyggt jobb!

<br> 

[◄ 3: Enkel poängsättning](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Mission 5: Importera en lista över människor ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
