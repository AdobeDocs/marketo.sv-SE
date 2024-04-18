---
description: Aktuell versionsinformation – Marketo Docs – produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 9f442b64f2e6d012207f79d06298583655db86b7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 2%

---

# Versionsinformation: april 2024 {#release-notes-apr-24}

Här nedan hittar du alla funktioner som ingår i versionen från 24 april. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner faller under standardversionscykeln och kommer att släppas den **26 april 2024**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Förbättringar av interaktiva webbinarier</strong>: Nu kan du ge värdar och presentatörer möjlighet att lägga till en webbinarititel, byta namn på ett rum och manuellt synkronisera engagemangsdata efter att eventet har levererats.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Förbättringar av granskningsspår</strong>: Nya typer av åtgärder kan nu fångas in i granskningsspåret för ändringar som gjorts i Fälthantering, ändringar som gjorts i Användare och roller samt antalet personer som exporterats från listor och smarta listor.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Nya behörigheter för användare och roller</strong>: Det finns nya behörigheter som ger användare mer detaljerad åtkomst till Marketo Engage. Styr delar av Admin som inte tidigare har skapats, t.ex. Ny upplevelse och prediktiva målgrupper, dela behörigheter för att bevilja åtkomst till resursgranskningsspår och administratörsgranskningsspår separat, och använd nya skaps- och flyttbehörigheter för resurser och mappar för att förhindra att skrivskyddade användare gör ändringar.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **API-uppdatering för aktiviteter**: Den 26 april lägger vi till flera nya attribut till webbaserade och e-postbaserade aktiviteter som returneras när du hämtar aktiviteter med [MARKETO REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} slutpunkt för att granska attributinformation för varje aktivitet.

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
