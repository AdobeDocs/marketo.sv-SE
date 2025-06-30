---
description: Dynamic Chat versionsinformation – Marketo Docs – Produktdokumentation
title: Dynamic Chat versionsinformation
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 5dbc3add8acaae02f25c1f9b9ae39ecfc1aaf259
workflow-type: tm+mt
source-wordcount: '3408'
ht-degree: 1%

---

# Dynamic Chat versionsinformation {#dynamic-chat-release}

Adobe Dynamic Chat-releaser fungerar enligt en kontinuerlig leveransmodell som ger en mer skalbar metod för driftsättning av funktioner. Ibland finns det flera releaser på en månad, så var vänlig och kika regelbundet efter den senaste informationen.

Standardsidan för versionsinformation för Marketo Engage [finns här](/help/marketo/release-notes/current.md){target="_blank"}.

## Version från juni 2025 {#june-2025-release}

**Releasedatum: 30 juni 2025**

### Routing Logic Revamp {#routing-logic-revamp}

Vi har omarbetat logiken för live-chattroutning i Dynamic Chat för att säkerställa ett mer intelligent och förutsägbart engagemangsbeteende för alla routningstyper (konto, anpassad, team och Round Robin). Den nya logiken förenklar routningsflöden och förbättrar reservhanteringen när agenter inte är tillgängliga.

#### Viktiga förbättringar i routningsbeteende

* **Upp till två förlovningsförsök per session**

   * Systemet försöker ansluta med upp till två agenter (som mest), men strikt inom den primära routningsregeln.

   * Om en agent är tillgänglig men inte svarar (t.ex. avböjer eller missar chatten) försöker systemet ansluta till en annan agent från samma pool.

   * Reservlogik (som Round Robin) aktiveras bara om inga berättigade agenter hittas under den första upplösningen, inte för att försöka igen efter ett misslyckat engagemang.

* **Routningsregelspecifikt beteende**

##### —Kontoroutning—

Om en besökares e-postdomän mappar till ett känt konto prioriteras alltid den mappade agenten.

Om agenten är tillgänglig dirigeras chatten till dem direkt.

Om agenten inte är tillgänglig:

* Försöker inte med en annan agent, även om Round Robin är aktiverad som reserv.

* Istället:

   * Visar den mappade agentens möteskalender (om den är aktiverad),
-or-
   * Fallar tillbaka till ett standardmeddelande (värsta fall).

Routningsregeln på kortnivå (t.ex. Team, Custom) beaktas endast om Kontoroutning inte är giltig (ingen matchande domän eller agent).

##### —Custom/Team Routing—

Dessa regler kan returnera flera berättigade agenter.

Om den första tillgängliga agenten inte aktiveras kommer systemet att försöka med en till agent från samma lista.

Rund Robin-reservlösning utlöses inte bara för att en agent inte svarar.

Om ingen av agenterna engagerar:

* Systemet visar den första provade agentens kalender (om aktiverad),
-or-
* Visar standardfelmeddelandet.

##### —Round Robin Routing—

När det används som en primär routningsregel:

* Försöker att anlita den första tillgängliga agenten från poolen med resursallokering.

* Om den första agenten inte svarar försöker den igen med nästa bästa berättigade agent.

Om Round Robin används som reserv aktiveras den bara om inga agenter har lösts från den primära regeln.

##### Upplevelseflöde för besökare

Systemet kontrollerar om kontodirigering är relevant.

* Om ja och agent finns tillgänglig ansluter den omedelbart.

* Om agenten inte är berättigad eller inte är tillgänglig fortsätter den till routningsregeln på kortnivå.

Routningsregel på kortnivå (Custom, Team, Round Robin) utvärderas.

* Berättigade agenter kontrolleras för tillgänglighet (behörigheter, status).

* Systemet engagerar en agent och försöker vid behov att få en andra agent från samma regel.

* Om inget engagemang lyckas tillämpas reservlogik:

   * Kalenderreserv (om aktiverad),
-or-
   * Standardmeddelande.

Round Robin-reservlösningar beaktas endast när inga berättigade agenter hittas från den primära routningsregeln, inte när enskilda agenter inte svarar.

##### Användningsfall

<p>

_**Kontoroutning**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>Besökarens domänmappningar till ett konto. Den mappade agenten har live-chatt aktiverat och är tillgänglig</td>
    <td>Chatt ansluts direkt till den mappade agenten</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>Mappad agent är inte tillgänglig, Round Robin-reservfunktionen är aktiverad</td>
    <td>Systemet väljer en tillgänglig agent via Round Robin och engagerar dem </td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Den mappade agenten är inte tillgänglig, det finns ingen Round Robin-reserv. Mötesbokning är aktiverat</td>
    <td>Systemet visar den mappade agentens kalender eller visar ett standardreservmeddelande</td>
  </tr>
</tbody></table>

_**Anpassad routning**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>Anpassad logik löser en lista över agenter. Den första agenten är tillgänglig och accepterar chatt.</td>
    <td>Chatten ansluter till den första agenten.</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>Anpassad regel löser inga agenter. Round Robin-reservfunktionen är aktiverad.</td>
    <td>Systemet väljer en tillgänglig agent via Round Robin och engagerar dem.</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Två agenter har lösts. Ingen accepterar chatt, återgång har angetts till möteskalendern.</td>
    <td>Första testade agentens kalender visas eller standardåtergångsmeddelandet visas.</td>
  </tr>
</tbody></table>

_**Teamroutning**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>Teamet innehåller agenter med live-chatt. Den första tillgängliga agenten godkänner chatten.</td>
    <td>Chatten ansluter till den agenten.</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>Ingen teamagent är tillgänglig och Round Robin-reservfunktionen är aktiverad.</td>
    <td>Systemet väljer och ansluter med en agent från Round Robin-poolen.</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Två agenter är tillgängliga, men inget av dem, kalenderåtergång är aktiverat.</td>
    <td>Första provade agentens kalender visas eller så utlöses ett felmeddelande.</td>
  </tr>
</tbody></table>

_**Round Robin Routing**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>Round Robin-poolen har flera agenter. Den andra agenten accepterar chatt efter första steget.</td>
    <td>Chatten ansluter till den andra agenten.</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>Inga agenter är tillgängliga i Round Robin-poolen. Möteskalendern är aktiverad.</td>
    <td>Kalendern visas för den första agenten i listan (om den är konfigurerad), eller så visas ett felmeddelande.</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Inga tillgängliga agenter. Återställningen är inaktiverad.</td>
    <td>Statiskt reservmeddelande visas för besökaren.</td>
  </tr>
</tbody></table>

### Pulsmeddelande {#pulse-notification}

När en besökare begär att få ansluta till en agent skickar vi meddelanden i appen till agenten via webbläsaren. Men ibland saknar agenter dessa chattar.

Med den här versionen kan medarbetaren få e-post, Slack, meddelanden i appen och webbläsarmeddelanden när en ny besökare är intresserad av att chatta.

1. På din Adobe Experience Cloud-hemsida klickar du på kontoikonen och väljer **Inställningar**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Bläddra ned till _Meddelanden_ och gör de val du vill av Dynamic Chat.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Innehållet i ett Pulse-meddelande kan vara detsamma som det vi använder för meddelanden i appen och webbläsare.

## Version april/maj 2025 {#apr-may-25-release}

### Meddelandeljud {#message-notification-sound}

Nu kan du aktivera ett ljud för besökaren varje gång som chattbot aktiveras i en session. Det finns flera ljud att välja mellan.

### Aktivera Poke-meddelanden på mobilen {#enable-poke-messages-on-mobile}

&quot;Poke&quot;, som visar den inledande frågan bredvid chattikonen utan att besökaren behöver klicka på den för att se den, är nu ett alternativ att aktivera för besökare som använder en mobil enhet.

### Standarduppdatering för reserv {#default-fallback-update}

För anpassade regler/team som ett live-chattkort - om det inte finns några agenter tillgängliga (eller om chatten inte kan ansluta) återgår den till Round Robin för tillgängliga agenter (alla som är tillgängliga vid den tidpunkten oavsett vilken routningslogik/regel som placerades i strömmen).

### Demandbase-integrering {#demandbase-integration}

Demandbase-användare kan använda personattribut för Demandbase för dialog, villkorsstyrd varumärkesprofilering och anpassad routning i Dynamic Chat.

## September/oktober 2024-utgåvan {#sep-oct-release}

### Förbättrad chattanalys {#enhanced-live-chat-analytics}

Flera förbättringar har gjorts i kontrollpanelen för analyser, bland annat:

* Totalt antal begärda chattsamtal live: antal besökare som har begärt en chatt med agent

* Totalt antal anslutna live-chatt: antal anslutna besökare jämfört med totalt antal som har begärts för en&quot;chatt med agent&quot;

* Totalt antal missade chattförfrågningar: antal oövervakade besökare kontra totalt antal begärda för en&quot;chatt med agent&quot;

* Genomsnittlig chattlängd i minuter: analysera &quot;genomsnittlig chattlängd&quot; mellan besökare och agenter

* Genomsnittlig svarstid i sekunder för agenter: analysera&quot;genomsnittlig tid som agenter tar&quot; för att svara på frågor och svar om live-chatt

* Daglig instrumentpanel: live-chattförfrågningar anslutna, live-chattförfrågningar missade, sortera och filtrera nyligen använda live-chattaktiviteter

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Konversationsbedömning {#conversation-scoring}

Kvantifiera era leads baserat på kvaliteten på deras chattinteraktion och använd det måttet som utlösare/filter i Marketo Engage Smart Campaigns. Använd det nya attributet _konversationspoäng_ för följande aktiviteter:

* Engagerad med en dialogruta
* Engagerad med ett konversationsflöde
* Anställda hos en agent

**Saker att notera:**

* Poängvärdet är från 0, 1, 2, 3 (standardvärdet är null)

* När konversationen är klar eller tas bort går det inte att redigera poängvärdet

* Ställa in poäng:

   * I agentens inkorg - under en live-chatt kan agenten uppdatera eller ange ett poängvärde för konversationen, som lagras i konversationsaktiviteten

   * I strömdesignern - på målkortet, kan användaren uppdatera eller ange ett poängvärde för konversationen

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Ny logik för att skapa leads {#new-lead-creation-logic}

Om ett lead fyller i ett formulär med e-postadressen `abc@test.com` och cookies som xyz, fyller sedan i samma formulär med e-postadressen `def@test.com`, skapas en ny personpost, men cookie xyz kopplas till personen och tas bort från personen `abc@test.com`.

Så när en besökare med cookie abc kommer till en sida och anger ett e-post-ID som `abc@test.com`:

<table><thead>
  <tr>
    <th>Besökare</th>
    <th>Cookie</th>
    <th>E-postmeddelande</th>
    <th>Förväntat beteende</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonym</td>
    <td>abc</td>
    <td>Finns inte i databasen</td>
    <td>Skapa en ny person</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>abc</td>
    <td>Finns i databasen</td>
    <td>Sammanfoga person</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>xyz</td>
    <td>Finns i databasen</td>
    <td>Sammanfoga person</td>
  </tr>
  <tr>
    <td>Känd person</td>
    <td>abc</td>
    <td>Samma som befintlig person</td>
    <td>Uppdatera person</td>
  </tr>
  <tr>
    <td>Känd person</td>
    <td>abc</td>
    <td>Annat än befintlig person</td>
    <td>Om det redan finns en känd person överför du cookien och löser sedan den profilen. Om det inte finns någon person med det här e-postmeddelandet skapar du en ny personpost och överför cookien</td>
  </tr>
  <tr>
    <td>Känd person</td>
    <td>xyz</td>
    <td>Samma som befintlig person</td>
    <td>Lägg till ny cookie till samma person</td>
  </tr>
  <tr>
    <td>Känd person</td>
    <td>xyz</td>
    <td>Annat än befintlig person</td>
    <td>det här scenariot är inte möjligt som om det är en ny cookie från   standard betraktas som ny anonym profil</td>
  </tr>
</tbody></table>

### Möjlighet att ärva teckensnitt {#option-to-inherit-font}

Nu kan du aktivera chattbot för att direkt ärva teckensnittet från webbsidan där det ligger i stället för att hantera teckensnittet i Dynamic Chat. När du aktiverar det här alternativet får chattbot det teckensnitt som är definierat i taggen `<body>` på sidan.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Demandbase-integrering med Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Demandbase-användare kan hämta sin egen licens för Demandbase och aktivera integreringen. Använd personattribut för Demandbase för dialog, villkorsstyrd varumärkesprofilering och anpassad routning.

De här attributvärdena ska lösas mot en person i realtid och lagras i respektive personprofil.

### Optimerad inläsningstid för konversationsflöde {#optimized-conversation-flow-load-time}

För att förbättra användarupplevelsen visas nu en kortare inläsare i stället för ett tomt utrymme när konversationsflödet läses in.

**Före**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**Efter**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Version från augusti 2024 {#august-release}

**Releasedatum: 23 augusti 2024**

### Anpassa format för konversationsmeddelanden {#custom-format-conversation-messages}

Strömdesigners har nu stöd för [infogning av HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} för att anpassa konversationernas utseende och känsla.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Chatbot rullar längst ned {#chatbot-scroll-to-bottom}

En ikon har lagts till i chattbot så att webbbesökare kan gå direkt till det sista meddelandet. Detta hjälper besökare att bläddra igenom texten för att snabbt komma tillbaka till konversationen.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Meddelanden om kärnpuls {#core-pulse-notifications}

Användarna får nu ett [e-postmeddelande](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} när en mötesbokning eller live-chatt misslyckas.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Stöd för flera samtal {#support-for-multiple-conversations}

Chatbot stöder nu flera konversationer. Besökare på webbplatser kan engagera sig i olika konversationer på olika sidor samtidigt, med möjlighet att växla mellan dem.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Standardsortering av innehåll {#default-sorting-for-content}

Som standard sorteras dina konversationsloggar, obesvarade frågor och frågagenereringstabeller efter skapandedatum (från senaste till äldsta).

### Leadupplösning i realtid {#real-time-lead-resolution}

Under en konversation med ett anonymt lead och ett e-post-ID anges, löser vi om det finns en känd lead-post med det e-post-ID:t och använder posten för personalisering i realtid. Om vi hittar flera poster sammanfogar vi dem i realtid. Detta beteende implementeras för både dialogrutor och konversationsflöden.

### Synkronisera leads utan cookies från Marketo Engage {#syncing-leads-without-cookies}

Tidigare synkroniserades endast kända leads med ett eller flera cookie-ID från Marketo Engage när Marketo Engage-synkroniseringen aktiverades. Alla kända leads (cookie-ID finns eller inte) synkroniseras nu till Dynamic Chat och kan användas för personalisering av konversationer.

### Skicka ytterligare besöksdata till konversationsflöden {#pass-additional-visitor-data}

Om du hämtar besöksinformation via andra kanaler som formulär eller inloggning kan du nu skicka informationen direkt till Dynamic Chat.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Uppdaterade härledda data {#refreshed-inferred-data}

De flesta samtal på en webbplats pågår med anonyma besökare. Du kan fortfarande rikta in dem på slutna data, som är beroende av besökarnas IP-adresser. Vi har uppdaterat vår databas över IP-adresser och härledda data som nu stöder fyra gånger fler IP-adresser.

### Ljud har lagts till i agentwebbläsarmeddelanden {#sound-added-to-agent-browser-notification}

När en live-chatt tilldelas till en agent får de ett webbläsarmeddelande. Men ibland ser de inte dem. Vi har lagt till ett [meddelandeljud](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} för att förhindra att missade meddelanden går framåt.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Möjlighet att uppdatera lead-profilen under live-chatt {#update-lead-profile-during-live-chat}

Under en live-chatt vill agenter samla in information om besökaren och uppdatera respektive profil. Det finns nu ett alternativ för att uppdatera attributvärden för lead- och företagsobjekt.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version från juni 2024 {#june-release}

**Releasedatum: 6 juni 2024**

### Konversationsflödeskort {#conversational-flow-card}

Effektivisera flera steg i ett flöde i dialogrutorna genom att utnyttja Conversational Flow-kortet.

Exempel: Om ditt mål är att skapa registreringar för ditt webbinarium via flera dialogrutor måste du återskapa samma flöde för alla dialogrutor som har det målet. Och om du måste uppdatera någon detalj måste du redigera varje dialogruta en åt gången. Det är inte längre fallet, tack vare konversationsflödet.

Förutom att återanvända flöden mellan flera dialogrutor kan du även använda samma övergångsflöde för att utlösa via andra kanaler, som formulär och landningssidor.

![](assets/dynamic-chat-june-2024-release-1.png)

### Användningsgränser {#usage-limits}

På sidan Användningsbegränsningar visas viktig information, t.ex. paketinformation och status för din användningsgräns.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version från maj 2024 {#may-release}

**Releasedatum: 15 maj 2024**

### Förgodkänt svarsbibliotek {#pre-approved-response-library}

[Skapa ett marknadsföringsgodkänt bibliotek](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} med AI-genererade frågor och svar som hjälper dig att konfigurera generativ AI-chatt på några minuter.

![](assets/dynamic-chat-may-2024-release-1.png)

### Obesvarade frågor {#unanswered-questions}

[Använd en databas med obesvarade frågor](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} från tidigare konversationer för att generera nya förgodkända svar och underhålla ett svarsbibliotek med den senaste informationen.

![](assets/dynamic-chat-may-2024-release-2.png)

### Sammandrag {#conversation-summaries}

[Ge säljarna sammanfattade konversationer](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"} med insikter om viktiga diskussionsämnen före möten för att minska förberedelsetiden och ge säljarna bättre information.

![](assets/dynamic-chat-may-2024-release-3.png)

### GenAI-säljgenvägar {#genai-sales-shortcuts}

[Ge chattagenter snabbare sätt](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} att komma åt AI-genererade svar, redigera befintliga genererade svar och söka efter ytterligare innehåll att skicka till köpare under konversation.

![](assets/dynamic-chat-may-2024-release-4.png)

### Konversationsassistenten {#conversation-assist}

Hjälp säljarna att svara korrekt under live-samtal med svar som förgodkänts av ert marknadsföringsteam.

### Konversationsövningar {#conversation-nudges}

Knuffa webbbesökarna med en call-to-action för att slutföra konversationerna.

<p>

## Version från april 2024 {#april-release}

**Releasedatum: 23 april 2024**

### Konversationsflöden är nu tillgängliga för alla användare {#conversational-flows-available-to-all-users}

Gör formulären och landningssidorna mer konvergerande och korta säljprocessen genom att tillåta kvalificerade leads att boka ett möte eller chatta med försäljningen direkt efter att ett formulär har skickats in med Conversational Forms, nu helt tillgängligt&#42; för alla Dynamic Chat-användare.

_&#42;Tidigare tillgänglig som utvärderingsfunktion med 100 livstidsåtaganden. Konversationsflödesåtaganden räknas nu mot månadsgränsen på 250 aktiverade konversationer för användare i Select-paketet._

### Återanropsfunktioner {#callback-functions}

[Med återanropsfunktionerna](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} kan du samla in Dynamic Chat analyshändelser i externa system, som Adobe Analytics eller Google Analytics, när besökarna interagerar med Dynamic Chat-konversationer. Du aktiverar Dynamic Chat analyshändelser genom att registrera ett återanrop med API:t för att lyssna på händelserna. På så sätt kan ni få en helhetsbild av Dynamic Chat engagemang när det gäller andra nyckeldata, till exempel webbtrafik.

### Tillgänglighetsvillkor för Live-agent har lagts till i villkorlig förgrening {#live-agent-availability-conditional-branching}

Förutom inbyggda och anpassade Marketo Engage-fält kan du nu använda villkorlig förgreningslogik för att skapa förgreningar baserat på agentens tillgänglighet. Det här är användbart om du bara vill ge besökarna möjlighet att tala med en handläggare när det finns aktiva agenter tillgängliga.

![](assets/dynamic-chat-release-1.png)

### Villkoret Smart lista har lagts till i villkorlig förgrening {#smart-list-condition}

Med det nya villkoret Marketo Engage Smart List i villkorlig förgrening kan du skapa förgreningar baserat på befintliga målgrupper som du redan har skapat i Marketo Engage i stället för att definiera förgreningsvillkoren för målgrupper i Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Villkorliga förgreningar för konversationsflöden {#conditional-branching-for-conversational-flows}

Vi lanserade villkorliga förgreningar för dialogrutor tidigare i år, och nu kan du även utnyttja villkorliga förgreningar i konversationsflöden! Med villkorlig förgreningslogik kan du skapa förgreningar i ditt flöde baserat på olika villkor.

### Live-chatt för konversationsflöden {#live-chat-for-conversational-flows}

Vi lanserade chattfunktioner för dialogrutor 2023, och nu kan du även lägga till live-chattengagemang i dina konversationsflöden. Om du använder konversationsflöden med dina Marketo Engage-formulär kan du nu tillåta kvalificerade besökare att chatta med en handläggare direkt efter att formuläret har skickats in!

### Senaste Marketo Engage-aktiviteter i agentinkorgen {#recent-marketo-engage-activities-in-agent-inbox}

Vi har lagt till nyligen använda Marketo Engage-aktiviteter i avsnittet Senaste aktiviteter i Agent Inbox, så när en besökare på en webbplats begär att chatta med en agent kan agenten snabbt se om besökaren nyligen har deltagit i någon av följande Marketo Engage-aktiviteter (de senaste 25 aktiviteterna):

* Öppnad e-post
* Besökt webbsida
* Ifyllt formulär
* Hade intressant ögonblick

![](assets/dynamic-chat-release-3.png)

### Kalenderanslutningsstatus i Agenthantering {#calendar-connection-status-in-agent-management}

Administratörer kan nu enkelt se vilka agenter med mötesbokningsbehörighet som har kopplat sina kalendrar till Dynamic Chat. På så sätt kan du se till att hela säljteamet är anslutet och redo att acceptera mötesförfrågningar från Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Inställning för minsta meddelande i agentkalenderns konfiguration {#minimum-notice-setting-in-agent-calendar-configuration}

Användare rapporterade att webbbesökare bokade möten i sin kalender med så lite som 10 minuters förhandsmeddelande, så vi introducerade en inställning för minsta antal meddelanden i agentkalenderkonfigurationen och angav standardledtiden till 24 timmar.

![](assets/dynamic-chat-release-5.png)

### Lägg till/ta bort användarbeteende har uppdaterats {#add-remove-user-behavior-updated}

Vissa användare angav att de hade problem med att lägga till och ta bort agenter i den dynamiska chatten, så vi har gjort några ändringar för att åtgärda dessa problem.

När en användare läggs till i Admin Console med direktchatt eller mötesbokningstillstånd visas de omedelbart i listan över agenthantering och kan läggas till i dialogrutor, konversationsflöden, routningsregler och team.

När en användare med mötesbokning eller behörigheter för live-chatt tas bort från Admin Console, tas de omedelbart bort från Dynamic Chat, blir inte längre tillgängliga för live-chatt eller mötesroutning och kommer inte längre att räkna mot licensbegränsningar.

### Förbättrade rapportprestanda på konversationsnivå {#improved-conversation-level-report-performance}

Rapporterna om individuella dialoger och konversationsflöden har nu blivit mer presterande och korrekta. Tidigare kunde det ta flera sekunder att läsa in dialograpporter och data stämde ibland inte överens med globala prestandarapporter. Nu läses rapporterna från din dialogruta in på ett ögonblick och data justeras alltid efter globala rapportdata.

![](assets/dynamic-chat-release-6.png)

### Behörighetsuppdateringar {#permission-updates}

Vi har rensat bort behörighetsstrukturen och namngivningen i Adobe Admin Console för att göra behörighetshanteringen mer intuitiv.

* Kategorin &#39;Konversationshantering&#39; kallas nu för &#39;Konversationer&#39;
* Kategorin Möten kallas nu för Verksamheter
* Kategorin Agentinställningar kallas nu för Agenter
* Kategorin Administratörsinställningar kallas nu Konfiguration
* Kategorin Live Chat har tagits bort och alla behörigheter för live-chatt flyttades till kategorin Agenter

![](assets/dynamic-chat-release-7.png)

### Stöd för hyperlänkar i Agent Inbox {#support-for-hyperlinks-in-agent-inbox}

Nu när chattagenter delar URL:er med besökare i chatten kommer dessa URL:er att hyperlänkas så att besökarna enkelt kan klicka på dem för att navigera till sidan, i stället för att behöva kopiera och klistra in URL:en i webbläsaren.

### Ange nyckelbeteende som har uppdaterats i agentinkorgen {#enter-key-behavior-updated-in-agent-inbox}

Vi bytte returtangentsbeteende i Agent Inbox, så om du trycker på Retur- eller Retur-tangenten skickas ditt meddelande och om du trycker på Skift+Enter skapas en radbrytning.

![](assets/dynamic-chat-release-8.png)

### Round robat page removed {#round-robin-page-removed}

Oroa dig inte! Cirkulationsrundning av råmaterial fungerar fortfarande som avsett och fungerar på samma sätt som tidigare. Vi har just tagit bort sidan som visade en ofta felaktig lista över agenter och deras ordning i den runda routningskön för robin.

När vi lanserade Dynamic Chat 2022 fanns det inget stöd för live-chatt, enbart mötesbokning, och den runda sidan för routing har utformats med enbart mötesbokning i åtanke. I och med lanseringen av live chatt förra året blev den runda startsidan föråldrad eftersom den inte korrekt återspeglar den mer komplexa karaktären av rundrobat-routning mellan agenter med både mötesbokningar och live chattbehörigheter. Vi undersökte några olika alternativ för att ta itu med detta, men bestämde slutligen att det var det bästa alternativet för att minimera förvirringen att ta bort allt.

![](assets/dynamic-chat-release-9.png)

## Version från februari 2024 {#february-release}

**Releasedatum: 22 februari 2024**

### Sidan Konversationer {#conversations-page}

På den nya sidan Konversationer får du tillgång till en enda butik där du kan visa transkriberingar för alla konversationer (automatiska och aktiva) som har ägt rum för din instans, både kända och anonyma leads, vilket ger dig en bättre inblick i hur kunderna interagerar med era dialogrutor, konversationsflöden och aktiva agenter.

![](assets/dynamic-chat-release-10.png)

### Datumintervallet på den globala kontrollpanelen har ökat från 90 dagar till 24 månader {#date-range-in-global-dashboard}

Du frågade och vi levererade. Nu kan ni se Dynamic Chat engagemangsdata i upp till två år på alla analyspaneler.

### Villkorliga förgreningar i dialogrutor {#conditional-branching-in-dialogues}

Med villkorlig förgreningslogik kan du skapa förgreningar i Dialog-flöden baserat på olika villkor. Nu kan du presentera olika innehåll för olika personer i samma dialogruta baserat på lead- och företagsattribut i Marketo Engage.

## Version från januari 2024 {#january-release}

**Releasedatum: 24 januari 2024**

### Inställning för samtidiga chattbegränsningar i agenthantering {#Concurrent-live-chat-limit-setting}

Som standard kan varje live chattagent i din instans delta i högst fem live chattsessioner åt gången. Vi har infört en ny inställning för agenthantering som gör att du kan justera den här gränsen från 1 till 10.

![](assets/dynamic-chat-release-11.png)
