---
description: Dynamic Chat Overview - Marketo Docs - produktdokumentation
title: Dynamisk chattöversikt
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Dynamisk chattöversikt {#dynamic-chat-overview}

Med Dynamic Chat kan ni utnyttja ett lättanvänt gränssnitt för att nå ut till både personer och konton på er webbplats. Samla in relevant innehåll som namn, kontaktinformation och fritext. Besökarna kan även boka möten med säljteamet. Dynamic Chat-aktivitet och engagemangsdata kan användas för att lägga till medlemmar i Marketo-program och aktivera flerkanalsaktiviteter.

>[!NOTE]
>
>Dynamic Chat håller på att lanseras gradvis och har för närvarande begränsad tillgänglighet. Den här sidan uppdateras med allmän tillgänglighetsinformation (GA) allt eftersom de blir tillgängliga.

>[!TIP]
>
>Besök [den här sidan](https://dcweb.z20.web.core.windows.net/) för att visa självstudiekurser och en inspelad demo av Dynamic Chat.

## Integreringar {#integrations}

En viktig komponent i Dynamic Chat är möjligheten att kunna interagera direkt med din Marketo-prenumeration. För att kunna utnyttja den här integreringens fulla kapacitet måste du först initiera datasynkroniseringen. Beroende på storleken på din Marketo-databas kan det ta upp till 24 timmar för data för den första, [engångssynkronisering](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) för att slutföra.

Följande synkroniseras:

* Personfältdata
* Företagsfältdata
* Aktivitetsdata

## Dialogrutor {#dialogues}

Dialoger representerar ett enda chattengagemang. Se det som en behållare med allt du behöver för att få en engagerande chattdialog till webbplatsens besökare. I varje dialogruta kan du ange vilka sidor du vill att dialogrutan ska visas på, till vilka du vill att den ska visas samt innehållet och flödet för själva dialogrutan. Dessutom kan du hitta mätvärden för att se hur bra din dialog fungerar. [Läs mer om dialogrutor](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

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

**Tillåter Dynamic Chat live-chatt?**

Nej, det använder bara förbestämda svar.

**Hur kan jag rikta mig till anonyma människor?**

I dialogrutan måste du använda _Personens e-postadress är tom_ -attribut.

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur länge lagras data för rapportering?**

90 dagar.

**Finns det några andra språk än engelska i Dynamic Chat?**

Inte just nu.
