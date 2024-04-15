---
description: Versionsinformation för Dynamic Chat - Marketo Docs - produktdokumentation
title: Versionsinformation för Dynamic Chat
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Versionsinformation: april 2024 {#release-notes-apr-24}

Adobe Dynamic Chat-releaser fungerar enligt en kontinuerlig leveransmodell som ger en mer skalbar metod för driftsättning av funktioner. Ibland finns det flera releaser på en månad, så var vänlig och kika regelbundet efter den senaste informationen.

Standardsidan för versionsinformation för Marketo Engage [finns här](/help/marketo/release-notes/current.md){target="_blank"}.

## April-utgåvan {#april-release}

**Releasedatum: 16 april 2024**

### Konversationsflöden är nu tillgängliga för kunder på Select-paket {#conversational-flows-select-package}

När vi lanserade konversationsflöden förra året kunde kunder i paketet Dynamic Chat Select bara utnyttja möjligheten att testa 100 livstidsavtal. Nu är konversationsflöden helt tillgängliga för alla kunder i Select-paketet.

Konversationsflöde-engagemang räknas med i den månatliga gränsen på 250 engagerade konversationer för kunder i Select-paketet.

### Återanropsfunktioner {#callback-functions}

Med återanropsfunktionerna kan ni samla in Dynamic Chat-analyshändelser i externa system, som Adobe Analytics eller Google Analytics, när besökarna interagerar med Dynamic Chat-konversationer. Du aktiverar analyshändelser för Dynamic Chat genom att registrera ett återanrop med API:t för att avlyssna händelserna. På så sätt kan ni få en helhetsbild av Dynamic Chat engagemang när det gäller andra nyckeldata, till exempel webbtrafik.

### Tillgänglighetsvillkor för Live-agent har lagts till i villkorlig förgrening {#live-agent-availability-conditional-branching}

Förutom inbyggda och anpassade Marketo-fält kan du nu använda villkorlig förgreningslogik för att skapa förgreningar baserat på agentens tillgänglighet. Det här är användbart om du bara vill ge besökarna möjlighet att tala med en handläggare när det finns aktiva agenter tillgängliga.

SCREENSHOT

### Villkoret Smart lista har lagts till i villkorlig förgrening {#smart-list-condition}

Med det nya villkoret Marketo Engage Smart List i villkorlig förgreningslogik kan du skapa förgreningar baserat på befintliga målgrupper som du redan har skapat i Marketo i stället för att definiera förgreningsvillkoren för målgrupper i Dynamic Chat.

SCREENSHOT

### Villkorliga förgreningar för konversationsflöden {#conditional-branching-for-conversational-flows}

Vi har släppt villkorliga förgreningar för dialogrutor tidigare i år och nu kan du även använda villkorliga förgreningar i konversationsflöden! Med villkorlig förgreningslogik kan du skapa förgreningar i ditt flöde baserat på olika villkor.

### Live-chatt för konversationsflöden {#live-chat-for-conversational-flows}

Vi lanserade chattfunktioner för dialoger förra året, och nu kan du även lägga till live-chattengagemang i dina konversationsflöden. Om du använder konversationsflöden med dina Marketo-formulär kan du nu tillåta kvalificerade besökare att chatta med en handläggare direkt efter att formuläret har skickats in!

### Nyligen använda Marketo Engage-aktiviteter i agentinkorgen {#recent-marketo-engage-activities-in-agent-inbox}

Vi har lagt till nyligen utförda Marketo Engage-aktiviteter i avsnittet Senaste aktiviteter i Agent Inbox så att agenten enkelt kan se om besökaren nyligen har deltagit i någon av följande Marketo-aktiviteter (de senaste 25 aktiviteterna) när en besökare på platsen begär att få chatta med en agent:

* Öppnad e-post
* Besökt webbsida
* Ifyllt formulär
* Hade intressant ögonblick

SCREENSHOT

### Kalenderanslutningsstatus i Agenthantering {#calendar-connection-status-in-agent-management}

Administratörer kan nu enkelt se vilka agenter med mötesbokningsbehörighet som har kopplat sina kalendrar till Dynamic Chat. På så sätt kan ni se till att hela säljteamet är anslutet och redo att acceptera mötesförfrågningar från Dynamic Chat.

SCREENSHOT

### Inställning för minsta meddelande i agentkalenderns konfiguration {#minimum-notice-setting-in-agent-calendar-configuration}

Kunderna rapporterade att webbbesökare bokade möten i sin kalender med så lite som 10 minuters förhandsmeddelande, så vi introducerade en miniminivå för avisering i agentkalenderkonfigurationen och angav standardledtiden till 24 timmar.

SCREENSHOT

### Nya meddelanden i appen {#new-in-app-notifications}

Vi har introducerat tre nya meddelanden i appen som hjälper dig att hålla dig informerad om statusen för din instans i Dynamic Chat i realtid.

* Text
* Text
* Text

### Lägg till/ta bort användarbeteende har uppdaterats {#add-remove-user-behavior-updated}

Vissa kunder meddelar oss om problem de har med att lägga till och ta bort agenter i Dynamic Chatt, så vi har gjort några ändringar för att åtgärda dessa problem.

När en användare läggs till i Admin Console med direktchatt eller mötesbokningstillstånd visas de omedelbart i listan över agenthantering och kan läggas till i dialogrutor, konversationsflöden, routningsregler och team.

När en användare med mötesboknings- eller live-chattbehörigheter tas bort från Admin Console tas de omedelbart bort från Dynamic Chat, inte längre är tillgängliga för live-chatt eller mötesroutning och inte längre räknas av mot licensbegränsningar.

### Förbättrade rapportprestanda på konversationsnivå {#improved-conversation-level-report-performance}

Rapporterna om individuella dialoger och konversationsflöden har nu blivit mer presterande och korrekta. Tidigare kunde det ta flera sekunder att läsa in dialograpporter och data stämde ibland inte överens med de globala prestandarapporterna. Nu läses rapporterna från de enskilda dialogrutorna in på ett ögonblick och data justeras alltid efter globala rapportdata.

SCREENSHOT

### Behörighetsuppdateringar {#permission-updates}

Vi har rensat bort behörighetsstrukturen och namngivningen i Adobe Admin Console för att göra behörighetshanteringen mer intuitiv.

* Kategorin Konversationshantering kallas nu Konversationer
* Möteskategorin kallas nu för aktiviteter
* Kategorin Agentinställningar kallas nu Agenter
* Kategorin Administratörsinställningar kallas nu Konfiguration
* Kategorin Live Chat har tagits bort och alla behörigheter för live-chatt flyttades till kategorin Agenter

SCREENSHOT

### Stöd för hyperlänkar i agentinkorgen {#support-for-hyperlinks-in-agent-inbox}

Nu när chattagenter delar URL:er med besökare i chatten kommer dessa URL:er att hyperlänkas så att besökarna enkelt kan klicka på dem för att navigera till sidan, i stället för att behöva kopiera och klistra in URL:en i webbläsaren.

### Ange nyckelbeteende som har uppdaterats i agentinkorgen {#enter-key-behavior-updated-in-agent-inbox}

Vi har ändrat returtangentsbeteendet i Agent Inbox så att du skickar meddelandet genom att trycka på Retur eller Retur och genom att trycka på Skift+Retur skapas en radbrytning.

SCREENSHOT

### Round robat page removed {#round-robin-page-removed}

Oroa dig inte! Cirkulationsrundning av råmaterial fungerar fortfarande som avsett och fungerar på samma sätt som tidigare. Vi har just tagit bort sidan som visade en ofta felaktig lista över agenter och deras ordning i den runda routningskön för robin.

För att skapa någon typ av kontext fanns det inget stöd för live chatt när vi lanserade Dynamic Chat 2022, bara mötesbokning och den runda sidan för robin-routning utformades endast med mötesbokning i åtanke. I och med lanseringen av live chatt förra året blev den runda startsidan föråldrad eftersom den inte korrekt återspeglar den mer komplexa karaktären av rundrobat-routning mellan agenter med både mötesbokningar och live chattbehörigheter. Vi undersökte några olika alternativ för att ta itu med detta, men bestämde slutligen att det var det bästa alternativet för att minimera förvirringen att ta bort allt.

## Februariversion {#february-release}

**Releasedatum: 22 februari 2024**

### Sidan Konversationer {#conversations-page}

På den nya sidan Konversationer får du en enda kontaktpunkt där du kan se transkriberingar för alla konversationer (automatiska och aktiva) som har ägt rum för din instans, både kända och anonyma leads, vilket ger dig bättre insyn i hur kunderna interagerar med era dialoger, konversationsflöden och aktiva medarbetare.

SCREENSHOT

Datumintervallet på den globala kontrollpanelen har ökat från 90 dagar till 24 månader

Du frågade och vi levererade. Nu kan ni se data om engagemang i Dynamic Chat i upp till två år på alla kontrollpaneler för analyser.

### Villkorliga förgreningar i dialogrutor {#conditional-branching-in-dialogues}

Med villkorlig förgreningslogik kan du skapa förgreningar i Dialog-flöden baserat på olika villkor. Nu kan du presentera olika innehåll för olika personer i samma dialogruta baserat på lead- och företagsattribut i Marketo.

## Januariversion {#january-release}

**Releasedatum: 24 januari 2024**

### Inställning för samtidiga chattbegränsningar i agenthantering {#Concurrent-live-chat-limit-setting}

Som standard kan varje live chattagent i din instans delta i högst fem live chattsessioner åt gången. Vi har infört en ny inställning för agenthantering som gör att du kan justera gränsen från 1 till 10.

SCREENSHOT
