---
description: Dynamic Chat versionsinformation – Marketo Docs – Produktdokumentation
title: Dynamic Chat versionsinformation
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 236c99d8939f076d93dfcd7988fc89e4c617c113
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 2%

---

# Versionsinformation om TEMP Dynamic Chat {#dynamic-chat-release}

## September/oktober 2024-utgåvan {#august-release}

### Förbättrad chattanalys {#enhanced-live-chat-analytics}

Flera förbättringar har gjorts i kontrollpanelen för analyser, bland annat:

* Totalt antal begärda chatt live: antal besökare som har begärts för en chatt med agent

* Totalt antal anslutna live-chatt: antal anslutna besökare jämfört med totalt antal som har begärts för en chatt med agent

* Totalt antal missade chattförfrågningar: antal oövervakade besökare kontra totalt antal begärda för en chatt med agent

* Genomsnittlig chattlängd i minuter: analysera &quot;genomsnittlig chattlängd&quot; mellan besökare och agenter

* Genomsnittlig svarstid för agenter i sekunder: analysera&quot;genomsnittlig tid som agenter tar&quot; för att svara på frågor och svar om live-chatt

* Daglig instrumentpanel: live-chattförfrågningar anslutna, live-chattförfrågningar missade, sortera och filtrera nyligen använda live-chattaktiviteter

SCREENSHOT

### Konversationsbedömning {#conversation-scoring}

Kvantifiera era leads baserat på kvaliteten på deras chattinteraktion och använd det måttet som utlösare/filter i Marketo Engage Smart Campaigns. Använd det nya attributet _konversationspoäng_ för följande aktiviteter:

* Engagerad med en dialogruta
* Engagerad med ett konversationsflöde
* Anställda hos en agent

**Saker att notera:**

* Poängvärdet är från 0, 1, 2, 3 (standardvärdet är null)

* När konversationen är klar eller utesluten sparar aktiviteten poängvärdet och posten som den inte kan redigeras????????????????????????????????????????????????????????????????????????? (vad betyder detta)

* Ställa in poäng:

   * I agentens inkorg - under en live-chatt kan agenten uppdatera eller ange ett poängvärde för konversationen, som lagras i konversationsaktiviteten

   * I strömdesignern - på målkortet, kan användaren uppdatera eller ange ett poängvärde för konversationen

SCREENSHOT

SCREENSHOT

SCREENSHOT

### Ny logik för att skapa leads {#new-lead-creation-logic}

Om ett lead fyller i ett formulär med e-postadressen `abc@test.com` och kodas som xyz, fyller sedan i samma formulär med e-postadressen `def@test.com`, skapas ett nytt lead, men cookie xyz kopplas till det nya leadet och tas bort från leadet `abc@test.com` .

Från och med då blir `abc@test.com` en lead utan cookie. LEDER DU?

Så när en besökare med cookie abc kommer till en sida och anger ett e-post-ID som `abc@p.com`:

TABELL

### Optimerad inläsningstid för konversationsflöde {#optimized-conversation-flow-load-time}

För att förbättra användarupplevelsen visas nu en kortare inläsare i stället för ett tomt utrymme när konversationsflödet läses in. KONVERSATION ELLER KONVERSATION???

**Före**

GIF

**Efter**

GIF

### Möjlighet att ärva teckensnitt {#option-to-inherit-font}

Som användare vill jag att min chattbot ska kunna ärva teckensnittet direkt från webbsidan där det läses in, i stället för att hantera teckensnittet i Dynamic Chat

Obs! När du aktiverar det här alternativet använder Chatbot det teckensnitt som är definierat i body-taggen på sidan
