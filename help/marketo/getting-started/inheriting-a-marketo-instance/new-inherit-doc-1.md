---
description: Inherit Doc 1 - Marketo Docs - produktdokumentation
title: Ärv dok 1
hide: true
hidefromtoc: true
source-git-commit: 0f34b8ac4283e78027c81bf654d090c5ee78b9ee
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 2%

---

# Ärv dok 1 {#inherit-doc-1}

Granskning av en ärvd instans kan se ut som en..

Har du ärvt en befintlig Marketo Engage-instans från en annan administratör? I så fall är den här artikeln till dig ...

Checklistan nedan har lagts ihop med indata från Marketo Champions så att du snabbt kommer igång i den ärvda instansen..

>[!TIP]
>
>Om du är nybörjare i Marketo Engage och inte känner till många av villkoren kan du läsa [Marketo-ordlista](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Användare och roller {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td><li>Hur många användare finns det?</li>
<li>Finns det några användare som borde ha gått ut?</li>
<li>Har ditt företag policyer för att ta bort användare?</li> 
<li>Hur många användare har administratörsbehörighet?</li>
<li>Ska någon av dessa användare ändras till andra roller?</li> 
<li>Vilka är API-användarna i den här instansen?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Roller</td> 
   <td><li>Hur många roller finns det?</li>  
<li>Vilka behörigheter/behörigheter har varje roll? Ska någon justeras?</li>
<li>Hur många användare finns det per roll?</li>
<li>Hur ofta loggar användare in?</li>
<li>Har varje API-användare en egen användarroll? Om inte, bör du implementera den för att underlätta felsökningen.</li> 
<li>Anpassar era användarroller och behörigheter till era integritetspolicyer för företagsdata?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Intern dokumentation</td> 
   <td><li>Är användare och roller tydligt definierade i din organisation?</li>
<li>Hur lägger du till en ny användare/administratör?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Sandlåda (om tillämpligt)</td> 
   <td><li>Har du en sandlådeinstans? I så fall kan du granska kategorierna ovan för din sandlåda.</li>
<li>Är programimport länkad till din sandlåda?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Granskningsspår {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Granskningsspår</td> 
   <td><li>Vem arbetar i instansen?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Arbetsytor och partitioner {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Arbetsytor och partitioner</td> 
   <td><li>Hur många arbetsytor och/eller partitioner har du?</li>
<li>Vad är det primära syftet med varje arbetsyta och partition?</li>
<li>Måste de granskas eller ändras?</li>
<li>Vilken är relationen mellan arbetsytorna och partitionerna?</li>
<li>Hur många användare har tillgång till varje arbetsyta?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Intern dokumentation</td> 
   <td><li>Hur definieras arbetsytor och partitioner?</li>
<li>Hur lägger du till arbetsytor i instansen eller lägger till användare på en arbetsyta?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Smarta kampanjer {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Inställningar för smart kampanj</td> 
   <td><li>Har du en begränsning för storleken på Smart Campaign?</li>
<li>Om inte, överväg att lägga till en. Vi rekommenderar att gränsen för smarta kampanjer begränsas till 25 % av databasen för att undvika överkommunikation eller att hela databasen behandlas i arbetsflöden. Detta skyddar inte bara varumärket utan hjälper till att skydda instansens prestanda.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbegränsningar</td> 
   <td><li>Finns det begränsningar? Har ert företag policyer där kommunikationsbegränsningar kan behövas?</li>
<li>Adobe rekommenderar att du begränsar din kommunikation till 1 per dag och 3 per 7 dagar, med e-post som inte fungerar blockerad.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Taggar {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Taggar</td> 
   <td><li>Hur många taggar finns det? Hur många taggar används? Behöver du lägga till något?</li>
<li>Krävs det taggar i programmen?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Kanaler</td> 
   <td><li>Hur många kanaler finns det? Hur många används?</li>
<li>Är alla kanalprogramstatusar lämpliga? Visas framsteg inom programmet?</li>
<li>Är era kanaler relaterade till specifika programtyper?</li>
<li>Vilka statusvärden anses vara framgångsrika för varje kanal? Anpassar de era marknadsföringsmål?</li>
<li>Används den operativa kanalen korrekt?</li>
<li>För Advanced Report Builder (Revenue Cycle Explorer\RCE), är kanalanalysfunktionen inställd på att anpassa sig till era programrutiner med periodkostnader?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marknadsföringskalender (om tillämpligt)</td> 
   <td><li>Hur många kalenderposttyper finns det? Är de fortfarande relevanta?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Databashantering {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Fälthantering</td> 
   <td><li>Hur många fält finns det? Klicka på Exportera fältnamn om du vill visa en lista över fält, anpassade fält och deras API-namn.</li>
<li>Hur många anpassade fält finns det?</li>
<li>Hur många fält används? Välj Exportera som används av i listrutan Fältåtgärder om du vill granska relaterade resurser i ett fält.</li>
<li>Hur många synkroniseras mellan Marketo Engage och CRM?</li>
<li>Synkroniseras CRM-fält med rätt objekt?</li>
<li>Finns det en anpassad vyuppsättning för persondetaljer? Borde det vara?</li>
<li>Har du en namngivningsregel för dina fält baserat på källa? Om inte, överväg att genomföra detta.</li>
<li>Finns det några fält blockerade? Se till att förstå varför de är det.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Anpassade aktiviteter</td> 
   <td><li>Finns det några anpassade aktiviteter?</li>
<li>Klicka i så fall igenom dem för att förstå vilka aktiviteter som inte är relaterade till ett Marketo-formulär, e-postmeddelande eller en landningssida.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Anpassade objekt</td> 
   <td><li>Hur många anpassade objekt finns det? Hur synkroniseras de med din CRM?</li>
<li>Hur används dessa anpassade objekt av program och listfrågor?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integreringar {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Vilken CRM synkroniserar du med? Salesforce? MS Dynamics? Veeva?</li>
<li>Är den anpassade synkroniseringen eller dubbelriktad? (KG: KORRIGERA GRAMMAR OCH KONTROLLERA VIKTIGHET)</li>
<li>[Endast Salesforce] Har din instans anpassade synkroniseringsfilter implementerats? Kontakta Marketo Support för att identifiera anpassade synkroniseringsfilter eller begära att en anpassad synkroniseringsregel implementeras.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Landningssidor</td> 
   <td><li>Vad är domänen angiven som?</li>
<li>Vad är reservinställningen som?</li>
<li>Vad är hemsidan som?</li>
<li>Är förifyllning av formulär aktiverat?</li>
<li>Är personaliserade URL-adresser aktiverade?</li>
<li>Finns det regler för omdirigeringar?</li>
<li>Har du befintliga domänalias? Följer du igenom dokumentation om hur du använder domänalias?</li>
<li>Är säkra domäner för landningssidor aktiverade? Bekräfta om dina resurser på landningssidan innehåller en http-URL.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Finns din Munchkin-spårningskod på din webbplats (inte i Marketo)?</li>
<li>Är en Do Not Track-webbläsarbegäran aktiverad?</li>
<li>Är ditt Munchkin API konfigurerat? Om du saknar dokumentation om var munkinkoden finns på webbplatsen kan du snabbt komma igång med att använda Web Analytics-rapporten i grundläggande Analytics för att förstå var Munchkin-koden placeras på webbplatsen.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Webbtjänster</td> 
   <td><li>Är IP-begränsningar aktiverade? Borde de vara det?</li>
<li>Vilka användare/appar gör API-anrop i din instans?</li>
<li>Stöter du eller är du nära att stöta på API-gränsen? Om så är fallet bör du överväga att öka den eller granska instansen för att få ned API-anropen.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (om tillämpligt)</td> 
   <td><li>Har <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-paketet har installerats</a>?</li>
<li>Har du <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">uppgraderat till den senaste versionen av Sales Insight</a>?</li>
<li>Har du slutfört konfigurationen av Sales Insight? Företag/obegränsade användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">klicka här</a>, Professional-användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">klicka här</a>.</li>
<li>Har du <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ger åtkomst till dina användare</a> baserat på hur många licenser du har köpt?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Treasure Chest {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Treasure Chest</td> 
   <td><li>Vad är aktiverat i skattekameran?</li>
<li>Finns det funktioner som ska aktiveras eller inaktiveras?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Campaign Inspector</td> 
   <td><li>Är Campaign Inspector aktiverad?</li>
<li>Om inte kan du aktivera det för att enkelt identifiera vilka kampanjer som är aktiva, synkronisera med CRM och/eller ta bort poster.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Diverse {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Område</th> 
   <th>Granska fokus</th>
   <th>Kolumn 3</th>
  </tr> 
  <tr> 
   <td>Marketo Engage statusuppdateringar</td> 
   <td><li>Är din instans registrerad för statusuppdateringar för Marketo Engage?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Auktoriserade kontakter</td> 
   <td><li>Har du konfigurerat lämpliga behöriga kontakter i supportportalen?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Varningar</td> 
   <td><li>Finns det några aktiva varningar som skickas ut till interna team från Marketo Engage?</li>
<li>Om ja, fungerar dessa aviseringar på rätt sätt?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Meddelanden</td> 
   <td><li>Prenumererar du på lämpliga administratörsmeddelanden?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
