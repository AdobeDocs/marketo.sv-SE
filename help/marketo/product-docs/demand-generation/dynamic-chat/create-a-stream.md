---
description: Skapa en ström - Marketo Docs - produktdokumentation
title: Skapa en ström
hide: true
hidefromtoc: true
source-git-commit: 1022d3eaf4ee4a1686c5d8ae3168ee0197776289
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Skapa en ström {#create-a-stream}

Det finns _många_ strömkombinationer som du kan skapa. Nedan visas ett exempel där marknadsföraren frågar besökaren om han eller hon har några produktfrågor. Om ja, kan besökaren boka ett möte. Om nej, ges besökaren möjlighet att ansluta sig till en sändlista för framtida korrespondens. Målet är antingen att schemalägga en avtalad tid eller att samla in besökarens e-post.

1. Efter [skapa en dialogruta](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue)klickar du på **Stream Designer** -fliken.

   ![](assets/create-a-stream-1.png)

1. Dra och släpp frågekortet.

   ![](assets/create-a-stream-2.png)

1. Under Chatbot Response, skriv din fråga hur du vill.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke är som standard aktiverat, vilket innebär att den inledande frågan visas bredvid chattikonen utan att besökaren behöver klicka på den för att se den.

1. Ange dina användarsvar och klicka på **Spara**.

   ![](assets/create-a-stream-4.png)

1. För Ja vill vi schemalägga en avtalad tid, så under det alternativet drar du över schemaläggarkortet för avtalad tid.

   ![](assets/create-a-stream-5.png)

1. Klicka på i kolumnen till höger **Spara**.

   ![](assets/create-a-stream-6.png)

1. Eftersom det är ett mål drar du målkortet under schemaläggaren för avtalade tider.

   ![](assets/create-a-stream-7.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/create-a-stream-8.png)

1. För&quot;Nej&quot; vill vi se om de kommer att gå med i e-postlistan, så under det alternativet drar du över ett annat frågekort.

   ![](assets/create-a-stream-9.png)

1. Ange ditt svar och lägg till svarsalternativ för besökaren. Klicka **Spara** när det är klart.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Du kan lägga till fler svar genom att klicka på **Lägg till svar**.

1. Under svaret&quot;Ja&quot; drar du över Info Capture-kortet så att du kan samla in besökarens e-post.

   ![](assets/create-a-stream-11.png)

1. Klicka på **Typ** nedrullningsbar meny och välj **E-post**.

   ![](assets/create-a-stream-12.png)

1. Ange ett chattbot-meddelande och en platshållare. Kontrollera att attributet är mappat till rätt fält i Marketo och klicka på **Spara**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Typ</strong></td>
     <td>Vilken typ av information du vill hämta: Telefon, Text, E-post.</td>
    </tr>
    <tr>
     <td><strong>Chatbot-meddelande</strong></td>
     <td>Det meddelande besökaren ser där han/hon uppmanas att ange informationen.</td>
    </tr>
    <tr>
     <td><strong>Platshållare</strong></td>
     <td>Exempeltext som hjälper besökaren att se vad han/hon ska ange.</td>
    </tr>
    <tr>
     <td><strong>Mappa svar till attribut</strong></td>
     <td>Gör att du kan synkronisera besökarens svar till motsvarande fält i personposten i din Marketo-prenumeration.</td>
    </tr>
   </table>

1. Eftersom det är ett mål att samla in deras e-post drar du målkortet under Info Capture.

   ![](assets/create-a-stream-14.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/create-a-stream-15.png)

1. Kom ihåg att lägga till ett svar om de säger&quot;Nej&quot;. Dra ett meddelandekort under det alternativet.

   ![](assets/create-a-stream-16.png)

1. Skriv ditt meddelande och klicka på **Spara**.

   ![](assets/create-a-stream-17.png)

1. När du vill aktivera dialogrutan klickar du på **Publicera**.

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>Innan du klickar på Publicera bör du kontrollera att [angett mål-URL:er](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[Dialogrutor](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
