---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 2%

---

# Versionsinformation: januari 2026 {#release-notes-jan-26}

Här nedan hittar du alla funktioner som ingår i versionen från 26 januari. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **30 januari 2026**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - Hantera varumärken (beta)</strong>: Generera e-postinnehåll baserat på din organisations/varumärkes specifika riktlinjer för copywriting.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - AI Assistant Enhancement</strong>: Nu kan du lägga till varumärkesresurser direkt i din uppmaning och be modellen referera till den källan för att generera innehåll, i stället för att manuellt lägga till en varumärkesresurs som en fil.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - visuella förhandsvisningar för fragment</strong>: Alla publicerade fragment visas nu som miniatyrbilder, vilket gör det mycket snabbare att identifiera det du behöver.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - Punkter</strong>: Nu kan du skapa punkter på flera nivåer när du redigerar ett e-postmeddelande i Designer för e-post.</td>
   <td>Frisläppt</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - Villkorligt innehåll</strong>: Paritet med funktionen <i>Dynamiskt innehåll</i> i den gamla e-postredigeraren.
   <ul>
   <li>Villkorligt innehåll gäller nu för segmentering i delade mappar.</li>
   <li>Segmenteringar sorteras nu i alfabetisk ordning.</li>
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
   <td><strong>Skicka e-post till Designer - mappar</strong>: Nu kan du ordna dina resurser som skapats med e-post-Designer (e-post, e-postmallar, fragment) med mappar.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Funktioner för icke-standard-releasecykel {#non-standard-release-cycle-features}

Följande funktioner släpptes utanför Marketo Engage standardversionscykel.

### Interaktiva webbinarier {#interactive-webinars}

* **Undersökningsruta**: Med en ny undersökningsruta kan värdarna utforma och leverera strukturerade feedbackformulär direkt i en livesession.

* **Resurspanel**: Den nya resurspanelen ersätter de tidigare rutorna för filer och webblänkar, vilket ger ett enda enhetligt sätt att dela resurser under livesessioner.

* **Förbättrat rumsgränssnitt**: Dra nytta av ett uppdaterat och modernare rumsgränssnitt som bygger på Adobe senaste Spectrum 2-ramverk och som är anpassat till det visuella språk som används i andra Adobe-produkter som Creative Cloud och Experience Cloud.

Mer information finns på [den här sidan](https://helpx.adobe.com/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Meddelanden {#announcements}

* **Marketo Community Migration Complete**: Den nya Adobe Experience League-communityn finns nu tillgänglig! [Flera förbättringar](https://experienceleaguecommunities.adobe.com/community-pulse-blog-34/community-update-streamlined-ways-to-engage-and-a-redesigned-homepage-247673){target="_blank"} har gjorts för att göra Marketo Community ännu bättre. [Kolla in det](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-26){target="_blank"}.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 mars 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör den 31 mars 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
