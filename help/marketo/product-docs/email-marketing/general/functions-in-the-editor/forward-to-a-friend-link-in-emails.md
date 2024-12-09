---
unique-page-id: 1900581
description: Vidarebefordra till en vän-länk i e-postmeddelanden - Marketo Docs - produktdokumentation
title: Vidarebefordra till en länk i e-postmeddelanden
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Vidarebefordra till en länk i e-postmeddelanden {#forward-to-a-friend-link-in-emails}

Genom att lägga till länken Vidarebefordra till vän i dina e-postmeddelanden kan du spåra personer som har fått ett vidarebefordrat e-postmeddelande via den här länken och automatiskt lägga till dem som en ny person om de inte redan finns i databasen.

Exempel: Keith använder länken Vidarebefordra till vän för att vidarebefordra e-postmeddelandet till en okänd person, Mark. Mark läggs automatiskt till som en ny person, tilldelas sin egen cookie och hans e-post och webbaktiviteter länkas till honom. Men om Keith använder framåtknappen i sin e-postklient, så kommer Mark felaktigt att kodas som Keith och hans aktivitet loggas som Keith.

## Lägg till länken i en e-postmall {#add-the-link-to-an-email-template}

1. Gå till **Design Studio**.

   ![](assets/one-8.png)

1. Sök efter och välj den e-postmall som du vill lägga till länken i. Klicka på **Redigera utkast**.

   ![](assets/two-7.png)

1. Klistra in följande HTML-kod där du vill att länken &quot;Vidarebefordra till vän&quot; ska visas (om du behöver hjälp med den här delen kontaktar du webbutvecklaren):

   `<a href="{{system.forwardToFriendLink}}">Forward to Friend</a>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Du kan lägga till format i länken för att den ska se trevligare ut. Exempel:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Vi rekommenderar inte att du använder formatet **position:relative** i din e-postmall. Det kan skapa problem med placeringen och visningen av rutan Vidarebefordra till vän.

1. Klicka på **Förhandsgranska utkast** för att kontrollera att mallen ser ut som du vill ha den.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Kom ihåg att godkänna mallutkastet för att tillämpa ändringarna.

   Alla e-postmeddelanden som använder den mallen får nu länken Vidarebefordra till vän. När e-postmottagaren klickar på den hämtas de till en webbversion av e-postmeddelandet med rutan Vidarebefordra till en vän:

   ![](assets/f2afbox.png)

## Lägg till länken i ett enskilt e-postmeddelande {#add-the-link-to-an-individual-email}

Du kan också lägga till länken Vidarebefordra till vän direkt i ett e-postmeddelande.

1. Öppna det e-postmeddelande som du vill ta med länken i och dubbelklicka i det redigerbara området.

   ![](assets/five-4.png)

1. Placera markören där du vill att länken ska visas och klicka på knappen **Infoga token** .

   ![](assets/six-2.png)

1. Välj token **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Denna token är webbadressen för webbversionen av e-postmeddelandet med rutan Vidarebefordra till vän.

1. Skriv vad du vill att visningstexten för länken ska vara (till exempel &quot;Vidarebefordra till en vän&quot;).

   ![](assets/seven-1.png)

1. Klipp ut **`{{system.forwardToFriendLink}}`**-token med Ctrl+X (Windows) eller Cmd+X (Mac). Markera Vidarebefordra till en vän och klicka på knappen **Infoga/redigera länk** .

   ![](assets/eight-1.png)

1. Klistra in **`{{system.forwardToFriendLink}}`**-token i rutan **URL** med Ctrl/Cmd+V och klicka sedan på **Infoga**.

   ![](assets/nine.png)

1. Spara redigeringen och förhandsgranska den nya länken!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Nya personer som läggs till genom att ett e-postmeddelande om vidarebefordran till en vän tas emot, avbeställer som standard marknadsföringsmeddelanden.

## Visa vidarebefordringsaktivitet {#view-forwarding-activity}

Du kan se vem som vidarebefordrat och tagit emot e-postmeddelanden i personens aktivitetslogg.

1. Gå till **`Database`**.

   ![](assets/db.png)

1. Dubbelklicka på den person som du vill visa aktivitet för.

   ![](assets/fourteen.png)

1. Gå till fliken **Aktivitetslogg**. Dubbelklicka på **Mottaget till väns-e-post** eller **Skickat framåt till väns-e-post** för att visa information.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >För Mottaget vidarebefordrat till väns-e-post är person-ID den person som vidarebefordrade e-postmeddelandet.
   >
   >För Skickat Vidarebefordra till väns-e-post är person-ID den person som tog emot e-postmeddelandet.

   ![](assets/sixteen.png)

1. Om du vill visa en person efter ID kopierar och klistrar du in **person-ID** i slutet av URL:en (början av URL:en beror på din Marketo-instans):

   `...marketo.com/Database/loadPersonDetail?personId=`

   >[!NOTE]
   >
   >Vi gör **person-ID** klickbart och länkar direkt till personen i en kommande korrigering.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Om den vän som tar emot vidarebefordran är en okänd person, skapas en ny person med &quot;Vidarebefordra till vän&quot;, markerad som personens **Source**.
   >Om e-postmeddelandet är en lokal tillgång i ett program markeras programmet som personens **förvärvsprogram**.

## Utlös eller filtrera med hjälp av vidarebefordringsaktivitet {#trigger-or-filter-using-forwarding-activity}

Det finns sex utlösare/filter som du kan använda för att utlösa flödesåtgärder eller filtrera personer genom att skicka och ta emot aktiviteten Vidarebefordra till vän.

Om du söker efter &quot;framåt&quot; i en smart kampanjlista hittar du tillgängliga utlösare och filter.

![](assets/nineteen.png)

## Testa framåt till vän {#test-forward-to-friend}

Om du vill testa Vidarebefordra till vän skickar du dig ett e-postmeddelande med länken Framåt. Kontrollera att du skickar det genom flödessteget **Skicka e-post**, *inte* via **Skicka testmeddelande**.
