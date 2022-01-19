---
description: Push Clone - Marketo Docs - produktdokumentation
title: Skjut klon
hide: true
hidefromtoc: true
source-git-commit: 97015b31c9a20a3052526a39ed26fc9cf0097e82
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Skjut klon {#push-clone}

Med den här funktionen kan du överföra segment som finns i din Adobe Experience Platform till Marketo i form av en statisk lista.

>[!PREREQUISITES]
>
>* [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) i Marketo.
>* Gå sedan till **Administratör** > **Startpunkt**. Sök efter namnet på den roll du just skapade och klicka på **Visa detaljer**. Kopiera och spara informationen i **Klient-ID** och **Klienthemlighet** som du behöver för den här funktionen.
>* Skapa en statisk lista i Marketo eller sök efter och välj en som du redan har skapat. Du behöver dess ID.


1. Logga in på [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Klicka på rutnätsikonen och välj **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Klicka på **Destinationer**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Klicka **Katalog**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Hitta plattan Marketo Engage och klicka **Aktivera segment**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Klicka **Konfigurera nytt mål**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Under Kontotyp väljer du alternativknappen Befintligt eller Nytt konto (i det här exemplet väljer vi **Befintligt konto**). Klicka på ikonen Välj konto.

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

1. Välj målkonto och klicka på **Välj**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Ange ett mål **Namn** och en valfri beskrivning. Klicka på listrutan Skapa person och välj&quot;Matcha befintliga Marketo-personer och skapa saknade personer i Marketo&quot; _eller_ &quot;Matcha endast befintliga Marketo-användare.&quot; I det här exemplet väljer vi den första.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Om du väljer&quot;Matcha endast befintliga Marketo-användare&quot; behöver du bara mappa e-postmeddelandet och/eller ECID så att du kan hoppa över steg 13-16.

1. Det här avsnittet är valfritt. Klicka **Skapa** att hoppa över.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Markera målet som du skapade och klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Välj det segment som du vill skicka till Marketo och klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. Klicka **Lägg till ny mappning**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Mappa förnamn genom att markera **firstName** och klicka **Välj**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. Mappa efternamn och företagsnamn genom att klicka på **Lägg till ny mappning** och upprepa steg 15 två gånger genom att välja **lastName** och sedan **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Nu är det dags att mappa e-postadressen. Klicka **Lägg till ny mappning** igen.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Klicka på alternativknappen Välj identitetsnamnområde och välj  **E-post** och sedan klicka **Välj**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. Nu är det dags att välja källfälten. Klicka på markörikonen för e-post.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Klicka på alternativknappen Välj identitetsnamnutrymme, sök efter och markera **E-post** och sedan klicka **Välj**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Om du vill välja källfältet för företagsnamnet klickar du på markörikonen på raden.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Låt alternativknappen Välj attribut vara markerad. Sök efter&quot;företag&quot; och välj **companyName** och sedan klicka **Välj**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Mappa källfälten för Efternamn och Förnamn genom att klicka på markörikonen för varje och upprepa steg 23 två gånger. Välj **lastName** och sedan **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Klicka **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Du behöver nu din listas ID. Klicka på den flik i webbläsaren där Marketo statiska lista är öppen (eller öppna en ny flik och välj önskad statisk lista).

   ![](assets/push-an-adobe-experience-platform-segment-26.png)

1. Markera och kopiera list-ID:t i slutet av URL:en.

   ![](assets/push-an-adobe-experience-platform-segment-27.png)

1. Klistra in det ID du kopierade under Mappnings-ID och klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-28.png)

1. Klicka **Slutför**.

   ![](assets/push-an-adobe-experience-platform-segment-29.png)
