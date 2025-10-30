---
description: Versionsinformation - september 2025 - Marketo Docs - produktdokumentation
title: Versionsinformation - september 2025
feature: Release Information
source-git-commit: 7f56808ec26ec28065cc974716a5eab66e1d38b3
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Versionsinformation: september 2025 {#release-notes-sep-25}

Här nedan hittar du alla funktioner som ingår i versionen från 25 september. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den 19 september 2025 **, med en fasad utrullning av återstående funktioner under de följande veckorna.** Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Bevaring av webbinariaktivitet på begäran</strong>: Interaktiva webbinarier-användare har nu tillgång till konsoldata för webbinariet på begäran i mer än 30 dagar (tidigare var det bara upp till 30 dagar från dagen för webbinariet).</td>
   <td>Levererat</td>
   <td><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/event-workflows#manual-sync">Manuell synkronisering</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - Innehåll i Collaboration Workflow</strong>: Nu kan du kommentera och samarbeta med andra Marketo-användare i en e-postresurs. Tagga teammedlemmar (Marketo-användare som har rätt resursbehörigheter) så får de ett e-postmeddelande eller ett pulsmeddelande.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Skicka e-post till Designer - AI Assistant-behörigheter</strong>: Marketo-administratörer kan ge vissa användare åtkomst till GenAI-funktioner.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">Konfigurera behörigheter</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - mörkt läge</strong>: Nu kan du använda mörkt läge, som gör att e-postklienter och appar kan visa e-postmeddelanden med mörkare bakgrund och ljusare färger för text, knappar och andra gränssnittselement.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">Mörkt läge</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-post-Designer - Omdirigeringskorrigeringar</strong>: Vissa användare hade problem med omdirigering av URL:er för e-postmeddelanden som skapats med den nya Designer-versionen (det gick inte alltid att klistra in URL:er direkt eller bokmärka e-postresurser). Problemet har åtgärdats. Dessutom kommer länkar till e-postresurser från <b>E-postmallar</b> &gt; <b>Detaljer</b> &gt; <b>Används av</b> att dirigera om till motsvarande e-postresurs.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **REST API Double Slash Deprecation**: 16 september 2025 gick Adobe över till en modernare värdinfrastruktur för REST API-URL:er som utnyttjar nyare teknik, vilket ger högre säkerhet och skalbarhet. Om din prenumeration har använt API:er med ett snedstreck (//) i URL:en läser du [det här Nation-inlägget](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} för nästa steg.

* **Växla tillbaka till snabbskriptning i den nya e-postversionen av Designer**: Adobe Marketo Engage har släppt en funktion som heter _Villkorligt innehåll_ för den nya e-postversionen av Designer i juni. Funktionen drivs av Handlebar-skriptning i stället för Snabb skriptning, i ett försök att ge lite mer flexibilitet i ditt dynamiska innehåll. Men när vi upptäckte att det orsakade att vissa tokens inte löstes korrekt bestämde vi oss för att tillfälligt inaktivera det. [Läs mer](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity End of Life**: I augusti 2025 började Adobe fasa ut stödet för Marketo Engage Identity (logga in via `login.marketo.com`). För att förhindra avbruten åtkomst till Marketo Engage måste du övergå till [Adobe Identity](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} senast den 30 september 2025.

   * _Borttagning av IP-begränsningar_: Stöd för [Begränsa Marketo-inloggningar baserat på IP](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. En ny platsbaserad åtkomstkontrollsfunktion för Adobe Identity i Adobe Admin Console kommer snart.

   * _Borttagning av enkel inloggning (SSO)_: Stöd för [Marketo Identity SSO](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. Single Sign-On för Adobe Identity i Adobe Admin Console måste konfigureras separat. Inställningssteg finns i [Konfigurera identitet och enkel inloggning](https://helpx.adobe.com/se/enterprise/using/set-up-identity.html){target="_blank"}.

* **Borttagning av _Framåt till en vän_-funktion**: 29 september 2025 kommer funktionen _Framåt till en vän_ i e-postmeddelanden från Marketo Engage 2.0 (den gamla e-postredigeraren) att vara helt inaktuell för alla prenumerationer. Detta påverkar token &quot;Vidarebefordra till en vän&quot; och &quot;Vidarebefordra till en vän&quot; i e-postmeddelanden som redan har skickats eller kommer att skickas med denna token. [Läs mer](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop är inaktuell och kommer inte att vara tillgänglig efter den 31 januari 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 januari 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
