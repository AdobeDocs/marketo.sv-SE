---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 1850dd03baba259e99e8cc089b39f35735e63fdf
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 2%

---

# Versionsinformation: mars 2026 {#release-notes-mar-26}

Här nedan hittar du alla funktioner som ingår i mars 26. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **27 mars 2026**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - Hantera varumärken (beta)</strong>: Generera e-postinnehåll baserat på din organisations/varumärkes specifika riktlinjer för copywriting.</td>
   <td>Frisläppt</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">Skapa och hantera varumärken</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - snabbåtgärder</strong>: <i>Paritet med den gamla e-postredigeraren</i>. Snabbåtgärder är nu tillgängliga för alla e-postresurser i Designer (e-post, e-postmallar, fragment). Följande snabbåtgärder stöds: Duplicera, Ta bort, Flytta, Skapa/redigera utkast.
   </td>
   <td>Frisläppt</i></td>
   <td>n/a</td>
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
   <td><strong>E-posta Designer - Outlook-återgivningskorrigering</strong>: Den här uppdateringen åtgärdar återgivningsproblem, särskilt i MS Outlook. I expertläget kan du göra mindre HTML-/CSS-redigeringar eller lägga till script-taggar i e-postmeddelandet (det bästa sättet är att inte göra några andra ändringar i e-postmeddelandets HTML för att behålla de visuella elementen som de är).
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
   <td><strong>Hantering av plocklistor</strong>: Nu kan du ange värden som kan användas i fält i Marketo Engage.
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
   <td><strong>Push-meddelanden</strong>: Omdirigerings-URL:er som konfigurerats i push-meddelanden har nu stöd för Marketo Engage-tokens (gäller endast <i>Starta program-URL:er</i>).
   </td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Borttagning av SEO-funktioner**: tisdagen den 31 mars 2026 kommer Marketo Engage att ersätta sökmotoroptimeringsfunktionen (SEO). Om du inte aktivt använder SEO behöver du inte göra någonting. Om du nyligen har använt SEO kan du exportera dina data. [Läs mer](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **REST API-sammanslagningslead-gräns**: Från och med 31 mars 2026 resulterar anrop som innehåller fler än 25 ID:n i leadIds-parametern i ett API-anrop för sammanslagningsleads i en felkod på 1080 och anropet hoppas över. Jobb som kräver sammanslagning av mer än 25 poster till ett bör delas upp i flera jobb för att säkerställa att dessa samtal blir framgångsrika.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 juli 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 juli 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
