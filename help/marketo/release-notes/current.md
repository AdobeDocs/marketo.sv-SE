---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuella utgivningsnoter
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 733b85495632eaa31ce7fc08a82fb4948aadf29f
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 1%

---

# Releasenoteringar: oktober 2025 {#release-notes-oct-25}

Nedan hittar du alla funktioner som ingår i oktober-25-utgåvan. Kolla din Adobe Marketo Engage-utgåva för tillgänglighet av funktioner.

Release Notes specifikt för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner markerade med en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Vänligen kontakta din Marketo Engage-representant för att få veta mer.

## Standardutgivningscykelfunktioner {#standard-release-cycle-features}

Följande funktioner omfattas av den vanliga releasecykeln och kommer att börja släppas den **31 oktober 2025**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Utgivningsfunktioner och datum kan ändras. Vänligen kontrollera vid varje funktion för dess status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Template Importer (Beta):</strong> Importera e-postmallar från den klassiska e-postredigeraren för att skapa mallar kompatibla med New Email Designer i Design Studio.</td>
   <td>Skeppat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Mallimport</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-postdesigner – Varumärkesteman</strong>: Du kan nu definiera varumärkesteman inom Marketo Engage. Stylingkonfigurationer kan återanvändas och tillämpas på e-postmallar och andra e-postresurser för varumärkets konsistens.</td>
   <td>Skeppat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brand-themes.md" target="_blank">Varumärkesteman</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Villkorat innehåll</strong>: Paritetsfunktion för den nya Email Designer, som låter dig uppnå e-postpersonalisering utöver tokens.</td>
   <td>Skeppat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/conditional-content.md" target="_blank">Villkorat innehåll</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>E-postdesigner – Bild-till-HTML-omvandlare</strong>: Ladda upp en kompatibel PNG/JPEG-bildfil av ett e-postmeddelande så konverteras den automatiskt till HTML för användning i den nya e-postdesignern.</td>
   <td>Skeppat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/image-to-html.md" target="_blank">Konvertera bilder till HTML-mallar</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-postdesigner - Klona e-poståtgärd</strong>: Du kan nu klona ett mejl till en annan programmapp i Marknadsföringsaktiviteter och snabbt återanvända befintliga e-postmeddelanden.</td>
   <td>Skeppat</td>
   <td>ej tillgängligt</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - A/B-testning</strong>: Paritetsfunktion för den nya Email Designer, som låter dig utföra A/B-tester för att se vilka typer av innehåll som får bäst respons.</td>
   <td>Skeppat</td>
   <td>ej tillgängligt</td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Salesforce CRM-integrationsuppgradering: En** ny version av den inbyggda CRM-integrationen kommer att distribueras till aktiva sandlådor som har den inbyggda kontakten aktiverad under sju dagar, med start den 13 november 2025. Få fullständiga detaljer i [detta Nation-inlägg](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}

* **REST API dubbel snedskärning av** snedstreck: Den 16 september 2025 övergick Adobe till en modernare hostinginfrastruktur för REST API-URL:er som utnyttjar nyare teknik och tillför säkerhet och skalbarhet. Om din prenumeration har använt API:er med dubbel framåtsnedstreck (//) i URL:en, vänligen läs [detta Nation-inlägg](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} för nästa steg.

* **Att återgå till Velocity Scripting i den nya Email Designer**: Adobe Marketo Engage släppte en funktion kallad _Villkorat innehåll_ för den nya Email Designer i juni i år. Funktionen drevs av Handlebar-skriptning istället för Velocity-skriptning, i ett försök att ge lite mer flexibilitet i ditt dynamiska innehåll. Men när vi upptäckte att det orsakade att vissa tokens löstes fel, bestämde vi oss för att tillfälligt inaktivera det. [Lära sig mer](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity Slutet på livslängden**: I augusti 2025 började Adobe fasa ut stödet för Marketo Engage Identity (inloggning via `login.marketo.com`). För att förhindra avbruten åtkomst till Marketo Engage måste du övergå till [Adobe Identity](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} senast den 30 september 2025.

   * _Avveckling_ av IP-begränsningar: Stöd för [att begränsa Marketo-inloggningar baserat på IP](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att vara i drift tills övergången till Adobe Identity är klar. En ny platsbaserad åtkomstkontrollfunktion för Adobe Identity i Adobe Admin Console kommer snart.

   * _Single Sign-On (SSO) avveckling_: Stödet för [Marketo Identity SSO](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att vara i drift tills övergången till Adobe Identity är klar. Single Sign-On för Adobe Identity i Adobe Admin Console måste konfigureras separat. För installationssteg, se [Sätt upp identitet och Single Sign-On](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

* **Avveckling av _funktionen_ Vidarebefordra till en vän**: Den 29 september 2025 _togs funktionen Vidarebefordra till en vän_ i Marketo Engage 2.0-mejl (den äldre e-postredigeraren) helt bort för alla prenumerationer. Detta påverkade länkarna &#39;Vidarebefordra till en vän&#39;-token och &#39;Vidarebefordra till en vän&#39;-länkarna i e-postmeddelanden som redan hade skickats eller var schemalagda att skickas med token. [Läs mer](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API &#39;access_token&#39; parameteravskaffning**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop är föråldrad och kommer inte att vara tillgänglig efter den 31 mars 2026. Alla nya och befintliga integrationer bör autentisera REST API-anrop med hjälp av headern &#39;Authorization&#39;, [som beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **SOAP API-avveckling**: Stödet för Marketo SOAP API upphör den 31 mars 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}
