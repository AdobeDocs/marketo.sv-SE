---
description: Versionsinformation - augusti 2025 - Marketo Docs - produktdokumentation
title: Versionsinformation - augusti 2025
feature: Release Information
source-git-commit: 95dda7d6e09f0e64fbce8e5bd39613f10ebde382
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Versionsinformation: augusti 2025 {#release-notes-aug-25}

Här nedan hittar du alla funktioner som finns i augusti 25. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den 22 augusti 2025 **, med en fasad utrullning av återstående funktioner under de följande veckorna.** Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>E-posta Designer - Rapporter</strong>: Prestanda för e-post och e-postlänk visar nu data från e-postmeddelanden som skapats med den nya e-postfunktionen Designer.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - Automatisk borttagning</strong>: Alternativet Autocomplete i redigeraren för tokenanpassning pekar på felaktiga objekt och har tagits bort. För närvarande finns det inga planer på att återimplementera den.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer för e-post - optimering av e-postförhandsgranskning</strong>: Vissa användare fick en långsammare inläsningstid när de försökte förhandsgranska sin e-post på e-postmallens/fragmentinformationssidan. Den här upplevelsen har optimerats för upp till 60 % snabbare laddningstider.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-posta Designer - mallkorrigeringar</strong>: Vissa färdiga mallar hade problem med återgivningen (t.ex. inte korrekt återgivning i vissa webbläsare/mörkt läge, feljusterade bilder, felplacerade CTA-knappar och några andra). De här är åtgärdade i den här versionen.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-post-Designer - låsning av innehåll</strong>: Tidigare, om en e-postmall skapades med låsning av innehåll och mallen användes för att skapa ett e-postmeddelande, skulle innehållslåsning finnas kvar även när e-postmeddelandet återställdes eller när"ändra design" valdes. Problemet har åtgärdats i den här versionen.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Behörighet att redigera gränser för smarta kampanjer</strong>: Administratörer kan nu begränsa möjligheten att ändra gränserna för smarta kampanjer till endast behöriga användare.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Marketo Engage Identity End of Life**: I augusti 2025 började Adobe fasa ut stödet för Marketo Engage Identity (logga in via `login.marketo.com`). För att förhindra avbruten åtkomst till Marketo Engage måste du övergå till [Adobe Identity](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} senast den 30 september 2025.

   * _Borttagning av IP-begränsningar_: Stöd för [Begränsa Marketo-inloggningar baserat på IP](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. En ny platsbaserad åtkomstkontrollsfunktion för Adobe Identity i Adobe Admin Console kommer snart.

   * _Borttagning av enkel inloggning (SSO)_: Stöd för [Marketo Identity SSO](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. Single Sign-On för Adobe Identity i Adobe Admin Console måste konfigureras separat. Inställningssteg finns i [Konfigurera identitet och enkel inloggning](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

* **Borttagning av _Framåt till en vän_-funktion**: 29 september 2025 kommer funktionen _Framåt till en vän_ i e-postmeddelanden från Marketo Engage 2.0 (den gamla e-postredigeraren) att vara helt inaktuell för alla prenumerationer. Detta påverkar token &quot;Vidarebefordra till en vän&quot; och &quot;Vidarebefordra till en vän&quot; i e-postmeddelanden som redan har skickats eller kommer att skickas med denna token. [Läs mer](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 oktober 2025. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 oktober 2025. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
