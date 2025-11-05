---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 588ec23961df42de8a8c0aed919ba9a016b61f18
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 1%

---

# Versionsinformation: oktober 2025 {#release-notes-oct-25}

Här nedan hittar du alla funktioner som ingår i versionen från 25 oktober. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **31 oktober 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - mallimporterare (Beta)</strong>: Importera e-postmallar från den klassiska e-postredigeraren för att skapa mallar som är kompatibla med nya e-post-Designer i Design Studio.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Import av mallar</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - villkorligt innehåll</strong>: Paritetsfunktionen för den nya e-postfunktionen Designer, som gör att du kan skapa e-postpersonalisering utöver token.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - A/B-testning</strong>: Paritetsfunktionen för den nya e-postversionen av Designer, så att du kan utföra A/B-tester för att se vilka typer av innehåll som får bäst svar.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - varumärkesteman</strong>: Nu kan du definiera varumärkesteman i Marketo Engage. Formatkonfigurationer kan återanvändas och användas i alla e-postmallar och andra e-postresurser för enhetlig varumärkesexponering.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>Skicka e-post till Designer - bild till HTML Converter</strong>: Överför en kompatibel PNG/JPEG-bildfil av ett e-postmeddelande och den konverteras automatiskt till HTML för användning i det nya e-postmeddelandet till Designer.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - klona e-poståtgärd</strong>: Nu kan du klona ett e-postmeddelande till en annan programmapp i marknadsföringsaktiviteter och snabbt återanvända befintliga e-postmeddelanden.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Salesforce CRM-integrationsuppgradering**: En ny version av den inbyggda CRM-integreringen kommer att distribueras till aktiva sandlådor där den inbyggda kopplingen är aktiverad under sju dagar från och med 13 november 2025. Få fullständig information i [det här Nation-inlägget](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}

* **REST API Double Slash Deprecation**: 16 september 2025 gick Adobe över till en modernare värdinfrastruktur för REST API-URL:er som utnyttjar nyare teknik, vilket ger högre säkerhet och skalbarhet. Om din prenumeration har använt API:er med ett snedstreck (//) i URL:en läser du [det här Nation-inlägget](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} för nästa steg.

* **Växla tillbaka till snabbskriptning i den nya e-postversionen av Designer**: Adobe Marketo Engage har släppt en funktion som heter _Villkorligt innehåll_ för den nya e-postversionen av Designer i juni. Funktionen drivs av Handlebar-skriptning i stället för Snabb skriptning, i ett försök att ge lite mer flexibilitet i ditt dynamiska innehåll. Men när vi upptäckte att det orsakade att vissa tokens inte löstes korrekt bestämde vi oss för att tillfälligt inaktivera det. [Läs mer](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity End of Life**: I augusti 2025 började Adobe fasa ut stödet för Marketo Engage Identity (logga in via `login.marketo.com`). För att förhindra avbruten åtkomst till Marketo Engage måste du övergå till [Adobe Identity](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} senast den 30 september 2025.

   * _Borttagning av IP-begränsningar_: Stöd för [Begränsa Marketo-inloggningar baserat på IP](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. En ny platsbaserad åtkomstkontrollsfunktion för Adobe Identity i Adobe Admin Console kommer snart.

   * _Borttagning av enkel inloggning (SSO)_: Stöd för [Marketo Identity SSO](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. Single Sign-On för Adobe Identity i Adobe Admin Console måste konfigureras separat. Inställningssteg finns i [Konfigurera identitet och enkel inloggning](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

* **Borttagning av _Framåt till en vän_-funktion**: 29 september 2025 togs funktionen _Framåt till en vän_ bort helt för alla prenumerationer i e-postmeddelanden från Marketo Engage 2.0 (den gamla e-postredigeraren). Detta påverkade token &quot;Vidarebefordra till en vän&quot; och &quot;Vidarebefordra till en vän&quot; i e-postmeddelanden som redan har eller var planerade att skickas med token. [Läs mer](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop är inaktuell och kommer inte att vara tillgänglig efter den 31 januari 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 januari 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
