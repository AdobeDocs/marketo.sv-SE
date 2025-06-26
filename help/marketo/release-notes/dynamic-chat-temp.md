---
description: Dynamic Chat versionsinformation – Marketo Docs – Produktdokumentation
title: Dynamic Chat versionsinformation
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 3%

---

# Dynamic Chat versionsinformation {#dynamic-chat-release}

Adobe Dynamic Chat-releaser fungerar enligt en kontinuerlig leveransmodell som ger en mer skalbar metod för driftsättning av funktioner. Ibland finns det flera releaser på en månad, så var vänlig och kika regelbundet efter den senaste informationen.

Standardsidan för versionsinformation för Marketo Engage [finns här](/help/marketo/release-notes/current.md){target="_blank"}.

## Version från juni 2025 {#june-25-release}

### Routing Logic Revamp {#routing-logic-revamp}

Vi har omarbetat logiken för live-chattroutning i Dynamic Chat för att säkerställa ett mer intelligent och förutsägbart engagemangsbeteende för alla routningstyper (konto, anpassad, team och Round Robin). Den nya logiken förenklar routningsflöden och förbättrar reservhanteringen när agenter inte är tillgängliga.

#### Viktiga förbättringar i routningsbeteende

* **Upp till två förlovningsförsök per session**

   * Systemet försöker ansluta till högst två agenter, men strikt inom den primära routningsregeln.

   * Om en agent är tillgänglig men inte svarar (t.ex. avböjer eller missar) försöker systemet att göra en andra agent från samma pool.

   * Reservlogik (som Round Robin) aktiveras bara om inga berättigade agenter hittas under den första upplösningen - inte för att försöka igen efter ett misslyckat engagemang.

* **Routningsregelspecifikt beteende**

_**Kontoroutning**_

Om en besökares e-postdomän mappar till ett känt konto prioriteras alltid den mappade agenten.

Om agenten är tillgänglig dirigeras chatten till dem direkt.

Om agenten inte är tillgänglig:

Försöker inte med en annan agent, även om Round Robin är aktiverad som reserv.

Istället:

Visar den mappade agentens möteskalender (om den är aktiverad), eller

Fallar tillbaka till ett standardmeddelande (värsta fall).

Routningsregeln på kortnivå (t.ex. Team, Custom) beaktas endast om Kontoroutning inte är giltig (ingen matchande domän eller agent).

_**Anpassad routning/teamroutning**_

Dessa regler kan returnera flera berättigade agenter.

Om den första tillgängliga agenten inte aktiveras kommer systemet att försöka med en till agent från samma lista.

Rund Robin-reservlösning utlöses inte bara för att en agent inte svarade.

Om ingen av agenterna engagerar:

Systemet visar den första provade agentens kalender (om aktiverad), eller

Visar standardfelmeddelandet.

_**Round Robin Routing**_

När det används som en primär routningsregel:

Försöker att anlita den första tillgängliga agenten från poolen med resursallokering.

Om den första inte svarar försöker den igen med nästa bästa berättigade agent.

Om Round Robin används som reserv aktiveras den bara om inga agenter har lösts från den primära regeln.

**Upplevelseflöde för besökare**

Systemet kontrollerar om kontodirigering är relevant.

Om ja och agent finns tillgänglig → ansluter omedelbart.

Om det inte är godkänt eller om agenten inte är tillgänglig → går vidare till routningsregeln på kortnivå.

Routningsregel på kortnivå (Custom, Team, Round Robin) utvärderas.

Berättigade agenter kontrolleras för tillgänglighet (behörigheter, status).

Systemet engagerar en agent och försöker vid behov att få en andra agent från samma regel.

Om inget engagemang lyckas → reservlogik används:

kalenderreserv (om aktiverad), eller

Standardmeddelande.

Round Robin-reservlösningar beaktas endast när inga berättigade agenter hittas från den primära routningsregeln, inte när enskilda agenter inte svarar.

**Användningsexempel**

Kontodirigering

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

Anpassad routning

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

Teamroutning

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

Round Robin Routing

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Exempel</th>
    <th>Resultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idealiskt</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Reservfall (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Ingen återställningsagent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

### Pulsmeddelande {#pulse-notification}

När en besökare begär att få ansluta till en agent tillhandahåller vi idag meddelanden i appen till agenten, men agenterna saknar ofta dessa chattar.

* Live-agenten får nu e-post, Slack, Inapp, webbläsarmeddelanden när en ny besökare är intresserad av att chatta

* Innehåll för Pulse-meddelanden kan vara samma som det vi använder idag för meddelanden i appen och webbläsare

Beteendet bör vara detsamma som det är för agenten att acceptera när flera agenter accepterar.
