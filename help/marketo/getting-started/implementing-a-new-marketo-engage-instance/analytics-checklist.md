---
description: NYTT OMRÅDESANALYS - Marketo Docs - produktdokumentation
title: New Instance Best Practices - Analytics Checklist
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: ae40e26966ed85da9c55fc510732841fa1e5212a
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 0%

---

# NYTT OMRÅDE: Analyschecklista {#new-area-analytics-checklist}

I avsnittet Analytics (Analyser) finns globala rapporter som analyserar resultatet av era marknadsföringssatsningar. Lär dig hur du navigerar i dem.

Kom ihåg [ladda ned checklistor](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) och spåra dina framsteg.

## Träd {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organisation: Namngivning, mappar och arkivering <br> </td>
    <td>Använd en namngivningskonvention för rapporter för att skilja på rapporter på fliken Globala rapporter. <br>Ett exempel på god praxis för namngivning är [rapporttyp] [Global vs. BU-specifik tagg] [Rapportbeskrivning], till exempel [E-postprestanda]-[Global]-[180 dagars e-poståtagande].  <br>Identifiera rapporter som ska delas med olika användargrupper inom organisationen (t.ex. säljteam, ledarskap inom marknadsföring) och ordna rapporterna efter mapp i mappen Grupprapporter i Analytics for Global Reports. <br>Arkiveringen bör begränsas till mappen Globala rapporter, eftersom dessa alltid är aktiverade rapporter.   <br>Begränsa arkivering till organisatoriska förändringar som att minska eller lägga till relevanta affärsenheter om du rapporterar baserat på en affärsenhetsstruktur.</td>
  </tr>
  <tr>
    <td>Arbetsyta (om tillämpligt) </td>
    <td>Replikera de globala rapporterna och mappstrukturen mellan arbetsytorna, om du använder arbetsytan, för att få enhetliga rapporter för dina team. Rapporterna finns i mappen Grupprapporter.</td>
  </tr>
  <tr>
    <td>Mina rapporter </td>
    <td>Identifiera och skapa rapporter som behövs för att du ska kunna använda dem i <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mina rapporter</a> -avsnitt. Använd det här privata rapportavsnittet som din sandlåda för globala rapporter. Dessa är bara tillgängliga för den användare som skapar rapporten.   <br>Använd organisationens namnkonvention för att identifiera rapporten och användningen så att du kan stämma av dina rapporter i Mina rapporter med rapporter i Grupprapporter.</td>
  </tr>
  <tr>
    <td>Grupprapporter </td>
    <td>Grupprapporter är din organisations globala rapporter och bör rapportera om den övergripande aktiviteten för din Marketo Engage-organisation.   <br>Överväg att skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank" rel="noopener noreferrer">klanderbara kärnrapporter</a> du förväntar dig att varje affärsenhet ska använda mest för att minska den tid som krävs för att ta fram rapporten och säkerställa att data är korrekta. Se informationen i tabellen"Grundläggande rapportering - Globala rapporter" [INFOGA LÄNK TILL BOOKMARKERAT AVSNITT]. <br>Prestandarapport för människor (heltid och tidsbaserad) - per källa, månad <br>Resultatrapport för program (per kostnadsmånad, tidsbaserad) <br>Resultatrapport för e-post (tidsbaserad) <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank" rel="noopener noreferrer">Aktivera"Global Reporting"</a> på rapportens inställningsflik för att inkludera data från alla dina arbetsytor i e-postprestanda- och e-postlänkens prestandarapporter. Om du har mer än en arbetsyta behöver du bara aktivera den i standardarbetsytan.  <br>TIPS: Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank" rel="noopener noreferrer">Smart List</a> med de filter som du vill ta med i de flesta rapporterna i avsnittet Databas. När du behöver uppdatera villkoren för smart lista kan du uppdatera dem på ett ställe i stället för att uppdatera dem i alla globala rapporter.</td>
  </tr>
</tbody>
</table>

## Prenumerationer {#subscriptions}

<table>
<thead>
  <tr>
    <th>Område </th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumerationer </td>
    <td>Anpassa er till er marknadsledare när det gäller personer som ska granska rapportresultaten och deras frånvaro under implementeringen. <br>Använd prenumerationer för att distribuera data till välbekanta personer i organisationen utan att behöva utnyttja en personlig licens. <br>TIPS: Prenumerationens e-postmeddelanden skickas vanligtvis under natten. Om du vill att användarna ska få tillgång till realtidsrapportdata måste du lägga till personer som användare, så att de direkt kan kontrollera rapporten. <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Ställ in prenumerationer</a> enligt önskad (daglig/veckovis/månadsvis) frånvaro för varje teamets pågående övervakning. Du kan också <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">visa alla prenumerationer</a> på ett och samma ställe under prenumerationsfliken i Analytics.</td>
  </tr>
</tbody>
</table>

## Globala rapporter {#global-reports}

Identifiera rapporter som ska delas med olika användargrupper inom organisationen (t.ex. säljteam, marknadsledare). Skapa en lämplig mappstruktur för varje team/användargrupp/affärsenhet för att ordna rapporterna i grupprapporter när du klonar rapporterna. Överväg att konfigurera globala rapporter som:

<table>
<thead>
  <tr>
    <th style="width:20%">Typ av rapportering</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport om e-postprestanda </td>
    <td>Skapa rapporter för hela arbetsytan/affärsenheten med rätt e-postmeddelanden markerat.  <br>Skapa en lokal rapport om e-postprestanda i alla klonbara programmallar. <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Använd en relevant tidsram</a> (t.ex. År, senaste 180 dagar, senaste 90 dagar) för rapporten så att du får en korrekt bild av standardiserade e-postinteraktions- och leveransvärden. <br>TIPS: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Aktivera filtrering av startaktivitet i Admin&gt;E-post</a> för att undvika loggning eller identifiera om loggning är aktiverat för robotaktiviteterna. <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Inkludera filtret så att bara öppnade/klickade aktiviteter tillåts med begränsningen "Är punktaktivitet" satt till "Falskt"</a> i Smart List of your cloneable Global Reports.</td>
  </tr>
  <tr>
    <td>Prestandarapport för människor</td>
    <td>Obs! Vi rekommenderar att du har en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">strategi för kanaler och taggar</a> för varje implementering av Marketo Engage, innan ni kan spåra de personer ni köpt genom varje, och avkastningen på era marknadsföringsinvesteringar per kanal. <br>Ta reda på vilka kriterier du ska använda för att mäta resultatet i era kundvärvningsprogram och skapa tidsbaserade (innevarande år, senaste rullande 12-månadersvy eller 180-dagarsrapporter) standardrapporter baserade på följande mätvärden: <br>Förvärvningsprogram: Marketo Engage som krediteras för förvärvet av leadet.  <br>Personkälla: Källkategorin för hur posten skulle kännas känd för din databas (baserat på källlistan med värden i CRM) <br>Mät personer som skapats per vecka eller månad. Den här rapporten ger dig ett mått på databasens tillväxthastighet och om du närmar dig eller snart kommer att överskrida storleksgränsen för din databas. <br>Filtrera mätvärden i personprestandarapporter efter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">använda smarta listor som anpassade kolumner.</a>  <br>TIPS: Skapa smarta listor för de anpassade kolumner som du vill lägga till i personprestandarapporten i 'Databas' i stället för 'Marknadsföringsaktiviteter', så att du kan se namnet på den smarta listan korrekt och tydligt när den väljs i rapporten.</td>
  </tr>
  <tr>
    <td>Rapport om programprestanda</td>
    <td>OBS! Den här rapporten kräver att du har definierat dina kanaler, förloppsstatus och steg för slutförande i <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel">Admin &gt; Taggar</a>. <br><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mät effekten av er marknadsföringstaktik</a> inom selektiva program. <br>Hantera programmedlemskap (med hjälp av smarta kampanjer för att uppdatera förvärvsprogram, status, status) enligt bästa praxis inom marknadsföringsaktiviteter.  <br>Åtgärd som bygger på kostnader för innevarande år och rullande 12 månader.  <br>Kom ihåg att behålla <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Periodkostnader</a> är avgörande för att kunna utnyttja programprestandarapporten. <br>TIPS: Så här sammanställer du och visar <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">importerade listor</a> i Prestandarapporter för programmet ser du till att era team väljer rätt inköpsprogram för taggning. Överväg <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">skapa ett standardprogram</a> som ska väljas som förvärvsprogram när de importerade listorna inte gäller någon kanal. Detta garanterar att alla importerade personer har ett giltigt förvärvsprogram som är relaterat till deras källa, affärsenhet, kanal osv. i stället för ett tomt värde.</td>
  </tr>
  <tr>
    <td>Prestandarapport för landningssida</td>
    <td> Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Prestandarapport för landningssida</a> som en global rapport så att ni kan <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrera och granska siffrorna</a> av alla era landningssidor i Design Studio eller landningssidor för marknadsföringsaktiviteter på ett och samma ställe. <br>För program med landningssidor bör du överväga <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">skapa en dedikerad lokal rapport i programmallen</a> så att du kan granska resultatet på programnivå.</td>
  </tr>
  <tr>
    <td>Aktivitetsrapport för webbsida </td>
    <td>OBS! Endast webbsidor (externa och Marketo landningssidor) som har <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a> aktiveras och spåras i den här rapporten. Överväg att placera JavaScript-koden i Tag Management-plattformen, som <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, för att undvika hårdkodning av koden på alla webbsidor.  <br>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Aktivitetsrapport för webbsida</a> som en global rapport så att du kan granska alla dina webbsidor på ett och samma ställe. Observera att dina externa webbsidesaktiviteter endast återspeglas i aktivitetsrapporter för webbsidor. </td>
  </tr>
</tbody>
</table>

## Lokala rapporter {#local-reports}

Vissa Marketo Engage-rapporter är bäst lämpade att användas som lokala resurser inom specifika program i&quot;marknadsföringsaktiviteter&quot;, eftersom de används bäst i en mer begränsad uppsättning program och resurser. Överväg att skapa grundläggande rapporter som:

<table>
<thead>
  <tr>
    <th style="width:20%">Typ av rapportering</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Resultatrapport för e-postlänk</td>
    <td>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank" rel="noopener noreferrer">Resultatrapport för e-postlänk</a> inom program som skickar e-post och era droppkampanjer för att ge er insikter om de länkar som andra klickar på i era e-postmeddelanden.</td>
  </tr>
  <tr>
    <td>Kampanjaktivitetsrapport</td>
    <td>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank" rel="noopener noreferrer">Kampanjaktivitetsrapport</a> och välja en period i din arbetsmapp i Marknadsföringsaktiviteter. <br>Ställ in rapporter för att övervaka utlösarna för varje användningsfall och <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank" rel="noopener noreferrer">använda kampanjfilter</a>till exempel utlösare för beteendebedömning, utlösare för livscykelkvalificering, utlösare för intressanta ögonblick.</td>
  </tr>
  <tr>
    <td>Resultatrapport för engagemangsström (om tillämpligt)</td>
    <td>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank" rel="noopener noreferrer">Resultatrapport för engagemangsström</a> för att mäta effektiviteten hos innehåll och strömmar som driftsätts inom ert engagemangsprogram. <br>Överväg <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank" rel="noopener noreferrer">använda segmenteringsfiltret på rapportens inställningsflik</a> och gruppera rapportdata efter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank" rel="noopener noreferrer">segment</a> (t.ex. personkälla, bransch) som används i ditt Engagement Program. Detta hjälper er att få djupare insikter i varje segments engagemangsmönster och vägleder er att göra strategiska ändringar för att förbättra ert engagemangsprogram (innehåll, ström, strömavslut osv.).</td>
  </tr>
</tbody>
</table>
