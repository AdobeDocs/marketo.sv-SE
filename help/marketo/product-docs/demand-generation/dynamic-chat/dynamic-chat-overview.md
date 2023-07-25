---
description: Dynamic Chat Overview - Marketo Docs - Product Documentation
title: Dynamisk chattöversikt
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---

# Dynamisk chattöversikt {#dynamic-chat-overview}

Med Dynamic Chat kan ni utnyttja ett lättanvänt gränssnitt för att nå ut till både personer och konton på er webbplats. Samla in relevant innehåll som namn, kontaktinformation och fritext. Besökarna kan även boka möten med säljteamet. Dynamic Chat-aktivitet och engagemangsdata kan användas för att lägga till medlemmar i Marketo-program och aktivera flerkanalsaktiviteter.

>[!NOTE]
>
>Dynamic Chat håller på att gradvis släppas ut och har för närvarande begränsad tillgång. Den här sidan uppdateras med allmän tillgänglighetsinformation (GA) allt eftersom de blir tillgängliga.

>[!TIP]
>
>Besök [den här sidan](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) för att visa självstudiekurser om Dynamic Chat.

## Integreringar {#integrations}

En viktig komponent i Dynamic Chat är möjligheten att ha ett gränssnitt för Marketo-prenumerationer. För att kunna utnyttja den här integreringens fulla kapacitet måste du först initiera datasynkroniseringen. Beroende på storleken på din Marketo-databas kan det ta upp till 24 timmar för data för den första, [engångssynkronisering](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) för att slutföra.

Följande synkroniseras:

* Personfältdata
* Företagsfältdata
* Aktivitetsdata

## Dialogrutor {#dialogues}

Dialoger representerar ett enda chattengagemang. Se det som en behållare med allt du behöver för att få en engagerande chattdialog till webbplatsens besökare. I varje dialogruta kan du ange vilka sidor du vill att dialogrutan ska visas på, till vilka du vill att den ska visas samt innehållet och flödet för själva dialogrutan. Dessutom kan du hitta mätvärden för att se hur bra din dialog fungerar. [Läs mer om dialogrutor](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## Konfiguration {#configuration}

Anpassa utseendet på dina olika dialogrutor på fliken Konfiguration. Ändra typsnitt, färger, svarstid med mera! [Läs mer om konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## Kalender {#calendar}

Anslut Outlook- eller Gmail-kalendern för användning vid schemaläggning av möten i chattbot. [Läs mer om Kalender](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## Möten {#meetings}

Här ser du alla avtalade tider som har schemalagts av webbplatsbesökare via olika dialogrutor. [Läs mer om möten](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## Routning {#routing}

Här kan du se en lista över alla agenter som har kopplat samman sina kalendrar, i vilken ordning de presenteras för webbplatsens besökare och skapa anpassade routningsregler. [Läs mer om routning](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## Vanliga frågor {#faq}

**Kan jag installera Dynamic Chat var som helst på min företagswebbplats eller fungerar det bara på Marketo landningssidor?**

JavaScript-kodfragmentet Dynamic Chat kan installeras på alla webbplatser och på Marketo landningssidor.

**Hur länge lagras data för rapportering?**

90 dagar (se den fullständiga listan över gränser) [nedan](#limits-in-dynamic-chat)).

**Tillåter Dynamic Chat live-chatt?**

Nej, det använder bara förbestämda svar.

**Har Dynamic Chat stöd för andra språk än engelska?**

Ja. Dynamic Chat stöder följande språk: Franska, tyska, japanska, spanska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska. Läs mer i [avsnitt nedan](#changing-the-language).

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur kan jag rikta mig till anonyma människor?**

I dialogrutan måste du använda _Personens e-postadress är tom_ -attribut.

## Ändra språk {#changing-the-language}

Följ de här stegen för att ändra ditt Dynamic Chat-språk.

>[!IMPORTANT]
>
>Om du ändrar ditt språk på profilnivå ändras språket för _alla_ Experience Cloud, inte bara Dynamic Chat.

1. Klicka på inställningsikonen på ditt Experience Cloud-konto och välj **Inställningar**.

   ![](assets/dynamic-chat-overview-1.png)

1. Klicka på det aktuella språket under din e-postadress.

   ![](assets/dynamic-chat-overview-2.png)

1. Välj ditt nya språk (det andra språket är valfritt) och klicka på **Spara**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Det finns ett par dussin språk att välja bland, men Dynamic Chat stöder bara följande: Engelska, franska, tyska, japanska, spanska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska.

När du uppdaterar språket ändras allt i själva programmet utom orden som du har fyllt i personligen (t.ex. strömningssvar).

## Gränser i Dynamic Chat {#limits-in-dynamic-chat}

<table>
  <th>Parameter</th>
  <th>Beskrivning</th>
  <th>Gräns</th>
 <tr>
  <td>Totalt antal dialogrutor</td>
  <td>Antal dialogrutor (publicerade och utkast)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Totalt antal kalendrar</td>
  <td>Antal anslutna kalendrar</td>
  <td>25</td>
 </tr>
 <tr>
  <td>Totalt antal användare (administratörer och marknadsföringsanvändare)</td>
  <td>Antal kombinerade användare som tillåts per Dynamic Chat-instans</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Publicerade dialogrutor</td>
  <td>Antal publicerade dialogrutor som har sparats</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Mål-URL:er per dialogruta</td>
  <td>Antal mål-URL:er som kan läggas till i en enda dialogruta</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Attribut per dialogruta</td>
  <td>Antal attribut som kan läggas till i målgruppsvillkor för en enskild dialogruta</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Grupper</td>
  <td>Antal grupper som kan läggas till i en enda dialogruta</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Attribut per grupp</td>
  <td>Antal attribut som kan läggas till i en grupp</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Kort</td>
  <td>Antal kort som kan läggas till i arbetsytan per dialogruta</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Lagringsperiod för anonyma leaddata</td>
  <td>Hur länge information om ett anonymt lead utan något åtagande sparas</td>
  <td>90 dagar</td>
 </tr>
 <tr>
  <td>Lagringsperiod för målaktivitet</td>
  <td>Information om målaktivitet för tid behålls</td>
  <td>24 månader</td>
 </tr>
 <tr>
  <td>Lagringsperiod för dokumentaktivitet</td>
  <td>Hur länge dokumentaktivitetsdata sparas</td>
  <td>24 månader</td>
 </tr>
 <tr>
  <td>Interaktion med kvarhållningsperiod för dialogaktivitet</td>
  <td>Den tid som interagerats med dialogaktivitetsdata behålls</td>
  <td>90 dagar</td>
 </tr>
 <tr>
  <td>Bevarandeperiod för mötesbokningsaktivitet</td>
  <td>Den tid som mötesbokningen ska sparas i Dynamic Chat</td>
  <td>24 månader</td>
 </tr>
 <tr>
  <td>Engagerade konversationer</td>
  <td>Antal chattkonversationer som webbesökare kan interagera med per månad</td>
  <td>250</td>
 </tr>
 <tr>
  <td>Konversationer utlösta</td>
  <td>Antal chattsamtal som kan visas för webbbesökare per månad</td>
  <td>25,000</td>
 </tr>
</table>
