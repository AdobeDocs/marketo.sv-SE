---
description: Versionsinformation - mars 2024 - Marketo Docs - produktdokumentation
title: Versionsinformation - mars 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Versionsinformation: Mars 2024 {#release-notes-mar-24}

Här nedan hittar du alla funktioner som ingår i mars 24. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **8 mars 2024**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Avancerad logik för konversationsflöde</strong>: Lägg till ytterligare fält för utvärdering i ett enda val för konversationsflödesuppföljning.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationsflödesinställningar för Marketo Engage Forms</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Ändra ordning på logik för konversationsflöde</strong>: I Marketo Engage Forms kan du nu ändra ordning på alternativen för konversationsflöde i stället för att behöva ta bort och lägga tillbaka.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationsflödesinställningar för Marketo Engage Forms</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>API-aktivitetsmetadata</strong>:
   Metadata som User Agent, Platform och Device ingår nu i webb- och e-postaktiviteter, vilket ger enhetliga insikter i dessa aktiviteter via Marketo REST API.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
 </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Hämta API-korrigering för programmedlem**: En ändring gjordes nyligen för att korrigera beteendet för slutpunkten [Hämta programmedlemmar](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Tidigare, när filtertypen `updatedAt` användes för att ange ett datumintervall, fanns det en risk för att programmedlemsposter som uppdaterats inom det intervallet inte inkluderades i svaret. Dessutom fanns det en risk att poster för programmedlemskap som uppdaterats utanför det angivna datumintervallet felaktigt togs med i svaret. Båda problemen har lösts.

* **Borttagning av plugin-programmet för kontoinsikt**: Adobe tar bort plugin-programmet [Account Insight &#x200B;](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} från Chrome Web Store den 8 april 2024. Befintliga användare: du kan fortsätta använda plugin-programmet tills du migrerar din Marketo Engage-instans till Adobe Identity och Admin Console. Den här ändringen **påverkar inte** andra TAM-funktioner/data i Marketo Engage eller e-postplugin-programmen för Chrome och Outlook som fungerar med Sales Insight. [Läs mer](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
