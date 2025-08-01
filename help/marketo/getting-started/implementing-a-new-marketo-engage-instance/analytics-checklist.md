---
description: Ställ in Analytics-avsnittet för din nya Marketo Engage-instans.
title: New Instance Best Practices - Analytics Checklist
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Ny instansmetodpraxis: Analyschecklista {#new-instance-best-practices-analytics-checklist}

I avsnittet Analytics (Analyser) finns globala rapporter som analyserar resultatet av era marknadsföringssatsningar. Lär dig hur du navigerar i dem.

Kom ihåg att [hämta checklistorna](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) och spåra dina framsteg.

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
    <td>Organisation: Namngivning, mappar och arkivering</td>
    <td><li>Använd en namngivningskonvention för rapporter för att skilja på rapporter på fliken Globala rapporter.
    <ul><li>Ett exempel på god praxis för namngivning är [rapporttyp] [Global vs. BU-specifik tagg] [Rapportbeskrivning], till exempel [E-postprestanda]-[Global]-[180 dagars e-poståtagande].</li></ul><br>
    <li>Identifiera rapporter som ska delas med olika användargrupper inom organisationen (t.ex. säljteam, ledarskap inom marknadsföring) och ordna rapporterna efter mapp i mappen Grupprapporter i Analytics for Global Reports.</li>
    <li>Arkiveringen bör begränsas till mappen Globala rapporter, eftersom dessa alltid är aktiverade rapporter.   <ul><li>Begränsa arkivering till organisatoriska förändringar som att minska eller lägga till relevanta affärsenheter om du rapporterar baserat på en affärsenhetsstruktur.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Arbetsytor (om tillämpligt)</td>
    <td><li>Replikera de globala rapporterna och mappstrukturen mellan arbetsytorna för att få enhetliga rapporter för era team. Rapporterna finns i mappen Grupprapporter.</li></td>
  </tr>
  <tr>
    <td>Mina rapporter</td>
    <td><li>Identifiera och skapa de rapporter som behövs för att använda dem i avsnittet <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mina rapporter</a>. Använd det här privata rapportavsnittet som din sandlåda för globala rapporter. De är bara tillgängliga för den användare som skapar rapporten.</li>
    <li>Använd organisationens namnkonvention för att identifiera rapporten och användningen så att du kan stämma av rapporter i Mina rapporter med rapporter i Grupprapporter.</li></td>
  </tr>
  <tr>
    <td>Grupprapporter</td>
    <td><li>Grupprapporter är din organisations globala rapporter och bör rapportera om den övergripande aktiviteten för din organisation.</li>
    <li>Överväg att skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">klonbara kärnrapporter</a> som du förväntar dig att varje affärsenhet använder oftast för att minska den tid som krävs för att hämta rapporten och säkerställa att data är korrekta. Mer information finns i tabellen <a href="#global-reports">Globala rapporter nedan</a>.
    <ul><li>Prestandarapport för människor (heltid och tidsbaserad) per källa, månad</li>
    <li>Resultatrapport för program (per kostnadsmånad, tidsbaserad)</li>
    <li>Resultatrapport för e-post (tidsbaserad)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Aktivera Global rapportering</a> på rapportens konfigurationsflik om du vill inkludera data från alla dina arbetsytor i rapporten E-postprestanda och prestanda för e-postlänkar. Om du har mer än en arbetsyta behöver du bara aktivera den i standardarbetsytan.</li>
    <p><img src="assets/tip-icon.png" alt="anteckningsikon"> TIPS: Skapa den <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">smarta listan</a> med de filter som du vill ta med i de flesta rapporter i databasavsnittet. När du behöver uppdatera villkoren för smart lista kan du uppdatera dem på ett ställe i stället för att uppdatera dem i alla globala rapporter.</td>
  </tr>
</tbody>
</table>

## Prenumerationer {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumerationer</td>
    <td><li>Anpassa er till er marknadsledare när det gäller personer som ska granska rapportresultaten och deras frånvaro under implementeringen.</li> <li>Använd prenumerationer för att distribuera data till välbekanta personer i organisationen utan att behöva utnyttja en personlig licens.</li>
    <p><img src="assets/tip-icon.png" alt="anteckningsikon"> TIPS: Om du vill att användarna ska få tillgång till realtidsrapportdata måste du lägga till dem som användare så att de kan visa rapporten.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Ställ in prenumerationer</a> i önskad stängsel (varje dag/vecka/månad) för varje teams pågående övervakning. Du kan även <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">visa alla dina prenumerationer</a> på ett ställe på fliken Prenumerationer i Analytics.</li></td>
  </tr>
</tbody>
</table>

## Globala rapporter {#global-reports}

Identifiera rapporter som ska delas med olika användargrupper inom organisationen (t.ex. säljteam, marknadsledare). Skapa en lämplig mappstruktur för varje team/användargrupp/affärsenhet för att organisera klonade rapporter i grupprapporter. Överväg att konfigurera globala rapporter, som:

<table>
<thead>
  <tr>
    <th style="width:20%">Typ av rapportering</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport om e-postprestanda</td>
    <td><li>Skapa rapporter för hela Workspace/affärsenheten med rätt e-postadress markerad.</li>
    <li>Skapa en lokal e-postprestandarapport i alla klonbara programmallar.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Använd en relevant tidsram</a> (t.ex. YTD, de senaste 90 dagarna osv.) för rapporten för att få en korrekt bild av standarduppgifter för e-postinteraktion och leverans.</li>
    <p><img src="assets/tip-icon.png" alt="anteckningsikon"> TIPS: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Aktivera filtrering av startaktivitet i <strong>Admin &gt; E-post</strong></a> om du vill undvika loggning eller identifiera om loggning har aktiverats för båda aktiviteter. Inkludera filtret så att endast <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Öppnade/klickade aktiviteter tillåts med begränsningen "Är punktaktivitet" inställd på "Falskt"</a> i den smarta listan över dina klonbara globala rapporter.</td>
  </tr>
  <tr>
    <td>Prestandarapport för människor</td>
    <td><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Vi rekommenderar att du har en korrekt <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">kanal- och taggstrategi</a> för varje Marketo Engage-implementering innan du kan spåra de personer som förvärvats och avkastningen på dina marknadsföringsinvesteringar per kanal.
    <p>
    <li>Ta reda på vilka kriterier du ska använda för att mäta resultatet i era kundvärvningsprogram och skapa tidsbaserade (innevarande år, senaste rullande 12-månadersvy eller 180-dagarsrapporter) standardrapporter baserade på följande mätvärden: <ul><li>Förvärvningsprogram: Marketo Engage-program som har krediterats för att förvärva personen.</li>
    <li>Person Source: Källkategorin för hur posten blev känd för din databas (baserat på källlistan med värden i CRM)
    </li></ul>
    <li>Mät personer som skapats per vecka eller månad. Den här rapporten ger dig ett mått på databasens tillväxthastighet och om du närmar dig storleksgränsen för databasen.</li>
    <li>Filtrera måtten i personprestandarapporter efter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">med dina smarta listor som anpassade kolumner.</a></li>
    <p><img src="assets/tip-icon.png" alt="anteckningsikon"> TIPS: Skapa smarta listor för de anpassade kolumner som du vill lägga till i personprestandarapporten i databasen i stället för marknadsföringsaktiviteter så att du kan se namnet på den smarta listan korrekt och tydligt när den väljs i rapporten.</td>
  </tr>
  <tr>
    <td>Rapport om programprestanda</td>
    <td><p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Den här rapporten kräver att du har definierat dina kanaler, förloppsstatus och slutförandesteg i <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Admin</strong> &gt; <strong>Taggar</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mät effekten av er marknadsföringstaktik</a> inom selektiva program.</li>
    <li>Hantera programmedlemskap (med hjälp av smarta kampanjer för att uppdatera förvärvsprogram, status, status) enligt bästa praxis inom marknadsföringsaktiviteter.</li>
    <li>Åtgärd som bygger på kostnader för innevarande år och rullande 12 månader.
    <ul><li>Kom ihåg att det är viktigt att behålla <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">periodkostnader</a> för att du ska kunna utnyttja programprestandarapporten.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="anteckningsikon"> TIPS: Om du vill samla och visa alla <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">importerade listor</a> i Prestandarapporter för program måste dina team välja rätt förvärvsprogram för taggning. Överväg att <a href="https://experienceleague.adobe.com/sv/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">skapa ett standardprogram</a> som ska väljas som förvärvsprogram när de importerade listorna inte gäller någon kanal. Detta garanterar att alla importerade personer har ett giltigt förvärvsprogram som är relaterat till källa, affärsenhet, kanal osv. i stället för ett tomt värde.</td>
  </tr>
  <tr>
    <td>Prestandarapport för landningssida</td>
    <td><li>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">landningssidans resultatrapport</a> som en global rapport så att du kan <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrera och granska </a> av alla era landningssidor för Design Studio/Marketing Activities på ett och samma ställe.</li>
    <li>För program med landningssidor bör du överväga att <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">skapa en dedikerad lokal rapport i programmallen</a> så att du kan granska prestandan på programnivå.</li></td>
  </tr>
  <tr>
    <td>Aktivitetsrapport för webbsida</td>
    <td><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Endast webbsidor (externa och Marketo Landing Pages) som har <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a> aktiverat spåras i den här rapporten. Överväg att placera JavaScript-koden i Tag Management-plattformen, till exempel <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, för att undvika att hårdkoda koden på alla webbsidor.
    <p>
    <li>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">webbsidesaktivitetsrapporten</a> som en global rapport så att du kan granska alla dina webbsidor på ett och samma ställe. Observera att dina externa webbsidesaktiviteter endast återspeglas i aktivitetsrapporter för webbsidor.</li></td>
  </tr>
</tbody>
</table>

## Lokala rapporter {#local-reports}

Vissa Marketo Engage-rapporter distribueras bäst som lokala resurser inom specifika program i marknadsföringsaktiviteter, eftersom de vanligtvis används i en mer begränsad uppsättning program och resurser. Överväg att skapa grundläggande rapporter, till exempel:

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
    <td><li>Skapa en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">prestandarapport för e-postlänk</a> i program som skickar e-postmeddelanden och dina droppkampanjer för att ge dig insikter om de länkar som andra klickar på i e-postmeddelanden.</li></td>
  </tr>
  <tr>
    <td>Kampanjaktivitetsrapport</td>
    <td><li>Skapa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">kampanjaktivitetsrapporten</a> och välj en period i din arbetsmapp i marknadsföringsaktiviteter.</li>
    <li>Ställ in rapporter för att övervaka utlösarna för varje användningsfall och <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">tillämpa kampanjfilter</a> (t.ex. utlösare för beteendebedömning, utlösare för livscykelkvalificering, utlösare för intressanta ögonblick).</li></td>
  </tr>
  <tr>
    <td>Resultatrapport för engagemangsström (om tillämpligt)</td>
    <td><li>Skapa en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">resultatrapport för engagemangsströmmen</a> för att mäta effektiviteten hos innehåll och strömmar som distribuerats inom ditt engagemangsprogram.</li>
    <li>Använd filtret <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">"Segmentering" på rapportens fliken Inställningar </a> och gruppera rapportdata efter det <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segment</a> (t.ex. personkälla, bransch) som används i ditt Engagement Program. Detta hjälper er att få djupare insikter i varje segments engagemangsmönster och vägleder er att göra strategiska ändringar för att förbättra ert engagemangsprogram (innehåll, ström, strömavslut osv.).</li></td>
  </tr>
</tbody>
</table>
