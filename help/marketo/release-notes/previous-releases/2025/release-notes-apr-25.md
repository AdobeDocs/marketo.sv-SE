---
description: Versionsinformation - april 2025 - Marketo Docs - produktdokumentation
title: Versionsinformation - april 2025
feature: Release Information
exl-id: 94010780-41aa-4212-a1d4-1b78806bd728
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 2%

---

# Versionsinformation: april 2025 {#release-notes-apr-25}

Här nedan hittar du alla funktioner som ingår i versionen från 25 april. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **25 april 2025**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>SSL (Secure Socket Layer) Self Service</strong>: Med SSL-kryptering kan du göra landningssidor för en Marketo Engage-instans säkra. Om du aktiverar den här funktionen tidigare behöver du hjälp av Adobe supportteam. Marketo-användare kan nu aktivera programmet på egen hand, vilket sparar värdefull tid.</td>
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-ssl-to-your-landing-pages.md">Lägg till SSL på era landningssidor</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Meddelanden {#announcements}

* **Ny analysfunktion - offentlig Beta**: [Avancerad BI-analys](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (kallades tidigare Intresseutforskaren och avancerad Report Builder) börjar distribueras till alla aktuella Intäktscyklutforskaranvändare i mitten av april. Det nya verktyget erbjuder ett flexibelt gränssnitt för rapportering och visualisering av data från Marketo Engage, med detaljerad information om utveckling, prestanda och mycket annat. Den har bättre interaktivitet och visualisering, snabbare prestanda och en smidigare och mer intuitiv användarupplevelse.

För att få tillgång till den här funktionen måste du ha köpt tillägget Avancerad BI Analytics. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

* **Resten av API:t &#39;access_token&#39;-parametern har tagits bort**: Frågeparametern `access_token` som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 31 oktober 2025. Alla nya och befintliga integreringar ska autentisera REST API-anrop med rubriken Authorization, [, vilket beskrivs här](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Borttagning av SOAP API**: Stödet för Marketo SOAP API upphör 31 oktober 2025. Tjänster som använder SOAP API-funktioner bör migreras till [REST API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Borttagning av sociala funktioner**: Onsdagen den 31 juli 2024 började Marketo Engage ta bort följande sociala funktioner i produkten:

   * Omröstningar
   * Knappen Socialt
   * Värvningserbjudande
   * Videodelning
   * Dragningar

Sedan dess har användare inte kunnat skapa, klona eller bädda in någon av dessa sociala funktioner i Marketo Engage. Befintliga sociala tillgångar fortsätter att fungera fram till 31 januari 2025. Den 1 februari 2025 upphörde sociala tillgångar att fungera. Alla inbäddade sociala funktioner i landningssidor måste tas bort. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
