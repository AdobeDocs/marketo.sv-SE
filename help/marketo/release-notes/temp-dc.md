---
description: Dynamic Chat versionsinformation – Marketo Docs – Produktdokumentation
title: Dynamic Chat versionsinformation
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 7fbfdc6d34d2f1174e921464d64689b0c5687914
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 2%

---

# Versionsinformation om TEMP Dynamic Chat {#dynamic-chat-release}

## September/oktober 2024-utgåvan {#august-release}

### Förbättrad chattanalys {#enhanced-live-chat-analytics}

Flera förbättringar har gjorts i kontrollpanelen för analyser, bland annat:

* Totalt antal begärda chattsamtal live: antal besökare som har begärt en chatt med agent

* Totalt antal anslutna live-chatt: antal anslutna besökare jämfört med totalt antal som har begärts för en&quot;chatt med agent&quot;

* Totalt antal missade chattförfrågningar: antal oövervakade besökare kontra totalt antal begärda för en&quot;chatt med agent&quot;

* Genomsnittlig chattlängd i minuter: analysera &quot;genomsnittlig chattlängd&quot; mellan besökare och agenter

* Genomsnittlig svarstid i sekunder för agenter: analysera&quot;genomsnittlig tid som agenter tar&quot; för att svara på frågor och svar om live-chatt

* Daglig instrumentpanel: live-chattförfrågningar anslutna, live-chattförfrågningar missade, sortera och filtrera nyligen använda live-chattaktiviteter

SCREENSHOT

### Konversationsbedömning {#conversation-scoring}

Kvantifiera era leads baserat på kvaliteten på deras chattinteraktion och använd det måttet som utlösare/filter i Marketo Engage Smart Campaigns. Använd det nya attributet _konversationspoäng_ för följande aktiviteter:

* Engagerad med en dialogruta
* Engagerad med ett konversationsflöde
* Anställda hos en agent

**Saker att notera:**

* Poängvärdet är från 0, 1, 2, 3 (standardvärdet är null)

* När konversationen är slutförd eller släppt sparar du betygsvärdet i aktiviteten och postar att den inte kan redigeras?????? (vad betyder den här meningen)

* Ställa in poäng:

   * I agentens inkorg - under en live-chatt kan agenten uppdatera eller ange ett poängvärde för konversationen, som lagras i konversationsaktiviteten

   * I strömdesignern - på målkortet, kan användaren uppdatera eller ange ett poängvärde för konversationen

SCREENSHOT

SCREENSHOT

SCREENSHOT

### Ny logik för att skapa leads {#new-lead-creation-logic}

Om ett lead fyller i ett formulär med e-postadressen `abc@test.com` och kodas som xyz, fyller sedan i samma formulär med e-postadressen `def@test.com`, skapas ett nytt lead, men cookie xyz kopplas till det nya leadet och tas bort från leadet `abc@test.com` .

Från och med då blir `abc@test.com` en lead utan cookie. ANONYM LEAD?

Så när en besökare med cookie abc kommer till en sida och anger ett e-post-ID som `abc@p.com`:

TABELL

### Optimerad inläsningstid för konversationsflöde {#optimized-conversation-flow-load-time}

För att förbättra användarupplevelsen visas nu en kortare inläsare i stället för ett tomt utrymme när konversationsflödet läses in. KONVERSATION ELLER KONVERSATION???

**Före**

GIF

**Efter**

GIF

### Möjlighet att ärva teckensnitt {#option-to-inherit-font}

Nu kan du aktivera chattbot för att direkt ärva teckensnittet från webbsidan där det ligger i stället för att hantera teckensnittet i Dynamic Chat. När du aktiverar det här alternativet får chattbot det teckensnitt som är definierat i taggen `<body>` på sidan.

SCREENSHOT

### Demandbase-integrering med Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Demandbase-användare kan hämta sin egen licens för Demandbase och aktivera integreringen. Använd personattribut för Demandbase för dialog, villkorsstyrd varumärkesprofilering och anpassad routning.

Dessa attributvärden skulle matchas mot en lead i realtid och lagras i respektive lead-profil.
