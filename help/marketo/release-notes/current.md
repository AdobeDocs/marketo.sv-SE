---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 978bbe4de06a0e269b60108e5a91edc5499dc9c1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 3%

---

# Versionsinformation: Mars 2025 {#release-notes-mar-25}

Här nedan hittar du alla funktioner som finns i mars 25. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md).

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Funktioner för standardutgåva av cykeln {#standard-release-cycle-features}

Följande funktioner faller under standardlanseringscykeln och börjar släppas den **28 mars 2025**, med en stegvis distribution av återstående funktioner under de efterföljande veckorna. Lanseringsfunktioner och datum kan komma att ändras. Kontrollera bredvid varje funktion för dess status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>E-post för Designer finns i alla program</strong>: Designer nya e-postmeddelanden är nu tillgängliga i alla engagemangs-, standard- och händelseprogram (med det enda undantaget för interaktiva webbinariprogram). Tidigare var de bara tillgängliga i e-postprogram. Med den här uppdateringen blir kloning också tillgänglig.</td>
   <td>Levereras</td>
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>GenAI-funktioner i interaktiva webbinarier</strong>: Nu kan du generera både kapitel och en sammanfattning för on demand-webbinarier. Redigera och exportera en HTML-fil med dina data.</td>
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Global och Workspace My Tokens</strong>: Konfigurera mina tokens både på arbetsytan och på global nivå för att möjliggöra ökad produktivitet och kontroll över varumärkes- och marknadsföringsmaterial på Marketo Engage arbetsytor och till och med hela instanser.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Token för alla utlösarattribut</strong>: Expanderar listan över tillgängliga utlösartoken från enbart listan i <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">det här dokumentet</a> så att den stöder användning av data från alla utlösande aktivitetsattribut i kampanjflödesfält. Skriv ut data från ett aktivitetsattribut till ett intressant ögonblick eller ange ett lead-ID för senaste transaktion från en anpassad aktivitet till ett lead-fält.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Utfasning** av sociala funktioner: Onsdagen den 31 juli 2024 påbörjade Marketo Engage utfasningen av följande sociala funktioner i produkten:

   * Omröstningar
   * Knappen Socialt
   * Värvningserbjudande
   * Videodelning
   * Dragningar

Sedan dess har användare inte kunnat skapa, klona eller bädda in någon av dessa sociala funktioner i Marketo Engage. Befintliga sociala tillgångar fortsätter att fungera fram till 31 januari 2025. Den 1 februari 2025 upphörde sociala tillgångar att fungera. Alla inbäddade sociala funktioner i landningssidor måste tas bort. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977)

* **Utfasning** av REST API-access_token-parametrar: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop håller på att tas bort och kommer inte att vara tillgänglig efter den 30 juni 2025. Alla nya och befintliga integreringar bör autentisera REST API-anrop med hjälp av rubriken &quot;Auktorisering&quot;, [enligt beskrivningen här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication).

* **Utfasning** av SOAP API: Stödet för Marketo SOAP API upphör den 31 oktober 2025. Tjänster som använder SOAP API-funktioner bör migreras [till REST API.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api)

* **Ny Analytics-funktion – Public Beta**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md) (tidigare känt som Revenue Explorer och Advanced Report Builder) börjar rullas ut till alla nuvarande Revenue Cycle Explorer-användare i mitten av april. Det här nya verktyget erbjuder ett flexibelt gränssnitt för rapportering och visualisering av Marketo Engage-data, vilket ger detaljerad information om framsteg, prestanda med mera. Den har rikare interaktivitet och visualisering, snabbare prestanda och en mer sömlös och intuitiv användarupplevelse.

För att få tillgång till den här funktionen måste du ha köpt tillägget Advanced BI Analytics. Kontakta kontoteamet för Adobe (din kontoansvarige) om du vill ha mer information.
