---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: ce6a748acfb25ebc90c31dbfb16cf0230ca20b73
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 4%

---

# Versionsinformation: februari 2026 {#release-notes-jan-26}

Här nedan hittar du alla funktioner som finns i februari 26. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **20 februari 2026**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - mappåtgärder</strong>: Paritet med den gamla e-postredigeraren.
   <ul>
   <li>Dela och arkivera mappåtgärder för e-post till Designer-resurser.</li>
   <li>Dela mappar mellan arbetsytor, högerklicka på en mapp för att skapa en ny resurs, flytta resurser via dra och släpp.</li>
   </ul>
   </td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - API</strong>: Nu kan du använda API-anrop för e-post-Designer.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Hantering av plocklistor</strong>: Ange de värden som kan användas i fält i Marketo-gränssnittet.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - FUNKTION</strong>: Beskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - FUNKTION</strong>: Beskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - FUNKTION</strong>: Beskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 mars 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör den 31 mars 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
