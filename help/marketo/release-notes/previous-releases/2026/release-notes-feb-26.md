---
description: Versionsinformation - februari 2026 - Marketo Docs - produktdokumentation
title: Versionsinformation - februari 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 937c4a43066f957ddbeab9363174bc04e9a7d718
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 1%

---

# Versionsinformation: februari 2026 {#release-notes-feb-26}

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
   <td><strong>Skicka e-post till Designer - Kvalitetskontroll av varumärket</strong>: Utvärdera den allmänna innehållskvaliteten för att identifiera potentiella problem med läsbarhet, innehållets enhetlighet och effektivitet, oberoende av varumärkesriktlinjerna.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - AI Assistant Image Generation</strong>: Förutom Firefly kan du nu använda Nano Banana-modeller för att generera bilder med AI Assistant för e-postinnehåll.</td>
   <td>Frisläppt</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Skapa innehåll för ett visst avsnitt i e-postmeddelandet</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Borttagning av SEO-funktioner**: tisdagen den 31 mars 2026 kommer Marketo Engage att ersätta sökmotoroptimeringsfunktionen (SEO). Om du inte aktivt använder SEO behöver du inte göra någonting. Om du nyligen har använt SEO kan du exportera dina data. [Läs mer](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **REST API-sammanslagningslead-gräns**: Från och med 31 mars 2026 resulterar anrop som innehåller fler än 25 ID:n i leadIds-parametern i ett API-anrop för sammanslagningsleads i en felkod på 1080 och anropet hoppas över. Jobb som kräver sammanslagning av mer än 25 poster till ett bör delas upp i flera jobb för att säkerställa att dessa samtal blir framgångsrika.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 juli 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 juli 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
