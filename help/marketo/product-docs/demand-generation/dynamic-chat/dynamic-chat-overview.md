---
description: Dynamic Chat Overview - Marketo Docs - produktdokumentation
title: Dynamisk chattöversikt
hide: true
hidefromtoc: true
source-git-commit: fe4a4b89ee295d8e351587a5ac858806a83f1305
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Dynamisk chattöversikt {#dynamic-chat-overview}

Med Dynamic Chat kan du utnyttja ett lättanvänt gränssnitt för att rikta in dig på båda leads (PEOPLE?) och har sina konton (BESÖKER DITT?) webbplats. Samla in relevant innehåll som namn, kontaktinformation och fritext. Besökarna kan även boka möten med säljteamet. Dynamic Chat-aktivitet och engagemangsdata kan användas för att lägga till medlemmar i Marketo-program och aktivera flerkanalsaktiviteter.

>[!NOTE]
>
>Dynamic Chat håller på att lanseras gradvis, och alla prenumerationer ska ha tillgång till dem våren 2022. Kontakta din Customer Success Manager om du vill ha mer information.

## Integreringar {#integrations}

En viktig komponent i Dynamic Chat är möjligheten att kunna interagera direkt med din Marketo-prenumeration. För att kunna utnyttja den här integreringens fulla kapacitet måste du först initiera datasynkroniseringen. Beroende på storleken på din Marketo-databas kan det ta upp till 24 timmar innan den initiala [engångssynkroniseringen](/help/marketo/product-docs/demand-generation/dynamic-chat/access-dynamic-chat.md) har slutförts. Den genomsnittliga synkroniseringstiden är mindre än två timmar.

Följande synkroniseras:

* Fältdata för lead
* Företagsfältdata
* Aktivitetsdata

## Dialogrutor {#dialogues}

Dialoger representerar ett enda chattengagemang. Se det som en behållare med allt du behöver för att få en engagerande chattdialog till webbplatsens besökare. I varje dialogruta kan du ange vilka sidor du vill att dialogrutan ska visas på, till vilka du vill att den ska visas samt innehållet och flödet för själva dialogrutan. Dessutom kan du hitta mätvärden för att se hur bra din dialog fungerar. [Läs mer om dialogrutor](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Konfiguration {#configuration}

Anpassa utseendet på dina olika dialogrutor på fliken Konfiguration. Ändra typsnitt, färger, svarstid med mera! [Läs mer om konfiguration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Kalender {#calendar}

Anslut din (Outlook eller Gmail) kalender på fliken Kalender för användning vid schemaläggning av möten i chattbot. När en användares kalender är ansluten till Dynamiskt chatt läggs den användaren till i kön och hans/hennes kalender blir tillgänglig för webbplatsbesökare att schemalägga avtalade tider på.

Du kan också anpassa innehållet i inbjudan via e-post? som skickas till besökaren när de schemalägger en avtalad tid i användarens kalender.

## Möten {#meetings}

Här ser du alla avtalade tider som har schemalagts av webbplatsbesökare via olika dialogrutor. Här hittar du e-postadressen till den lead som bokade den avtalade tiden, vilken agent de bokade den avtalade tiden med, när den avtalade tiden ska äga rum och om mötet har ägt rum eller inte.

## Routning {#routing}

Här kan du se en lista över alla agenter som har kopplat samman sina kalendrar samt i vilken ordning de kommer att presenteras för webbplatsbesökare. Om du har fem agenter och agent tre som deltog i det senaste mötet får agent 4 nästa, följt av fem, och sedan tillbaka till agent ett.

## Vanliga frågor {#faq}

**Tillåter Dynamic Chat live-chatt?**

Nej, det använder bara förbestämda svar.

**Hur kan jag rikta mig mot anonyma leads?**

I dialogrutan måste du använda attributet _Lead Email är Empty_.

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur länge lagras data för rapportering?**

90 dagar.

**Finns det några andra språk än engelska i Dynamic Chat?**

Inte just nu.
