---
description: Stream Designer - Marketo Docs - produktdokumentation
title: Stream Designer
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: b4ba55769034e8fb8a7878f52e21bd08e073fa8c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Stream Designer {#stream-designer}

Det finns _många_ möjliga kombinationer av strömmar. Den här artikeln innehåller ett exempel där marknadsföraren frågar besökaren om han eller hon har några produktfrågor. Om ja, kan besökaren boka ett möte. Om nej, ges besökaren möjlighet att ansluta sig till en sändlista för framtida korrespondens. De erbjuds också en kostnadsfri PDF. Det slutliga målet är antingen att schemalägga en avtalad tid eller att samla in besökarens e-post.

>[!PREREQUISITES]
>
>Innan du kan använda dokumentkortet måste du [konfigurera](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} på ditt Adobe-konto.

## Stream Designer-kort {#stream-designer-cards}

Strömdesignern innehåller flera kort som du kan lägga till för att forma chattkonversationen.

<table>
 <tr>
  <td><strong>Meddelande</strong></td>
  <td>Använd det här alternativet om du vill göra en programsats utan något svar (t.ex. "Hi! Alla artiklar är 25 % rabatt idag med koden SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Fråga</strong></td>
  <td>Använd detta när du vill ställa en flervalsfråga, där du kan ge tillgängliga svar (t.ex. vilken typ av fordon är du intresserad av? Svar = SUV, Compact, Truck osv.).</td>
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
  <td>Det här är det enda kortet som besökarna inte ser. Det är upp till dig att avgöra vid vilken punkt ett mål uppnås i den specifika chatten (t.ex. om du vill samla in besökarens e-postadress placerar du målkortet omedelbart efter Info Capture i strömmen).</td>
 </tr>
 <tr>
  <td><strong>Åtgärd</strong></td>
  <td>På liknande sätt som med dolda fält i ett formulär kan du med åtgärdskortet fylla i alla lead- eller företagsattribut med implicita värden som du vill hämta mot en lead-post. Du kan lägga till åtgärdskortet när som helst i konversationen och uppdatera respektive attribut med ett värde eller inbyggda tokens som automatiskt fyller i respektive värde.</td>
 </tr>
 <tr>
  <td><strong>Live Chatt</strong></td>
  <td>Använd chattkortet när du vill att besökarna ska chatta med en live-agent.
  <li>Direktchattkortet måste vara det sista kortet i grenen</li>
  <li>Besökarna dirigeras till en agent så snart de kommer till det här kortet i strömmen, så vi rekommenderar att du före det här kortet tillfrågar besökarna ett frågekort om de vill chatta med en handläggare</li></td>
 </tr>
</table>

## Stream Designer-ikoner {#stream-designer-icons}

I det övre högra hörnet av Stream Designer visas en handfull ikoner. Så här gör de.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Lägger till ett rutnät i bakgrunden för dem som föredrar den vyn</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Zoomar in, skapar större kort</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Zoomar ut, skapa mindre kort</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Öppnar ett fönster där du kan testa chatten (tryck på samma knapp för att stänga)</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Ordnar alla kort i strömmen</td>
 </tr>
</table>

## Skapa en ström {#create-a-stream}

1. Efter att du [skapade dialogrutan](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}klickar du på **Stream Designer** -fliken.

   ![](assets/stream-designer-6.png)

1. Dra och släpp frågekortet.

   ![](assets/stream-designer-7.png)

1. Under Chatbot Response, skriv din fråga hur du vill.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Du kan personalisera upplevelsen för kända chattbesökare genom att använda variabler (t.ex. Hello `{{lead.leadFirstName:""}}`). Klicka bara på klammerparentesen till höger och gör ditt val. Lägg till ett standardvärde mellan offerterna om du vill att anonyma besökare ska se något generiskt (t.ex. Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Poke är som standard aktiverat, vilket innebär att den inledande frågan visas bredvid chattikonen utan att besökaren behöver klicka på den för att se den. Poke är bara tillgängligt på det första kortet i konversationen.

1. Ange dina användarsvar och klicka på **Spara**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Redigera lagrade värden** är ett valfritt steg för dem som vill lagra ett annat värde i databasen än vad som visas för besökare i chattbot för mappade attribut på frågekortet (t.ex.: besökaren ser &quot;Sökmotoroptimering&quot;, du lagrar värdet som &quot;SEO&quot;).

1. För Ja vill vi schemalägga en avtalad tid, så under det alternativet drar du över schemaläggarkortet för avtalad tid.

   ![](assets/stream-designer-10.png)

1. Klicka på i kolumnen till höger **Spara**.

   ![](assets/stream-designer-11.png)

1. Eftersom det är ett mål drar du målkortet under schemaläggaren för avtalade tider.

   ![](assets/stream-designer-12.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/stream-designer-13.png)

1. För&quot;Nej&quot; vill vi se om de kommer att gå med i e-postlistan, så under det alternativet drar du över ett annat frågekort.

   ![](assets/stream-designer-14.png)

1. Ange ditt svar och lägg till svarsalternativ för besökaren. Klicka **Spara** när det är klart.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Du kan lägga till fler svar genom att klicka på **Lägg till svar**.

1. Under svaret&quot;Ja&quot; drar du över Info Capture-kortet så att du kan samla in besökarens e-post.

   ![](assets/stream-designer-16.png)

1. Klicka på **Typ** nedrullningsbar meny och välj **E-post**.

   ![](assets/stream-designer-17.png)

1. Ange ett chattbot-meddelande och en platshållare. Kontrollera att attributet är mappat till rätt fält i Marketo och klicka på **Spara**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>Typ</strong></td>
     <td>Den typ av information som du vill hämta: Telefon, Text, E-post.</td>
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

   ![](assets/stream-designer-19.png)

1. Namnge målet (eller välj ett befintligt) och klicka på **Spara**.

   ![](assets/stream-designer-20.png)

1. Kom ihåg att lägga till ett svar om de säger&quot;Nej&quot;. Ett alternativ är att dra ett meddelandekort nedan och säga&quot;Tack ändå&quot;. Men i det här exemplet ger vi dem ett kostnadsfritt PDF-dokument istället.

   ![](assets/stream-designer-21.png)

1. I det här exemplet skapar vi ett nytt dokument. Ge den ett namn, ange URL:en till PDF som du redan har en värdserver och klicka på **Spara**.

   ![](assets/stream-designer-22.png)

1. Välj **Förhandsgranska** om du vill förhandsgranska dialogrutan.

   ![](assets/stream-designer-23.png)

1. När du är klar att aktivera dialogrutan klickar du på **Publicera**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Innan du klickar på Publicera bör du kontrollera att [angett mål-URL:er](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Skapa en dialogruta](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Målgruppskriterier](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* [Rapporter](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [Använda dokumentkortet](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}

