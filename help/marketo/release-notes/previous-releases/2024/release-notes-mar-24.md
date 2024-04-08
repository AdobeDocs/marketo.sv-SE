---
description: Versionsinformation - mars 2024 - Marketo Docs - produktdokumentation
title: Versionsinformation - mars 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Versionsinformation: Mars 2024 {#release-notes-mar-24}

Här nedan hittar du alla funktioner som ingår i mars 24. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner faller under standardversionscykeln och kommer att släppas den **8 mars 2024**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr> 
   <td><strong>Avancerad konverteringsflödeslogik</strong>: Lägg till ytterligare fält för utvärdering i ett och samma val för uppföljning av konversationsflöde.</td> 
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
   <td><strong>Ändra ordning på konversationsflödeslogik</strong>: I Marketo Engage Forms kan du nu ändra ordningen på alternativen för konversationsflöde i stället för att behöva ta bort och lägga tillbaka.</td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationsflödesinställningar för Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API-aktivitetsmetadata</strong>: Metadata som User Agent, Platform och Device ingår nu i webb- och e-postaktiviteter, vilket ger enhetliga insikter i dessa aktiviteter via Marketo REST API.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Hämta API-korrigering för programmedlem**: En ändring gjordes nyligen för att korrigera beteendet i [Hämta programmedlemmar](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} slutpunkt. Tidigare, vid användning av `updatedAt` filtertyp för att ange ett datumintervall. Det kan bero på att poster för programmedlemskap som uppdaterats inom det intervallet inte ingick i svaret. Dessutom fanns det en risk att poster för programmedlemskap som uppdaterats utanför det angivna datumintervallet felaktigt togs med i svaret. Båda problemen har lösts.

* **Borttagning av plugin-program för Insight Browser**: Adobe tar bort målkontohanteringen [Webbläsarplugin för Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
