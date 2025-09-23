---
description: Versionsinformation - maj 2025 - Marketo Docs - produktdokumentation
title: Versionsinformation - maj 2025
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Versionsinformation: maj 2025 {#release-notes-may-25}

Här nedan hittar du alla funktioner som ingår i versionen från maj 25. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **23 maj 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Rollbaserad åtkomstkontroll för e-post-Designer Assets</strong>: En ny förbättring av det rollbaserade åtkomstkontrollssystemet (RBAC) ger mer detaljerade behörigheter och förbättrad användarhantering för resurser som drivs av nya Email Designer.</td>
   <td>Levererat</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Detaljerade behörigheter för New Email Designer (bloggpost)</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Klona e-post som har skapats i e-postmeddelandet för Designer</strong>: Du kan nu klona ett befintligt e-postmeddelande som har skapats med den nya e-postversionen för Designer.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Utlösartoken för alla attribut</strong>: Utökad lista över utlösartoken som kan användas med data från alla aktivitetsattribut i smarta kampanjfält.</td>
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
 </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Integreringsuppdatering för offlinekonvertering för Facebook**: Den 29 maj 2025 migreras [Facebook-integreringen för offlinekonvertering](https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} för Marketo Engage till det nya Meta [Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"} , på grund av att Meta har ersatt [offlinekonverterings-API:t](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} i linje med Graph API-versionshantering. Mer information finns i Metas guide om att [skicka offlinehändelser via Conversions API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI för offline).

* **Ny analysfunktion - offentlig Beta**: [Avancerad BI-analys](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (kallades tidigare Intäktsutforskaren och avancerad Report Builder) började distribueras till alla nuvarande användare av intäktscykelutforskaren i mitten av april. Det nya verktyget erbjuder ett flexibelt gränssnitt för rapportering och visualisering av data från Marketo Engage, med detaljerad information om utveckling, prestanda och mycket annat. Den har bättre interaktivitet och visualisering, snabbare prestanda och en smidigare och mer intuitiv användarupplevelse.

För att få tillgång till den här funktionen måste du ha köpt tillägget Avancerad BI Analytics. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop är inaktuell och kommer inte att vara tillgänglig efter den 31 januari 2026. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 januari 2026. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
