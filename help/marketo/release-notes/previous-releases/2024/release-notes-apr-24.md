---
description: Versionsinformation - april 2024 - Marketo Docs - produktdokumentation
title: Versionsinformation - april 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Versionsinformation: april 2024 {#release-notes-apr-24}

Här nedan hittar du alla funktioner som ingår i versionen från 24 april. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **26 april 2024**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr>
   <td><strong>Förbättringar av interaktiva webbinarier</strong>: Nu kan du ge värdar och presentatörer möjlighet att lägga till en titel på ett webbinarium, byta namn på ett rum och manuellt synkronisera engagemangsdata efter att evenemanget har levererats.</td>
   <td>Levererat</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Skapa ett interaktivt webbinarium</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Manuell synkronisering</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Förbättringar av granskningsspår</strong>:
   Nya typer av åtgärder kan nu fångas in i granskningsspåret för ändringar som gjorts i Fälthantering, ändringar som gjorts i Användare och roller samt antalet personer som exporterats från listor och smarta listor.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Nya behörigheter för användare och roller</strong>: Det finns nya behörigheter som ger användare mer detaljerad åtkomst till Marketo Engage. Styr delar av Admin som inte tidigare har skapats, t.ex. Ny upplevelse och prediktiva målgrupper, dela behörigheter för att bevilja åtkomst till resursgranskningsspår och administratörsgranskningsspår separat, och använd nya skaps- och flyttbehörigheter för resurser och mappar för att förhindra att skrivskyddade användare gör ändringar.
   <p>De nya behörigheterna kommer att visas i din Marketo Engage-instans från och med den 26 april, men är passiva tills vidare och kommer att vara tillgängliga senare under det här kvartalet.
   <li>Använd Adobe Experience Manager</li>
   <li>Få tillgång till Adobe organisationsmappning</li>
   <li>Åtkomst till administratörsgranskningsspår</li>
   <li>Åtkomst till resursgranskningsspår</li>
   <li>Använd ny upplevelse</li>
   <li>Nå prediktiva målgrupper</li>
   <li>Skapa rapport</li>
   <li>Skapa lista</li>
   <li>Exportera kampanjaktivitet</li>
   </td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Beskrivningar av rollbehörigheter</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **API-uppdatering för aktiviteter**: Den 26 april lägger vi till flera nya attribut till webbaserade och e-postbaserade aktiviteter som returneras när du hämtar aktiviteter med [Marketo REST API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. Aktiviteterna som listas nedan inkluderar nu attribut för webbläsare, plattform, enhet och användaragent. Anropa slutpunkten [Hämta aktivitetstyper](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} om du vill granska attributinformation för varje aktivitet.

**Webbaserade aktiviteter**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Aktivitet</th>
   <th style="width:70%">Attribut som lagts till nyligen</th>
   </tr>
  <tr>
   <td>Besök webbsidan</td>
   <td>Webbläsare, plattform, enhet</td>
  </tr>
   <tr>
   <td>Fyll i formulär</td>
   <td>Webbläsare, plattform, enhet</td>
  </tr>
  <tr>
   <td>Klicka på Länk</td>
   <td>Webbläsare, plattform, enhet</td>
  </tr>
 </tbody>
</table>

**E-postbaserade aktiviteter**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Aktivitet</th>
   <th style="width:70%">Attribut som lagts till nyligen</th>
  </tr>
   <tr>
   <td>Skicka e-post</td>
   <td>Webbläsare, plattform, enhet, användaragent</td>
  </tr>
   </tr>
  <tr>
   <td>E-post levererad</td>
   <td>Webbläsare, plattform, enhet, användaragent</td>
  </tr>
   <tr>
   <td>E-post studsade</td>
   <td>Webbläsare, plattform, enhet, användaragent</td>
  </tr>
  <tr>
   <td>Avbeställ e-post</td>
   <td>Webbläsare, plattform, enhet</td>
  </tr>
  <tr>
   <td>Öppna e-post</td>
   <td>Webbläsare</td>
  </tr>
   <tr>
   <td>Klicka på E-post</td>
   <td>Webbläsare</td>
  </tr>
  <tr>
   <td>Mjuk e-poststudsning</td>
   <td>Webbläsare, plattform, enhet, användaragent</td>
  </tr>
 </tbody>
</table>
