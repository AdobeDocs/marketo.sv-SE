---
description: Push Clone - Marketo Docs - produktdokumentation
title: Skjut klon
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Skjut klon {#push-clone}

Med den här funktionen kan du överföra segment som finns i din Adobe Experience Platform till Marketo i form av en statisk lista.

>[!PREREQUISITES]
>
>* [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) i Marketo.
>* Gå sedan till **Administratör** > **Startpunkt**. Sök efter namnet på den roll du just skapade och klicka på **Visa detaljer**. Kopiera och spara informationen i **Klient-ID** och **Klienthemlighet** som du behöver för den här funktionen.


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

Därefter måste du välja om du bara vill matcha befintliga Marketo-användare eller matcha befintliga Marketo-användare och skapa de saknade i Marketo. Nedan finns avsnitt som visar hur du gör var och en av dem.

## Matcha befintliga Marketo-användare och skapa saknade personer i Marketo {#match-existing-marketo-people-create-missing-people}

Efter steg 1-8 ovan..

1. Ange ett mål **Namn** och en valfri beskrivning. Klicka på listrutan Skapa person och välj **Matcha befintliga Marketo-användare och skapa saknade personer i Marketo**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

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

1. Mappa efternamn och företagsnamn genom att klicka på **Lägg till ny mappning** och upprepa steg 7 två gånger, välj lastName och sedan companyName.

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

MORREEEE

## Matcha endast befintliga Marketo-användare {#match-existing-marketo-people-only}

>[!NOTE]
>
>Identiteter används för att söka efter matchningar i Marketo. Om en matchning hittas läggs personen till i den statiska listan. Om ingen matchning hittas tas dessa personer bort (d.v.s. de skapas inte i Marketo).

1. _I Marketo_, skapar en statisk lista eller söker efter och väljer en som du redan har skapat. Kopiera mappnings-ID:t från slutet av URL:en.

PICC

>[!NOTE]
>
>För bästa resultat bör du se till att den lista du refererar till i Marketo är tom.

1. I Adobe Experience Platform anger du det ID du just kopierade. Välj startdatum. Människor synkroniseras kontinuerligt till det valda slutdatumet. Lämna slutdatumet tomt om du vill synkronisera oändligt. Klicka **Nästa** när det är klart.

PICC

1. Bekräfta ändringarna och klicka på **Slutför**.

PICC
