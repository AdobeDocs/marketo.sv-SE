---
description: Aktuell versionsinformation – Marketo Docs – produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ea9bf2a002415936cdfb5bfb723ce80723003da5
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 2%

---

# Versionsinformation: juli 2024 {#release-notes-july-24}

Här nedan hittar du alla funktioner som ingår i versionen från 24 juni. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner faller under standardversionscykeln och kommer att släppas den **26 juli 2024**, med en stegvis utrullning av återstående funktioner under de följande veckorna. Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Marketo REST API-ändring</strong>: Vi introducerar en mindre ändring av <a href="https://developers.marketo.com/rest-api/user-management/">API för användarhantering</a>. Båda <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Bläddra bland användare</a> och <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Ta bort användare</a> slutpunkter har nu stöd <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Hantering av målkonto</a> -användare.</td> 
   <td><i>kommer snart</i></td>
   <td><i>kommer snart</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **Ny dokumentationswebbplats för utvecklare**: Som en del av vårt fortsatta arbete med att förbättra användarupplevelsen i Marketo Engage kommer vi att migrera all utvecklardokumentation till Adobe Experience League och Adobe Developer webbplats i juli 2024. [Läs mer](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Åtkomsttoken i borttagning av frågeparameter**: Stöd för autentisering med hjälp av åtkomsttoken i en frågeparameter för ett Marketo Engage REST API-anrop kommer att tas bort i en framtida version (specifikt datum för TBD). Befintliga integreringar bör migreras till användningen av auktoriseringshuvudet [beskrivs här](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Ny utveckling bör endast använda auktoriseringshuvudet för autentisering med Marketo Engage.

* **LinkedIn-omautentisering krävs**: LinkedIn uppgraderar sina Marketing API:er som används av integreringar med Marketo Engage LinkedIn. Dessa ändringar kräver omautentisering av alla LinkedIn LaunchPoint-tjänster i din **Administratör** > **LaunchPoint** meny mellan 26 juli och 15 december 2024 för att undvika avbrott i tjänsten. Du hittar instruktioner om hur du gör detta [här för Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} och [här för Matched Auditions](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Tjänsten Lead Gen Form har en typ av&quot;LinkedIn Lead Gen&quot; och tjänsten Matched Audience har typen&quot;LinkedIn Matched Audiences&quot;. Mer information finns i [Vanliga frågor om migrering](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
