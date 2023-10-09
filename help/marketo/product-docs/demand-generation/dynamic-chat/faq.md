---
description: Dynamic Chat FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om Dynamic Chat
feature: Dynamic Chat
source-git-commit: c4a02e1c365da6c56c94b119650e2c366cdc6641
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Vanliga frågor om Dynamic Chat {#dynamic-chat-faq}

Nedan finns svar på några vanliga frågor om Dynamic Chat.

**Kan jag installera Dynamic Chat var som helst på min företagswebbplats eller fungerar det bara på Marketo landningssidor?**

JavaScript-kodfragmentet Dynamic Chat kan installeras på alla webbplatser och på Marketo landningssidor.

**Hur länge lagras data för rapportering?**

90 dagar. En fullständig lista över begränsningar/parametrar finns på Marketo Engage [Produktbeskrivningssida](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Har Dynamic Chat stöd för andra språk än engelska?**

Ja. Dynamic Chat stöder följande språk: franska, tyska, japanska, spanska, italienska, brasiliansk portugisiska, koreanska, förenklad kinesiska och traditionell kinesiska. Läs mer i [Ändra språk](#changing-the-language).

**Stöder du AI/NLP-funktioner?**

Vi stöder inte AI/NLP-funktioner.

**Hur kan jag rikta mig till anonyma människor?**

I dialogrutan måste du använda _Personens e-postadress är tom_ -attribut.

**Vad räknas som en engagerad konversation?**

En engagerad konversation inträffar så snart en besökare svarar på roboten i en dialogruta eller ett konversationsflöde. Om besökaren öppnar chattbot men inte svarar på roboten (t.ex. väljer ett svar eller skickar information) räknas det inte som ett engagemang.

**Vad händer om jag når min månadskvot?**

När du når din månadsvisa konversationsgräns kommer alla publicerade dialogrutor och konversationsflöden att sluta aktiveras tills du ökar din gräns eller din gräns återställs i början av nästa månad.

**Hur vet jag när jag närmar mig gränsen för mitt deltagande i samtal?**

När du har nått 90 % av gränsen för antalet aktiva konversationer får Dynamic Chat-administratörer ett e-postmeddelande och alla användare ser ett banderollmeddelande i Dynamic Chat.

**Om en besökare interagerar med en dialog och sedan ansluter till en Live-agent, räknas det som ett eller två engagemang?**

För kunder med Select-paketet räknas detta som två separata åtaganden - en för Dialog-interaktionen och en för live-chattinteraktionen. För kunder med Prime-paketet räknas inte live-chattengagemang separat, så detta räknas bara som ett engagemang.

**Hur ofta återställs begränsningen för aktiverad konversation?**

Gränsen för aktiverad konversation återställs den första i varje kalendermånad.

**Varför kommer inte chattboten tillbaka efter jag har avslutat ett samtal?**

Dialogrutorna är avsedda att visas för en besökare endast en gång. Så när en besökare kommer till slutet av en viss gren i en dialogruta anses den dialogrutan vara fullständig och visas aldrig för besökaren igen.

**När jag klickar på rutan Dynamic Chat i Min Marketo och loggar in på Adobe Experience Cloud, varför får jag då följande meddelande? &quot;_Det verkar som att din Adobe ID inte är länkad till dina Adobe Experience Cloud-lösningskonton_.&quot;**

Detta innebär troligtvis att du inte har lagts till som Dynamic Chat i Adobe Admin Console. Kontakta antingen en systemadministratör för din Adobe-organisation eller en produktadministratör för Dynamic Chat för att begära åtkomst till Dynamic Chat.

**Hur får jag åtkomst till utskriften för en engagerad konversation?**

Dynamic Chat-transkript kan nås för alla kända leads som har interagerat med en Dynamic Chat-dialog via aktiviteten&quot;Engaged with Dialog&quot; i Marketo Engage.

**När en besökare deltar i en dialog, kan de då starta om konversationen eller gå tillbaka till en tidigare fråga?**

Det finns för närvarande inget systematiskt sätt att starta om en konversation eller gå tillbaka till en tidigare punkt, men detta är på Dynamic Chat färdplan.

**Kan Dynamic Chat integreras med Salesforce?**

Dynamic Chat integreras med Salesforce via Marketo Engage Salesforce-integreringen.

**Min kalender är uppkopplad i Dynamic Chat och jag ingår i routningsreglerna, så varför får jag inga möten?**

Detta tyder troligen på att din kalenderanslutning måste autentiseras på nytt. Det här inträffar oftast när du ändrar lösenordet för din kalenderleverantör och Dynamic Chat förlorar anslutningen. Du kan bara gå till sidan Agentinställningar i Dynamic Chat och klicka på &quot;Återautentisera kalender&quot;.

**Vad är skillnaden mellan en dialog och ett konversationsflöde?**

En dialogruta är en konversation som automatiskt visas för webbbesökare som uppfyller en definierad uppsättning målinriktningsvillkor. Ett konversationsflöde visas bara för besökare som utför en viss åtgärd på webben, till exempel trycker på en knapp.

**Kan jag använda Dynamic Chat utan Marketo Engage?**

Nej. Dynamic Chat är ett separat program från Marketo Engage, men de två är oupplösligt sammanlänkade.
