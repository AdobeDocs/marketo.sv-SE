---
description: Aktuell versionsinformation – Marketo Docs – produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: f49158e8b180641c1202b39b091ef8dd4088074e
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Versionsinformation: januari 2024 {#release-notes-jan-24}

Här nedan hittar du alla funktioner som ingår i versionen från 24 januari. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner faller under standardversionscykeln och kommer att släppas den **12 januari 2024**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>On Demand Webinars för interaktiva webbinarier</strong>: On-Demand Webinars gör att du kan publicera webbinariet och spåra dess besök/bevakningar. Detta hjälper dig att få fler leads genom registranter som inte deltar i webbinariet (ej showen) men som fortfarande är intresserade av att ta reda på mer och visa inspelningen.</td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">On-Demand-webbinarier</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
  </tr>
    <tr> 
   <td><strong>Conversational Landing Pages</strong>: Bädda in ett konversationsflöde i Dynamic Chat direkt på en landningssida i Marketo Engage så att besökarna kan schemalägga ett möte via Dynamic Chat utan att behöva fylla i ett formulär eller interagera med en chattbot.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   </tr>
    <tr> 
   <td><strong>Filtrerar e-postsatsaktivitet</strong>: Förbättrar hämtning av robotaktiviteter för e-postinteraktion genom att du kan välja hur aggressiv du vill att filtrering av robotaktivitet ska vara.</td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtrerar e-postsatsaktivitet</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   </tr>
    <tr> 
   <td><strong>API-uppdatering för massimport av leads</strong>: En mindre justering har gjorts av beteendet för API:t för import av gruppleads när <b>id</b> anges som <b>lookupField</b> när jobb skapades. Om en personpost är länkad till den angivna <b>id</b> finns inte i Marketo Engage-databasen, ingen postuppdatering kommer att ske eftersom posten inte kan hittas. Det uppdaterade beteendet innebär nu att antalet ökar i <b>numOfRowsFailed</b> -egenskapen i svaret, vilket signalerar att åtgärden har misslyckats i sådana fall.</td> 
   <td><i>Kommer snart</i></td>
   <td>n/a</td>
  </tr>
 </tbody> 
</table>
<br/>

## Agile Release-funktioner {#agile-release-features}

Alla funktioner nedan följer ett Agile-format och släpps på olika datum före eller efter standardreleasedatum. Kontrollera status bredvid varje funktion.

### Försäljningsinsikter {#sales-insight-actions}

![(stjärna)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:15%">Status</th>
   <th style="width:20%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Utbyggbart dispositionsfönster</strong>: Det oanvända utrymmet komprimeras nu automatiskt i e-postfönstret för disposition, vilket ger mer utrymme i redigeraren. Dessutom kommer fönstret att kunna öppnas och expandera ännu mer, vilket ger användarna så mycket utrymme de behöver för att redigera sina e-postmeddelanden.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:15%">Status</th>
   <th style="width:20%">Dokumentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Chatbot-användargränssnitt för konversationsbaserade Forms</strong>: Besökare på webbplatser kan nu begära live-chatt i ett konversationsflöde.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Alternativ för Chatbot-teckensnittsfärg</strong>: Anpassa teckensnittsfärger i en chattbot-konfiguration.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Alternativ för att upprepa dialogrutan</strong>: Du kan nu starta om dialogrutan i början när en besökare har nått slutet.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Manuell avbruten chatt</strong>: Både besökare och agenter kan nu avsluta en live-chattsession manuellt.</td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Agent Inbox</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Senaste Marketo Engage-aktiviteter i agentinkorgen</strong>: Nyligen utförda Marketo Engage-aktiviteter, t.ex. Öppnad e-post och Ifyllt formulär, visas för leads i agentinkorgen.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Villkorlig förgrening</strong>: Nu kan du visa besökare olika konversationsinnehåll baserat på fördefinierade villkor, till exempel besökarnas plats eller tillgänglighet som aktiv agent.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Synkronisera lead-API-uppdatering**: Funktionen för API:t för synkronisering av lead har ändrats något vad gäller uppdateringar av `unsubscribed` fält. Nu när du passerar `null` som värdet är lika med att skicka värdet för `false`.

* **Marketo Engage Forms jQuery 1.x**: I januariversionen 2024 uppdaterar vi jQuery för Marketo Engage Forms till jQuery 3.x. Detta kan påverka implementeringen av anpassade formulär beroende på äldre versioner av jQuery. [Läs mer här](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **E-postverifiering för användare med endast enkel inloggning**: Endast SSO-användare har verifierats automatiskt, vilket gör att de kan använda ett e-postkonto som inte är tillgängligt. Från och med mitten av januari kommer alla befintliga användare med enkel inloggning att bli overifierade och ombeds att verifiera sin e-post via en länk som vi skickar till e-postkontot. Alla nya användare med enkel inloggning behöver bara verifiera sina e-postadresser framöver.
