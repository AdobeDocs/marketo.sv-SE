---
description: Stream Designer - Marketo Docs - produktdokumentation
title: Stream Designer
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: f08484455baaf073bb42ae8a62a9dcc6fc7fd48f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Stream Designer {#stream-designer}

Det finns _många_ möjliga kombinationer av strömmar. Den här artikeln innehåller ett exempel där marknadsföraren frågar besökaren om han eller hon har några produktfrågor. Om ja, kan besökaren boka ett möte. Om nej, ges besökaren möjlighet att ansluta sig till en sändlista för framtida korrespondens. De erbjuds också en kostnadsfri PDF. Det slutliga målet är antingen att schemalägga ett möte eller att samla in besökarens e-post.

>[!PREREQUISITES]
>
>Innan du kan använda dokumentkortet måste du först [konfigurera](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/using-the-document-card.md){target=&quot;_blank&quot;} i ditt Adobe-konto.

## Stream Designer-kort {#stream-designer-cards}

Strömdesignern innehåller flera kort som du kan lägga till för att forma chattkonversationen.

<table>
 <tr>
  <td><strong>Meddelande</strong></td>
  <td>Använd när du vill göra en -programsats utan något svar (t.ex.: "Hej! Alla artiklar är 25 % rabatt idag med koden SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Fråga</strong></td>
  <td>Använd det här alternativet om du vill ställa en flervalsfråga, där du anger tillgängliga svar (t.ex.: Vilken typ av fordon är du intresserad av? Svar = SUV, Compact, Truck osv.).</td>
 </tr>
 <tr>
  <td><strong>Dokument</strong></td>
  <td>Gör att du kan bädda in PDF-dokument i dialogrutor och spåra besökares engagemang i dokument (hur många sidor som visades, om dokumentet hämtades och/eller eventuella söktermer som användes).</td>
 </tr>
 <tr>
  <td><strong>Information Capture</strong></td>
  <td>Använd när du vill samla in information. De tre fälten som ska väljas är E-postadress, Telefonnummer och Text (som gör att besökaren kan skriva sitt eget meddelande).</td>
 </tr>
 <tr>
  <td><strong>Schemaläggare för avtalad tid</strong></td>
  <td>Ger besökaren en kalender med tillgängliga datum för att schemalägga en uppföljning. Kalendertillgängligheten återspeglar <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">nästa anställd i rad</a>.</td>
 </tr>
 <tr>
  <td><strong>Mål</strong></td>
  <td>Det här är det enda kortet som besökarna inte ser. Det är upp till dig att avgöra vid vilken punkt ett mål uppnås i den specifika chatten (t.ex.: om du vill samla in besökarens e-postadress placerar du målkortet omedelbart efter Info Capture i strömmen).</td>
 </tr>
</table>

## Skapa en ström {#create-a-stream}

1. Efter att du [skapade dialogrutan](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}, klicka på **Stream Designer** -fliken.

   ![](assets/stream-designer-1.png)

1. Dra och släpp frågekortet.

   ![](assets/stream-designer-2.png)

1. Under Chatbot Response, skriv din fråga hur du vill.

   ![](assets/stream-designer-3.png)

   >[!NOTE]
   >
   >Poke är som standard aktiverat, vilket innebär att den inledande frågan visas bredvid chattikonen utan att besökaren behöver klicka på den för att se den. Poke är bara tillgängligt på det första kortet i konversationen.

1. Ange dina användarsvar och klicka på **Spara**.

   ![](assets/stream-designer-4.png)

   >[!NOTE]
   >
   >**Redigera lagrade värden** är ett valfritt steg för dem som vill lagra ett annat värde i databasen än vad som visas för besökare i chattbot för mappade attribut i frågekortet (t.ex.: besökaren ser&quot;Sökmotoroptimering&quot;, du lagrar värdet som&quot;SEO&quot;.)

1. För Ja vill vi schemalägga en avtalad tid, så under det alternativet drar du över schemaläggarkortet för avtalad tid.

   ![](assets/stream-designer-5.png)

1. Klicka på i kolumnen till höger **Spara**.

   ![](assets/stream-designer-6.png)

1. Eftersom det är ett mål drar du målkortet under schemaläggaren för avtalade tider.

   ![](assets/stream-designer-7.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/stream-designer-8.png)

1. För&quot;Nej&quot; vill vi se om de kommer att gå med i e-postlistan, så under det alternativet drar du över ett annat frågekort.

   ![](assets/stream-designer-9.png)

1. Ange ditt svar och lägg till svarsalternativ för besökaren. Klicka **Spara** när det är klart.

   ![](assets/stream-designer-10.png)

   >[!NOTE]
   >
   >Du kan lägga till fler svar genom att klicka på **Lägg till svar**.

1. Under svaret&quot;Ja&quot; drar du över Info Capture-kortet så att du kan samla in besökarens e-post.

   ![](assets/stream-designer-11.png)

1. Klicka på **Typ** nedrullningsbar meny och välj **E-post**.

   ![](assets/stream-designer-12.png)

1. Ange ett chattbot-meddelande och en platshållare. Kontrollera att attributet är mappat till rätt fält i Marketo och klicka på **Spara**.

   ![](assets/stream-designer-13.png)

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

   ![](assets/stream-designer-14.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/stream-designer-15.png)

1. Kom ihåg att lägga till ett svar om de säger&quot;Nej&quot;. Ett alternativ är att dra ett meddelandekort nedan och säga&quot;Tack ändå&quot;. Men i det här exemplet ger vi dem ett kostnadsfritt PDF-dokument istället.

   ![](assets/stream-designer-16.png)

1. I det här exemplet skapar vi ett nytt dokument. Ge den ett namn, ange URL:en till PDF som du redan har en värdserver och klicka på **Spara**.

   ![](assets/stream-designer-17.png)

1. Välj **Förhandsgranska** om du vill förhandsgranska dialogrutan.

   ![](assets/stream-designer-18.png)

1. När du är klar att aktivera dialogrutan klickar du på **Publicera**.

   ![](assets/stream-designer-19.png)

>[!NOTE]
>
>Innan du klickar på Publicera bör du kontrollera att [angett mål-URL:er](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}.

>[!MORELIKETHIS]
>
>* [Skapa en dialogruta](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Målgruppskriterier](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [Rapporter](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}
>* [Använda dokumentkortet](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/using-the-document-card.md){target=&quot;_blank&quot;}

