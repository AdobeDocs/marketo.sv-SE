---
description: Överför ett Adobe Experience Cloud-segment till en Marketo Static List - Marketo Docs - Product Documentation
title: Överför ett Adobe Experience Cloud-segment till en Marketo Static List
hidefromtoc: true
source-git-commit: f437495fbe004177f01c57729d97d2fec1f79509
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Överför ett Adobe Experience Cloud-segment till en Marketo Static List {#push-an-adobe-experience-cloud-segment-to-a-marketo-static-list}

Med den här funktionen kan du överföra segment som finns i din Adobe Experience Platform till Marketo i form av en statisk lista.

>[!PREREQUISITES]
>
>* [Skapa en API-](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) användare i Marketo.
>* Gå sedan till **Admin** > **Startpunkt**. Leta reda på namnet på den roll du just skapade och klicka på **Visa detaljer**. Kopiera och spara informationen i **Klient-ID** och **Klienthemlighet** så som du behöver den för den här funktionen.


1. Logga in på [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-1.png)

1. Klicka på rutnätsikonen och välj **Experience Platform**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-2.png)

1. Klicka på **Destinationer** i det vänstra nav.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-3.png)

1. Klicka på **Katalog**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-4.png)

1. Hitta plattan Marketo Engage och klicka på **Aktivera**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-5.png)

1. Klicka på alternativknappen **Nytt konto** under Kontotyp. Ange dina Marketo-inloggningsuppgifter och klicka på **Anslut till mål**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >Du kan hitta ditt Munchkin-ID genom att gå till **Admin** > **Munchkin** (det är också en del av din Marketo-URL när du har loggat in). Klient-ID/hemlighet som du bör ha från att följa de krav som anges högst upp i den här artikeln.

1. &quot;Ansluten&quot; ska visas under dina autentiseringsuppgifter. Klicka på **Nästa** i det övre högra hörnet.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-7.png)

1. Ange ett **namn** och en _valfri_ beskrivning. Klicka på **Skapa mål**.

   >[!NOTE]
   >
   >Det är också valfritt att välja något från Marknadsföringsåtgärder. Marketo utnyttjar inte den informationen just nu, men kommer troligen snart.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-8.png)

1. Klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-9.png)

1. Välj önskat segment och klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >Segmenten i statiska listor är 1:1. Om du väljer flera segment här måste du mappa varje segment till en angiven statisk lista på fliken Segmentschema.

1. Klicka på **Lägg till ny mappning**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-11.png)

1. Klicka på markörikonen.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-12.png)

1. Välj det relevanta fält som innehåller den e-postadress som identifierar användaren. Klicka på **Välj** när du är klar.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-13.png)

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-14.png)


   >[!NOTE]
   >
   >Exemplet som vi har valt kan se mycket annorlunda ut än det du valt.

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-15.png)

1. Välj målfält och klicka på **Välj**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-16.png)

1. Klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-17.png)

1. _Skapa en statisk lista i Marketo_ eller sök efter och välj en som du redan har skapat. Kopiera mappnings-ID:t från slutet av URL:en.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-18.png)

   >[!NOTE]
   >
   >För bästa resultat bör du se till att den lista du refererar till i Marketo är tom.

1. I Adobe Experience Platform anger du det ID du just kopierade. Välj startdatum. Människor synkroniseras kontinuerligt till det valda slutdatumet. Lämna slutdatumet tomt om du vill synkronisera oändligt. Klicka på **Nästa** när du är klar.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-19.png)

1. Bekräfta ändringarna och klicka på **Slutför**.

   ![](assets/push-an-adobe-experience-cloud-segment-to-a-marketo-static-list-20.png)
