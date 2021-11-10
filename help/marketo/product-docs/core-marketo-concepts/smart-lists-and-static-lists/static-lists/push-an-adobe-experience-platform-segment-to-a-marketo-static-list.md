---
description: Överför ett Adobe Experience Platform-segment till en Marketo Static List - Marketo Docs - Product Documentation
title: Överför ett Adobe Experience Platform-segment till en Marketo Static List
hidefromtoc: true
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: 8789ed464f532bbe76c2cb456374d9c0f505ece0
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Överför ett Adobe Experience Platform-segment till en Marketo Static List {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Med den här funktionen kan du överföra segment som finns i din Adobe Experience Platform till Marketo i form av en statisk lista.

>[!PREREQUISITES]
>
>* [Skapa en API-användare](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) i Marketo.
>* Gå sedan till **Administratör** > **Startpunkt**. Sök efter namnet på den roll du just skapade och klicka på **Visa detaljer**. Kopiera och spara informationen i **Klient-ID** och **Klienthemlighet** som du behöver för den här funktionen.


1. Logga in på [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-1.png)

1. Klicka på rutnätsikonen och välj **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-2.png)

1. Klicka på **Destinationer**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-3.png)

1. Klicka **Katalog**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-4.png)

1. Hitta plattan Marketo Engage och klicka **Aktivera segment**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-5.png)

1. Klicka **Konfigurera nytt mål**.

   PICC

1. Klicka på **Nytt konto** alternativknapp. Ange dina Marketo-uppgifter och klicka på **Anslut till mål**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-6.png)

   >[!NOTE]
   >
   >Du kan hitta ditt Munchkin-ID genom att gå till **Administratör** > **Munchkin** (den ingår också i din Marketo-URL när du har loggat in). Klient-ID/hemlighet som du bör ha från att följa de krav som anges högst upp i den här artikeln.

1. &quot;Ansluten&quot; ska visas under dina autentiseringsuppgifter. Klicka **Nästa** i det övre högra hörnet.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-7.png)

1. Ange **Namn** och _valfri_ Beskrivning. Klicka **Skapa mål**.

   >[!NOTE]
   >
   >Det är också valfritt att välja något från Marknadsföringsåtgärder. Marketo utnyttjar inte den informationen just nu, men kommer troligen snart.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-8.png)

1. Klicka **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-9.png)

1. Välj önskat segment och klicka på **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-10.png)

   >[!NOTE]
   >
   >Segmenten i statiska listor är 1:1. Om du väljer flera segment här måste du mappa varje segment till en angiven statisk lista på fliken Segmentschema.

1. Klicka **Lägg till ny mappning**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-11.png)

1. Klicka på markörikonen.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-12.png)

1. Välj antingen **Välj attribut** eller **Välj namnområde för identitet** alternativknapp (i det här exemplet väljer vi Attribut).

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-13.png)

   >[!NOTE]
   >
   >Om du valde **Välj namnområde för identitet** Gå till steg 15 när du har gjort ditt val.

1. Välj det relevanta fält som innehåller den e-postadress som identifierar användaren. Klicka **Välj** när det är klart.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-14.png)

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-15.png)

   >[!NOTE]
   >
   >Exemplet som vi har valt kan se mycket annorlunda ut än det du valt.

1. Klicka på mappningsikonen.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-16.png)

1. Välj **Välj namnområde för identitet**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-17.png)

   >[!IMPORTANT]
   >
   >Mappningsattribut är valfria. Mappa e-post och/eller ECID från **Identitetsnamnutrymme** -fliken är det viktigaste att göra för att säkerställa att personen matchas i Marketo. Mappning via e-post ger högsta matchningsfrekvens.

1. Välj mellan ECID och E-post. I det här exemplet väljer vi **E-post**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-18.png)

1. Klicka **Nästa**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-19.png)

   >[!NOTE]
   >
   >Identiteter används för att söka efter matchningar i Marketo. Om en matchning hittas läggs personen till i den statiska listan. Om ingen matchning hittas tas dessa personer bort (d.v.s. de skapas inte i Marketo).

1. _I Marketo_, skapar en statisk lista eller söker efter och väljer en som du redan har skapat. Kopiera mappnings-ID:t från slutet av URL:en.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-20.png)

   >[!NOTE]
   >
   >För bästa resultat bör du se till att den lista du refererar till i Marketo är tom.

1. I Adobe Experience Platform anger du det ID du just kopierade. Välj startdatum. Människor synkroniseras kontinuerligt till det valda slutdatumet. Lämna slutdatumet tomt om du vill synkronisera oändligt. Klicka **Nästa** när det är klart.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-21.png)

1. Bekräfta ändringarna och klicka på **Slutför**.

   ![](assets/push-an-adobe-experience-platform-segment-to-a-marketo-static-list-22.png)
