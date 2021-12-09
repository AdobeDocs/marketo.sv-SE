---
description: Dynamic Chat Overview - Marketo Docs - produktdokumentation
title: Dynamisk chattöversikt
hide: true
hidefromtoc: true
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Dynamisk chattöversikt {#dynamic-chat-overview}

Med Dynamic Chat kan ni utnyttja ett lättanvänt gränssnitt för att nå ut till både personer och konton på er webbplats. Samla in relevant innehåll som namn, kontaktinformation och fritext. Besökarna kan även boka möten med säljteamet. Dynamic Chat activity and engagement data can be used to add members to Marketo programs and trigger cross-channel activities.

>[!NOTE]
>
>Dynamic Chat is in the process of being rolled out gradually and is currently in limited availability. This page will be updated with general availability (GA) details as they become available.

## Integreringar {#integrations}

A key component of Dynamic Chat is its ability to natively interface with your Marketo subscription. In order to leverage the full capability of this integration, you’ll first need to initiate the data sync. Beroende på storleken på din Marketo-databas kan det ta upp till 24 timmar för data för den första, [engångssynkronisering](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) för att slutföra.

Följande synkroniseras:

* Personfältdata
* Företagsfältdata
* Aktivitetsdata

## Dialogrutor {#dialogues}

Dialoger representerar ett enda chattengagemang. Think of it as a container with all the stuff you need to have an engaging chat dialogue to your website visitors. I varje dialogruta kan du ange vilka sidor du vill att dialogrutan ska visas på, till vilka du vill att den ska visas samt innehållet och flödet för själva dialogrutan. Additionally, you can find metrics to see how well your Dialogue is performing. [Learn more about Dialogues](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configuration {#configuration}

Anpassa utseendet på dina olika dialogrutor på fliken Konfiguration. Ändra typsnitt, färger, svarstid med mera! [Learn more about Configuration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Kalender {#calendar}

Anslut din (Outlook eller Gmail) kalender på fliken Kalender för användning vid schemaläggning av möten i chattbot. När en användares kalender är ansluten till Dynamiskt chatt läggs den användaren till i kön och hans/hennes kalender blir tillgänglig för webbplatsbesökare att schemalägga avtalade tider på.

Du kan också anpassa innehållet i den inbjudan som skickas till besökaren när de schemalägger en avtalad tid i användarens kalender.

## Möten {#meetings}

Här ser du alla avtalade tider som har schemalagts av webbplatsbesökare via olika dialogrutor. Här hittar du e-postadressen till personen som bokade den avtalade tiden, vilken agent de bokade den avtalade tiden med, när den avtalade tiden ska äga rum och om mötet har ägt rum eller inte.

## Routing {#routing}

Här kan du se en lista över alla agenter som har kopplat samman sina kalendrar samt i vilken ordning de kommer att presenteras för webbplatsens besökare. Meetings go round robin style, so if you have five agents and agent three took the last meeting, agent four will get the next one, followed by agent five, then back to agent one.

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

Not at this time.
