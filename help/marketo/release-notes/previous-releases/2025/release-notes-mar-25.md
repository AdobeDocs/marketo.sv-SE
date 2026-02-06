---
description: Versionsinformation - mars 2025 - Marketo Docs - produktdokumentation
title: Versionsinformation - mars 2025
feature: Release Information
exl-id: a0e45d8e-6b74-4ab0-a1ba-4dae3754bc8f
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 2%

---

# Versionsinformation: Mars 2025 {#release-notes-mar-25}

Här nedan hittar du alla funktioner som finns i mars 25. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **28 mars 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr>
   <td><strong>E-post för Designer finns i alla program</strong>: Designer nya e-postmeddelanden är nu tillgängliga i alla engagemangs-, standard- och händelseprogram (med det enda undantaget för interaktiva webbinariprogram). Tidigare var de bara tillgängliga i e-postprogram.</td>
   <td>Frisläppt</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>GenAI-funktioner i interaktiva webbinarier</strong>: Nu kan du generera både kapitel och en sammanfattning för on demand-webbinarier. Redigera och exportera en HTML-fil med dina data.</td>
   <td>Frisläppt</td>
   <td><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai">GenAI-funktioner</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Global och Workspace My Tokens</strong>: Konfigurera mina tokens både på arbetsytan och på global nivå för att möjliggöra ökad produktivitet och kontroll över varumärkes- och marknadsföringsmaterial på Marketo Engage arbetsytor och till och med hela instanser.</td>
   <td>Frisläppt</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md#create-a-my-token">Skapa en global My Token</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Borttagning av sociala funktioner**: Onsdagen den 31 juli 2024 började Marketo Engage ta bort följande sociala funktioner i produkten:

   * Omröstningar
   * Knappen Socialt
   * Värvningserbjudande
   * Videodelning
   * Dragningar

Sedan dess har användare inte kunnat skapa, klona eller bädda in någon av dessa sociala funktioner i Marketo Engage. Befintliga sociala tillgångar fortsätter att fungera fram till 31 januari 2025. Den 1 februari 2025 upphörde sociala tillgångar att fungera. Alla inbäddade sociala funktioner i landningssidor måste tas bort. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 mars 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör den 31 mars 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Ny analysfunktion - offentlig Beta**: [Avancerad BI-analys](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (kallades tidigare Intresseutforskaren och avancerad Report Builder) börjar distribueras till alla aktuella Intäktscyklutforskaranvändare i mitten av april. Det nya verktyget erbjuder ett flexibelt gränssnitt för rapportering och visualisering av data från Marketo Engage, med detaljerad information om utveckling, prestanda och mycket annat. Den har bättre interaktivitet och visualisering, snabbare prestanda och en smidigare och mer intuitiv användarupplevelse.

För att få tillgång till den här funktionen måste du ha köpt tillägget Avancerad BI Analytics. Kontakta Adobe Account Team (din kontoansvarige) för mer information.
