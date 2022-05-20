---
description: Dynamic Chat Overview - Marketo Docs - produktdokumentation
title: Dynamisk chattöversikt
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: ff34ef099f2af949602aa3220eb44e4494a6a7a9
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Dynamisk chattöversikt {#dynamic-chat-overview}

Med Dynamic Chat kan ni utnyttja ett lättanvänt gränssnitt för att nå ut till både personer och konton på er webbplats. Samla in relevant innehåll som namn, kontaktinformation och fritext. Besökarna kan även boka möten med säljteamet. Dynamic Chat-aktivitet och engagemangsdata kan användas för att lägga till medlemmar i Marketo-program och aktivera flerkanalsaktiviteter.

>[!NOTE]
>
>Dynamic Chat håller på att lanseras gradvis och har för närvarande begränsad tillgänglighet. Den här sidan uppdateras med allmän tillgänglighetsinformation (GA) allt eftersom de blir tillgängliga.

>[!TIP]
>
>Besök [den här sidan](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) för att visa självstudiekurser om Dynamic Chat.

## Integreringar {#integrations}

En viktig komponent i Dynamic Chat är möjligheten att kunna interagera direkt med din Marketo-prenumeration. För att kunna utnyttja den här integreringens fulla kapacitet måste du först initiera datasynkroniseringen. Beroende på storleken på din Marketo-databas kan det ta upp till 24 timmar för data för den första, [engångssynkronisering](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) för att slutföra.

Följande synkroniseras:

* Personfältdata
* Företagsfältdata
* Aktivitetsdata

## Dialogrutor {#dialogues}

Dialoger representerar ett enda chattengagemang. Se det som en behållare med allt du behöver för att få en engagerande chattdialog till webbplatsens besökare. I varje dialogruta kan du ange vilka sidor du vill att dialogrutan ska visas på, till vilka du vill att den ska visas samt innehållet och flödet för själva dialogrutan. Dessutom kan du hitta mätvärden för att se hur bra din dialog fungerar. [Läs mer om dialogrutor](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target=&quot;_blank&quot;}.

## Konfiguration {#configuration}

Anpassa utseendet på dina olika dialogrutor på fliken Konfiguration. Ändra typsnitt, färger, svarstid med mera! [Läs mer om konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Kalender {#calendar}

Anslut din (Outlook eller Gmail) kalender på fliken Kalender för användning vid schemaläggning av möten i chattbot. När en användares kalender är ansluten till Dynamiskt chatt läggs den användaren till i kön och hans/hennes kalender blir tillgänglig för webbplatsbesökare att schemalägga avtalade tider på.

Du kan också anpassa innehållet i den inbjudan som skickas till besökaren när de schemalägger en avtalad tid i användarens kalender.

## Möten {#meetings}

Här ser du alla avtalade tider som har schemalagts av webbplatsbesökare via olika dialogrutor. Här hittar du e-postadressen till personen som bokade den avtalade tiden, vilken agent de bokade den avtalade tiden med, när den avtalade tiden ska äga rum och om mötet har ägt rum eller inte.

## Routning {#routing}

Här kan du se en lista över alla agenter som har kopplat samman sina kalendrar samt i vilken ordning de kommer att presenteras för webbplatsens besökare. Möten blir till rån, så om du har fem agenter och agent tre tog det senaste mötet får agent 4 nästa, följt av agent fem och sedan tillbaka till agent ett.

## Vanliga frågor {#faq}

**Kan jag installera Dynamic Chat var som helst på företagets webbplats eller fungerar det bara på Marketo landningssidor?**

JavaScript-kodfragmentet Dynamic Chat kan installeras på alla webbplatser och på Marketo landningssidor.

**Hur länge lagras data för rapportering?**

90 dagar (se den fullständiga listan över gränser) [nedan](#limits-in-dynamic-chat)).

**Tillåter Dynamic Chat live-chatt?**

Nej, det använder bara förbestämda svar.

**Har Dynamic Chat stöd för andra språk än engelska?**

Ja. Dynamic Chat har stöd för följande språk: Franska, tyska, japanska, spanska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska. Läs mer i [avsnitt nedan](#changing-the-language).

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur kan jag rikta mig till anonyma människor?**

I dialogrutan måste du använda _Personens e-postadress är tom_ -attribut.

## Ändra språk {#changing-the-language}

Följ de här stegen för att ändra ditt dynamiska chattspråk.

1. Klicka på inställningsikonen på ditt Experience Cloud-konto och välj **Inställningar**.

   ![](assets/dynamic-chat-overview-1.png)

1. Klicka på det aktuella språket under din e-postadress.

   ![](assets/dynamic-chat-overview-2.png)

1. Välj ditt nya språk (det andra språket är valfritt) och klicka på **Spara**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!IMPORTANT]
   >
   >Det finns ett fåtal språk att välja bland, men Dynamic Chat har bara stöd för följande: Engelska, franska, tyska, japanska, spanska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska.

När du uppdaterar ditt språk ändras allt i själva programmet, förutom orden som du själv har fyllt i (t.ex. strömningssvar).

## Gränser i dynamiskt chatt {#limits-in-dynamic-chat}

<table>
  <th>Parameter</th>
  <th>Beskrivning</th>
  <th>Gräns</th>
 <tr>
  <td>Totalt antal dialogrutor</td>
  <td>Totalt antal dialogrutor (publicerade och utkast)</td>
  <td>500</td>
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
  <td>Den tid som mötesbokningsaktiviteten sparas i Dynamic Chat</td>
  <td>24 månader</td>
 </tr>
</table>
