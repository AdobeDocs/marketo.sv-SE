---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 96050d108aae64bbdab377cf5e31392df177b363
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 2%

---

# Versionsinformation: januari 2026 {#release-notes-jan-26}

Här nedan hittar du alla funktioner som ingår i versionen från 26 januari. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

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
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FUNKTIONSTITEL</strong>: Funktionsbeskrivning.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Adobe Connect Features {#adobe-connect-features}

Dessa funktioner har redan släppts av Adobe Connect team. Marketo Engage [Interaktiva webbinarier](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} drivs av Adobe Connect. Därför gäller funktionerna nedan endast användare av interaktiva webbinarier.

* **Survey Pod**: Adobe Connect 12.11 introducerar en ny Survey Pod som gör det möjligt för värdar att utforma och leverera strukturerade feedbackformulär direkt under en live-session.

* **Resurspanel**: Den nya resurspanelen ersätter de tidigare rutorna för filer och webblänkar, vilket ger ett enda enhetligt sätt att dela resurser under livesessioner.

* **Förbättrat rumsgränssnitt**: I Adobe Connect 12.11 introduceras ett uppdaterat och modernare rumsgränssnitt som bygger på Adobe senaste Spectrum 2-designramverk och som anpassar sig till det visuella språk som används i andra Adobe-produkter som Creative Cloud och Experience Cloud.

Fullständig information finns i [versionsinformationen för Adobe Connect 12.11](https://helpx.adobe.com/se/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Meddelanden {#announcements}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 mars 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör den 31 mars 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Marketo Engage Identity End of Life**:

   * _Borttagning av IP-begränsningar_: Stöd för [Begränsa Marketo-inloggningar baserat på IP](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. En ny platsbaserad åtkomstkontrollsfunktion för Adobe Identity i Adobe Admin Console kommer snart.

   * _Borttagning av enkel inloggning (SSO)_: Stöd för [Marketo Identity SSO](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} upphörde den 30 juli 2025. Funktionen kommer att fortsätta att fungera tills övergången till Adobe Identity är klar. Single Sign-On för Adobe Identity i Adobe Admin Console måste konfigureras separat. Inställningssteg finns i [Konfigurera identitet och enkel inloggning](https://helpx.adobe.com/se/enterprise/using/set-up-identity.html){target="_blank"}.
