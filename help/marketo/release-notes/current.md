---
description: Aktuell versionsinformation – Marketo Docs – Produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 97806e0df45327fb695f02c02af0dde42a602737
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Versionsinformation: oktober 2024 {#release-notes-oct-24}

Här nedan hittar du alla funktioner som ingår i versionen från 24 oktober. Se om det finns funktioner i Adobe Marketo Engage Edition.

Versionsinformationen för Adobe Dynamic Chat [ finns här](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

## Standardfunktioner för lanseringscykel {#standard-release-cycle-features}

Följande funktioner ingår i standardversionscykeln och kommer att släppas den 4 oktober 2024 **, med en stegvis utrullning av återstående funktioner under de följande veckorna.** Versionsfunktioner och datum kan komma att ändras. Kontrollera status bredvid varje funktion.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>Tokenisering för interaktiva webbinarier</strong>: Du kan nu använda tokens för att marknadsföra interaktiva webbinarier i e-postmeddelanden och landningssidor utan att behöva lägga till information om webbinariet manuellt.</td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Marknadsför ett interaktivt webbinarium</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Smart lista "Ange som påverkar" antal</strong>: Se hur många som påverkas när du redigerar kvalificeringsreglerna för en smart kampanj.</td> 
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Knappen Mitt konto i navigeringsfältet</strong>: För dem som har migrerat till Adobe Identity Management System kan du konfigurera din tidszon och få åtkomst till prenumerationsinformation genom att klicka på knappen Mitt konto i det vänstra navigeringsfältet.</td> 
   <td>Levererat</td>
   <td>n/a</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Förbättringar av e-postprestandarapport</strong>: Flera förbättringar har gjorts av e-postrapporteringsstatistik och aktivitetsspårning, vilket ger ytterligare insikter och förbättrar noggrannheten.
   <ul>
   <li>Filtrera borttagna och sammanfogade personer från mätvärden för e-postprestanda</li>
   <li>E-postmeddelanden som nu klassificerats som <i>avbrutna</i> efter att ha väntat i tre dagar på svarsaktivitet</li>
   <li>E-postöppningar räknas som unika öppna separat för varje smart kampanj</li>
   </td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Rapport om e-postprestanda</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Salesforce Sync Backlog Metrics</strong>: Övervaka genomströmning och trender för eftersläpning för att planera och schemalägga CRM-uppdateringar för en optimal synkroniseringsupplevelse.
   </td> 
   <td>Levererat</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce Sync Backlog Metrics</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Meddelanden {#announcements}

* **API-uppdatering för massextrahering**: Vi har åtgärdat ett fel i API:t för gruppextrahering som inkluderar alternativet columnHeaderNames, som gör att du kan ange anpassade kolumnrubriknamn i den exporterade filen. Tidigare kunde kolumnrubriknamn som innehöll icke-ASCII-tecken bli skadade.

* **Resten av API-parametern access_token har tagits bort**: Frågeparametern access_token som används för att autentisera Marketo REST API-anrop har tagits bort och är inte tillgänglig efter den 30 juni 2025. Alla nya och befintliga integreringar ska autentisera REST API-anrop med hjälp av Authorization-huvudet [ enligt beskrivningen här](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).


* **QR-kodborttagning**: Den 4 oktober 2024 kommer QR-kodfunktionen som används i push-meddelanden och meddelanderesurser i appen att bli inaktuell. Detta inkluderar användning av QR-koder för en ny testenhet samt skapande av nya resurser med QR-koder. Genom att ta bort funktioner med lägre användning kan vi omfördela deras resurser till det övergripande underhållet av Marketo Engage.

* **Munchkin-ändringar**

   * **Ny version**: Den 17 september 2024 börjar [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 att rulla ut till Marketo Engage-instanser där inställningen Munchkin Beta är aktiverad i **Admin** > **Resurs Chest**. Det är schemalagt att börja lansera till alla andra förekomster den 29 oktober. Den här versionen uppdaterar skapandet av Munchkin cookie. Det finns inga förändringar i funktionaliteten.

   * **Tecken från URL Borttagen**: Aktiviteterna Besök webbsida och Klicklänk som skapas av Munchkin JS tar nu bort kontrolltecken som inte är URL-kodade från alla URL-fält. Den här ändringen är avsedd att förhindra fel som beror på spridning av dessa typer av tecken till system som saknar stöd för dem, och som inte kan användas i Marketo Engage.
