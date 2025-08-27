---
description: Dynamic Chat versionsinformation – Marketo Docs – Produktdokumentation
title: Dynamic Chat versionsinformation
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 2%

---

# Dynamic Chat versionsinformation {#dynamic-chat-release}

Adobe Dynamic Chat-releaser fungerar enligt en kontinuerlig leveransmodell som ger en mer skalbar metod för driftsättning av funktioner. Ibland finns det flera releaser på en månad, så var vänlig och kika regelbundet efter den senaste informationen.

Standardsidan för versionsinformation för Marketo Engage [finns här](/help/marketo/release-notes/current.md){target="_blank"}.

## Version från juni 2025 {#june-2025-release}

### Routing Logic Revamp {#routing-logic-revamp}

Vi har omarbetat logiken för live-chattroutning i Dynamic Chat för att säkerställa ett mer intelligent och förutsägbart engagemangsbeteende för alla routningstyper (konto, anpassad, team och Round Robin). Den nya logiken förenklar routningsflöden och förbättrar reservhanteringen när agenter inte är tillgängliga.

#### Viktiga förbättringar i routningsbeteende

* **Upp till två förlovningsförsök per session**

   * Systemet försöker ansluta med upp till två agenter (högst), men strikt inom den primära routningsregeln.

   * Om en agent är tillgänglig men inte svarar (till exempel avvisar eller missar chatten) försöker systemet ansluta till en annan agent från samma pool.

   * Reservlogik (som Round Robin) aktiveras bara om inga berättigade agenter hittas under den första upplösningen, inte för att försöka igen efter ett misslyckat engagemang.

* **Routningsregelspecifikt beteende**

_**Kontoroutning**_

Om en besökares e-postdomän mappar till ett känt konto prioriteras alltid den mappade agenten.

Om agenten är tillgänglig dirigeras chatten till dem direkt.

Om agenten inte är tillgänglig:

* Försöker inte med en annan agent, även om Round Robin är aktiverad som reserv.

I stället kan det antingen:

* Visar den mappade agentens möteskalender (om den är aktiverad), eller:
* Fallar tillbaka till ett standardmeddelande (värsta fall).

Routningsregeln på kortnivå (till exempel Team, Custom) beaktas endast om Kontoroutning inte är giltig (ingen matchande domän eller agent).

_**Anpassad routning/teamroutning**_

Dessa regler kan returnera flera berättigade agenter.

Om den första tillgängliga agenten inte aktiveras försöker systemet att använda ytterligare en agent från samma lista.

Rund Robin-reservlösning utlöses inte bara för att en agent inte svarar.

Om ingen av agenterna engagerar:

* Systemet visar den första provade agentens kalender (om aktiverad),
-or-
* Visar standardfelmeddelandet.

_**Round Robin Routing**_

När det används som en primär routningsregel:

* Försöker att anlita den första tillgängliga agenten från poolen med resursallokering.

* Om den första agenten inte svarar försöker den igen med nästa bästa berättigade agent.

Om Round Robin används som reserv aktiveras den bara om inga agenter har lösts från den primära regeln.

_**Upplevelseflöde för besökare**_

Systemet kontrollerar om kontodirigering är relevant.

* Om ja och agent finns tillgänglig ansluter den omedelbart.

* Om agenten inte är berättigad eller inte är tillgänglig fortsätter den till routningsregeln på kortnivå.

Routningsregel på kortnivå (Custom, Team, Round Robin) har utvärderats.

* Berättigade agenter kontrolleras för tillgänglighet (behörigheter, status).

* Systemet engagerar en agent och försöker vid behov att få en andra agent från samma regel.

* Om inget engagemang lyckas används reservlogiken:

   * Kalenderreserv (om aktiverad),
-or-
   * Standardmeddelande.

Round Robin-reservlösningar beaktas endast när inga berättigade agenter hittas från den primära routningsregeln, inte när enskilda agenter inte svarar.

##### Användningsfall {#use-cases}

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
    <td>Systemet visar en mappad agentkalender eller ett standardutfallsmeddelande.</td>
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
    <td>Anpassad logik löser en lista med agenter. Den första agenten är tillgänglig och accepterar chatt.</td>
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
    <td>Först försökte du att visa agentens kalender eller så visas standardåtergångsmeddelandet.</td>
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
    <td>Systemet väljer och ansluter till en agent från Round Robin-poolen.</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Två agenter är tillgängliga, men inget av dem, kalenderåtergång är aktiverat.</td>
    <td>Först försökte agentens kalender visas eller så utlöses ett reservmeddelande.</td>
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
    <td>Round Robin-poolen har flera agenter. Den andra agenten godkänner chatt efter det första inte.</td>
    <td>Chatten ansluter till en andra agent.</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>Inga agenter är tillgängliga i Round Robin-poolen. Möteskalendern är aktiverad.</td>
    <td>Kalendern visas för den första agenten i listan (om den är konfigurerad), eller så visas reservmeddelandet.</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>Inga tillgängliga agenter. Återställningen är inaktiverad.</td>
    <td>Ett statiskt reservmeddelande visas för besökaren.</td>
  </tr>
</tbody></table>

### Pulsmeddelande {#pulse-notification}

När en besökare begär att få ansluta till en agent skickar vi ett meddelande i appen till agenten. Men ibland saknar agenter dessa chattar.

Med den här versionen kan medarbetaren få e-post, Slack, meddelanden i appen och webbläsarmeddelanden när en ny besökare är intresserad av att chatta.

1. På din Adobe Experience Cloud-hemsida klickar du på kontoikonen och väljer **Inställningar**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Bläddra ned till _Meddelanden_ och gör de val du vill av Dynamic Chat.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Innehållet i ett Pulse-meddelande kan vara detsamma som det vi använder för meddelanden i appen och webbläsare.
