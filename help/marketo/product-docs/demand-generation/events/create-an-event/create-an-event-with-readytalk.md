---
unique-page-id: 2949870
description: Skapa en händelse med ReadyTalk - Marketo Docs - Produktdokumentation
title: Skapa en händelse med ReadyTalk
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Skapa en händelse med ReadyTalk {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [Lägg till ReadyTalk som en LaunchPoint-tjänst](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Ange lämpliga [flödesåtgärder](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)för att spåra engagemang


Konfigurera först ditt event i ReadyTalk konferenscenter. Om du behöver hjälp kan du gå till [ReadyTalk Resource Center](https://www.readytalk.com/resources/readytalk). När du väljer registreringstyp väljer du **förregistrera före mötet**. Om du väljer _registrera dig när du möts_ kommer Marketo **inte** att hämta en registrerad status för dina personer och kommer endast att hämta en personstatus som Attended _när_ webbinariet är avslutat.

Lämna **meddela mig om nya registreringar via e-post** avmarkerat.

![](assets/image2015-5-28-21-3a18-3a39.png)

Om du använder ReadyTalk för att skicka bekräftelsemeddelanden måste du också lägga till en beskrivning. Spara aktiviteten i ReadyTalk när du är klar.

>[!NOTE]
>
>Om du vill schemalägga en Operator Assisted Event-händelse klickar du på länken **Request Event Services** till vänster i hemskärmen för Conference Center för att schemalägga en händelse för vårt Events-team.

Nu kan du länka din aktivitet till Marketo.

1. Markera händelsen, klicka sedan på **Händelseåtgärder** och slutligen **Händelseinställningar.**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >Kanaltypen för den valda händelsen måste vara **webbinarium.**

1. Under **Event Partner,** väljer du **ReadyTalk**.

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. Under **Inloggning** väljer du din ReadyTalk-inloggning.

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. Under **Event** markerar du händelsen som du vill länka och klickar sedan på **Spara**.

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   Snyggt! Din aktivitet har synkroniserats.

   >[!NOTE]
   >
   >Fälten som Marketo skickar är: Förnamn, efternamn, e-postadress.

   >[!TIP]
   >
   >Om du vill fylla i bekräftelsemeddelandet med den här unika URL-adressen använder du följande token i e-postmeddelandet: `{{member.webinar url}}`. När bekräftelse-URL:en skickas, tolkas denna token automatiskt till personens unika bekräftelse-URL.
   >
   >Ange bekräftelsemeddelandet till Operational för att se till att personer som registrerar sig och som kan avbeställa tjänsten får sin bekräftelseinformation.

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge väljer du **Uppdatera från webbinariet Provider** på menyn Händelseåtgärder på fliken **Sammanfattning** för din händelse.

## Visa schemat {#viewing-the-schedule}

Klicka på kalenderposten för aktiviteten i programschemavyn. Schemat visas till höger på skärmen.

![](assets/image2015-5-18-12-9-58.png)

Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget Ändra programstatus när Ny status är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att du följer flödessteget Ändra programstatus 1 och Skicka e-postflöde 2.
