---
description: Dynamic Chat FAQ - Marketo Docs - produktdokumentation
title: DYNAMIC CHAT FAQ
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# DYNAMIC CHAT FAQ {#dynamic-chat-faq}

Nedan finns svar på några vanliga frågor om Dynamic Chat.

**Jag verkar inte ha tillgång till Dynamic Chat. Hur skaffar jag den?**

Kontakta din Marketo Engage-administratör och kontrollera att de har [lagt till dig som användare](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} i Adobe Admin Console.

**Kan jag installera Dynamic Chat var som helst på företagets webbplats eller fungerar det bara på Marketo landningssidor?**

Dynamic Chat JavaScript-fragmentet kan installeras på alla webbplatser och på Marketo landningssidor.

**Hur länge lagras data för rapportering?**

90 dagar. En fullständig lista över begränsningar/parametrar finns på Marketo Engage [produktbeskrivningssida](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Har Dynamic Chat stöd för andra språk än engelska?**

Ja. Dynamic Chat har stöd för följande språk: franska, spanska, tyska, japanska, nederländska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska. Läs mer i [Ändra språk](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur riktar jag mig till anonyma personer?**

I dialogrutan måste du använda attributet _Person-e-post är tomt_.

**Vad kvalificerar som en engagerad konversation?**

En engagerad konversation inträffar så snart en besökare svarar på roboten i en dialogruta eller ett konversationsflöde. Om besökaren öppnar chattbot men inte svarar på roboten (t.ex. väljer ett svar eller skickar information) räknas det inte som ett engagemang.

**Vad händer om jag når min månadsvisa konversationsgräns?**

När du når din månadsvisa konversationsgräns kommer alla publicerade dialogrutor och konversationsflöden att sluta aktiveras tills du ökar din gräns eller din gräns återställs i början av nästa månad.

**Hur vet jag när jag närmar mig gränsen för mitt deltagande samtal?**

När du har nått 90 % av gränsen för antalet aktiva konversationer får Dynamic Chat-administratörer ett e-postmeddelande och alla användare ser ett banderollmeddelande i Dynamic Chat.

**Om en besökare interagerar med en dialogruta och sedan ansluter till en Live-agent, räknas det som ett eller två engagemang?**

För kunder med Select-paketet räknas detta som två separata åtaganden - en för Dialog-interaktionen och en för live-chattinteraktionen. För kunder som har Prime-paketet räknas inte live-chattengagemang separat, så detta räknas bara som ett engagemang.

**Hur ofta återställs gränsen för deltagande konversationer?**

Gränsen för aktiverad konversation återställs den första i varje kalendermånad.

**Varför kommer inte chattbot tillbaka när jag har avslutat en konversation?**

Dialogrutorna är avsedda att visas för en besökare endast en gång. Så när en besökare kommer till slutet av en viss gren i en dialogruta anses den dialogrutan vara fullständig och visas aldrig för besökaren igen.

**När jag klickar på Dynamic Chat-rutan i Min Marketo och loggar in på Adobe Experience Cloud, varför får jag då följande meddelande? &quot;_Din Adobe ID verkar inte vara länkad till dina Adobe Experience Cloud-lösningskonton_.&quot;**

Detta innebär troligtvis att du inte har lagts till som Dynamic Chat-användare i Adobe Admin Console. Kontakta antingen en systemadministratör för din Adobe-organisation eller en produktadministratör för Dynamic Chat för att begära åtkomst till Dynamic Chat.

**Hur får jag åtkomst till utskriften för en engagerad konversation?**

Dynamic Chat-transkriberingar kan användas för alla kända leads som har deltagit i en Dynamic Chat-dialogruta via aktiviteten&quot;Engaged with Dialog&quot; i Marketo Engage och vars konversationsstatus är antingen&quot;Completed&quot; eller&quot;Dropped&quot;.

**När en besökare har anslutit till en dialogruta, kan de då starta om konversationen eller gå tillbaka till en tidigare fråga?**

Det finns för närvarande inget systematiskt sätt att starta om en konversation eller gå tillbaka till en tidigare punkt, men detta ligger på Dynamic Chat färdplan.

**Kan Dynamic Chat integreras med Salesforce?**

Dynamic Chat kan integreras med Salesforce via Marketo Engage Salesforce-integrering.

**Min kalender är ansluten i Dynamic Chat och jag ingår i routningsreglerna, så varför får jag inga möten?**

Detta tyder troligen på att din kalenderanslutning måste autentiseras på nytt. Detta inträffar oftast när du ändrar lösenordet för din kalenderleverantör och Dynamic Chat förlorar anslutningen. Du kan bara gå till sidan Agentinställningar i Dynamic Chat och klicka på &quot;Återautentisera kalender&quot;.

**Vad är skillnaden mellan en dialog och ett konversationsflöde?**

En dialogruta är en konversation som automatiskt visas för webbbesökare som uppfyller en definierad uppsättning målinriktningsvillkor. Ett konversationsflöde visas bara för besökare som utför en viss åtgärd på webben, till exempel trycker på en knapp.

**Finns det något sätt att använda Dynamic Chat för att boka möten direkt från ett e-postmeddelande?**

Ja! [Lär dig hur](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Vad betyder termer som &quot;Engaged&quot; eller &quot;People Acquired&quot; egentligen?**

Det finns flera termer som används i Dynamic Chat. Definitioner för många av dem finns i hjälpartiklar i respektive område.

* Analystermer som&quot;Personer som förvärvats&quot; [finns här](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}.
* Smart List-utlösare/filterdefinitioner [finns här](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}.
* Beskrivningar av de olika Stream Designer-korten [finns här](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}.

**Kan jag använda Dynamic Chat utan Marketo Engage?**

Nej. Även om Dynamic Chat är ett separat program från Marketo Engage är de två ofrånkomligen sammanlänkade.
