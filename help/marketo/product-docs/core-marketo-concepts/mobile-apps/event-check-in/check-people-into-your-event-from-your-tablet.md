---
unique-page-id: 2949839
description: Checka in personer i ditt event från din surfplatta - Marketo Docs - produktdokumentation
title: Checka in personer i din aktivitet från surfplattan
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Checka in personer i din aktivitet från surfplattan {#check-people-into-your-event-from-your-tablet}

När någon visas vid ditt evenemang hittar du deras information i appen. Efter incheckning befordras de till tillagd status när du synkroniserar till Marketo.

Programmet fungerar på samma sätt på både iPad och Android, förutom små skillnader i layout och design.

>[!PREREQUISITES]
>
>* Skapa ett event i Marketo och fyll i det med Inbjuden och Registrerad person.
>* Ladda ned appen för surfplattan för [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) eller [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)

## Checka in registrerade gäster {#check-in-registered-guests}

1. Tryck på appikonen på din iPad- eller Android-surfplatta.

1. Tryck **Inloggning** för att starta Marketo Event-appen.

   ![](assets/1.jpg)

1. Ange ditt användarnamn och lösenord för Marketo och klicka på **Inloggning**.

   >[!NOTE]
   >
   >Du måste ha en roll med åtkomst till databasen för att kunna se personer i appen.

1. Välj en **Händelse**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Endast händelseprogram (med undantag för webbinarier) som är schemalagda en vecka före och en vecka efter dagens datum visas.

1. På hemskärmen kan du bläddra efter registrerade gäster. Om du vill hitta en person i listan kan du:

   * Bläddra för att hitta ett namn
   * Ange ett namn i sökfältet
   * Hoppa till en viss inledande bokstav i efternamnet genom att trycka på den till höger om listan

   >[!NOTE]
   >
   >Processen är densamma på iPad och Android, men skärmarna skiljer sig åt och objekten kan finnas på olika platser. I den här artikeln finns iPad gränssnitt. Jämför Android-skärmen i det här avsnittet för referens.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Tryck på det valda namnet och tryck på personposten **Checka in**.

   ![](assets/img-0068-35-hands.png)

Gästen har nu statusen Attended och får en bock. Personposten uppdateras när du synkroniserar med Marketo. Den röda räknaren på knappen Synkronisera ökar för att visa antalet incheckningar sedan den senaste synkroniseringen med Marketo. Knappen Synkronisera ser annorlunda ut och finns på en annan plats för iPad och Android:

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Om en person är inbjuden men inte har registrerat sig kan du söka efter namnet genom att klicka på **Sök på servern**, precis nedanför sökrutan. Status för Inbjuden ändras till **Anmäld** för händelsen.

## Skapa en ny person på surfplattan {#create-a-new-person-on-the-tablet}

Du kan lägga till gäster som inte finns i din Marketo-databas manuellt. De checkas in automatiskt och läggs till i din databas när du synkroniserar med Marketo.

1. Klicka **Lägg till**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Fyll i så många grundläggande informationsfält du kan och tryck **Klar**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Du kan bara använda befintliga fält. Du kan inte skapa egna.

   >[!CAUTION]
   >
   >Dubbelkontrollera e-postadressen. Andra fält kan korrigeras senare, men e-postadressen är den primära metoden för att kontakta gästen.

Den nya personen registreras som incheckad till din händelse och läggs till i Marketo-databasen med statusen Attended (Bifogad) när du synkroniserar till Marketo.

## Invertera en incheckning {#reverse-a-check-in}

Om du checkade in en person av misstag _innan du synkroniserar med Marketo_ kan du vända på statusen för Bifogad.

1. Tryck på namnet i listan och tryck sedan på **Ångra**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Alla lagade!

## Redigera en personpost vid incheckning {#edit-a-person-record-at-check-in}

Du kan lägga till och ändra gästinformation direkt vid evenemanget!

1. Tryck på namnet i personlistan och tryck på **Redigera**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Redigera och lägga till information i fälten och tryck sedan på **Klar**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >I Android visas **Klar** knappen kan vara dold. Bläddra ned för att hitta den.

Informationen uppdateras när du synkroniserar appen med Marketo.

## Synkronisera appen med Marketo {#sync-the-app-with-marketo}

Appen Marketo Events fungerar oberoende tills du synkroniserar din aktivitet med Marketo Database igen. Det är bäst att synkronisera så snart som möjligt efter den sista incheckningen. Din surfplatta måste vara ansluten till Internet.

>[!CAUTION]
>
>När du har synkroniserat kan du inte återföra en incheckning från appen.

1. Öppna appen på surfplattan och navigera till din aktivitet.

1. Tryck **Synkronisera**.

   Din aktivitet uppdateras med nya incheckningar i Marketo-databasen. Den röda räknaren på knappen Synkronisera avmarkeras tills du checkar in någon annan.

   Av säkerhetsskäl bör du avsluta appen Marketo Events när du har synkroniserat klart.

## Arbeta med begränsad Internet-åtkomst {#working-with-limited-internet-access}

Vissa platser har dålig internetuppkoppling. Du behöver en bra anslutning till:

* Hämta och installera programmet
* Logga in
* Välj en händelse
* Synkronisera appen med Marketo

Om du är oroad över internetuppkoppling kan du logga in på Marketo Events-appen och välja ett evenemang i förväg på en plats med stark internetuppkoppling. På så sätt kan du fortfarande använda appen offline. När du sedan återfår en internetanslutning kan du synkronisera direkt till Marketo-databasen.

>[!TIP]
>
>Om du inte har någon internetanslutning kan du fortfarande skapa en ny person för att checka in en person. Den kommer att stämma av med den befintliga personen när du synkroniserar appen.

>[!NOTE]
>
>Appen loggar automatiskt ut dig efter åtta timmars inaktivitet.
