---
description: Aktuell versionsinformation – Marketo Docs – produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 1839ccb646e775b67efa8de7d2d2bf3dbbbefa72
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 2%

---

# Versionsinformation: juli 2024 {#release-notes-july-24}

Här nedan hittar du alla funktioner som finns i juliversionen från 24. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [ finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den **26 juli 2024**, med en fasad utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Engagement Dashboard för interaktiva webbinarier</strong>: Skaffa en sammanställd vy för webbinariets prestanda samt en heltäckande bild av engagemanget för varje deltagare under webbinariet så att ni kan bestämma vilka som leder till mål med hjälp av Marketo Engage verktyg för samordning.</td> 
    <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Instrumentpanel för engagemang</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Rumshantering för interaktiva webbinarier</strong>: Få tillgång till enskilda rum som har skapats (och gör ändringar om det behövs) samt få tillgång till innehållet och inspelningen (och rensa dem om det behövs för att optimera lagringen).</td> 
    <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Rumshantering</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Anpassning av webbinarium för interaktiva webbinarier</strong>: Skapa en enhetlig varumärkesupplevelse som godkänts av organisationen genom att använda ett gemensamt rumsgränssnitt, mellanskärmar (t.ex. bakgrunder för deltagande på skärmen) samt anpassade videobakgrunder, så att webbinaristrategi enklare kan anpassas efter varumärkesstrategin.</td> 
    <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Anpassning av interaktiva webbinarier</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API-ändring</strong>: Vi introducerar en mindre ändring i <a href="https://developers.marketo.com/rest-api/user-management/">API:t för användarhantering</a>. Både slutpunkterna <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Bläddra bland användare</a> och <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Ta bort användare</a> har nu stöd för <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">målkontohanteringsanvändare</a>.</td> 
   <td><i>Kommer snart</i></td>
   <td><i>Kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Ny dokumentationswebbplats för utvecklare**: Som en del av vårt fortsatta arbete med att förbättra användarupplevelsen för Marketo Engage migrerar vi all utvecklardokumentation till Adobe Experience League och Adobe Developer webbplats i juli 2024. [Läs mer](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Borttagning av sociala funktioner**: Onsdagen den 31 juli 2024 börjar Marketo Engage ta bort följande sociala funktioner i produkten:

   * Omröstningar
   * Knappen Socialt
   * Värvningserbjudande
   * Videodelning
   * Dragningar

Användare kommer inte längre att kunna skapa, klona eller bädda in någon av dessa sociala funktioner i Marketo Engage. Befintliga sociala resurser kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Åtkomsttoken i borttagning av frågeparametrar**: Stöd för autentisering med åtkomsttoken i en frågeparameter i ett Marketo Engage REST API-anrop kommer att tas bort i en framtida version (TBD för specifikt datum). Befintliga integreringar ska migreras till användning av auktoriseringshuvudet [som beskrivs här](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Ny utveckling bör endast använda auktoriseringshuvudet för autentisering med Marketo Engage.

* **LinkedIn-omautentisering krävs**: LinkedIn uppgraderar sina Marketing API:er som används av Marketo Engage LinkedIn-integreringar. Dessa ändringar kräver omautentisering av alla LinkedIn LaunchPoint-tjänster på **Admin** > **LaunchPoint** -menyn mellan 26 juli och 15 december 2024 för att undvika avbrott i tjänsten. Du hittar instruktioner om hur du slutför denna [här för Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} och [här för Matchade målgrupper](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Tjänsten Lead Gen Form har en typ av&quot;LinkedIn Lead Gen&quot; och tjänsten Matched Audience har typen&quot;LinkedIn Matched Audiences&quot;. Mer information finns i [Vanliga frågor om migrering](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
