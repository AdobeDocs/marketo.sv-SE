---
description: Inherit Doc 1 - Marketo Docs - produktdokumentation
title: Ärv dok 1
hide: true
hidefromtoc: true
source-git-commit: 8d9ea20f04ec6320b31c2d6000240b72a45be959
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%

---

# Ärv dok 1 {#inherit-doc-1}

Checklistorna nedan (efterföljande checklistor länkade till längst ned i varje artikel) har sammanställts med indata från Marketo Champions för att du snabbt ska komma igång. Du kan även hämta checklistorna och följa upp dina framsteg.

>[!TIP]
>
>Om du är nybörjare i Marketo Engage och inte känner till många av villkoren kan du läsa [Marketo-ordlista](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Adobe Admin Console {#adobe-admin-console}

<table> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th> 
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Prenumeration</td> 
   <td><li>Är din prenumeration på Marketo Engage på <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe Identity Management System</a> (Adobe IMS) ännu? 
<br/>
Om så är fallet, har du fått rollen "Adobe Admin Console Product Admin" av din "Adobe Admin Console System Admin"? Om du är osäker på vem i organisationen som har administratörsbehörighet i konsolen kontaktar du <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe kundtjänst</a>.  
<br/>Annars fortsätter du med <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">äldre användarroller och behörigheter</a> i Marketo Engage &gt; Admin &gt; Användare och roller tills din prenumeration förnyas.</li></td>
  </tr>
  <tr> 
   <td>Produktprofil</td> 
   <td>(Prenumerationer på Adobe IMS <b>endast</b>)
<p>
<li>Har du tilldelats rollen 'produktadministratör för Marketo Engage' i Marketo Engage/Admin/Users &amp; Roles?</li> 
<li>Har du tilldelat Marketo Engage till alla lämpliga användares produktprofiler i Adobe Admin Console?
<br/>Om inte, måste du tilldela Marketo Engage till deras Adobe IMS-produktprofil innan du tilldelar deras roller i Marketo Engage/Admin/Users &amp; Roles.</li>
<p>Obs! Om din prenumeration har fler än 75 användare och nyligen har migrerats till Adobe IMS kan du välja att migrera flera användare och administrera deras Adobe-ID i grupper eller alla samtidigt. Läs mer om vad du kan förvänta dig av <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md#prepare-users-for-migration-day" target="_blank">Migreringsdag för Adobe IMS</a>.</td>
  </tr>
  <tr> 
   <td>API för användarhantering</td> 
   <td><li>Har din prenumeration använt några Marketo API:er för användarhantering?
<br/>I så fall måste du använda <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API:er</a> om du vill bjuda in, uppdatera och ta bort användare framåt.</li></td>
  </tr>
 </tbody> 
</table>

## Användare och roller {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Hur många användare</a> Är det där?</li>
<li>Finns det några användare som borde ha gått ut?</li>
<li>Har ditt företag policyer för att ta bort användare?</li> 
<li>Hur många användare har <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Administratörsbehörigheter</a>?</li>
<li>Bör någon av dessa användare ändras till <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">andra roller?</a></li> 
<li>Vilka är API-användarna i den här instansen?</li></td>
  </tr>
  <tr> 
   <td>Roller</td> 
   <td><li>Hur många roller finns det?</li>  
<li>Vad <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">behörigheter/åtkomst</a> har varje roll? Ska någon justeras?</li>
<li>Hur många användare finns det per roll?</li>
<li>Hur ofta är användare <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">logga in</a>?</li>
<li>Har varje API-användare sina <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">egen användarroll</a>? Om inte, bör du implementera den för att underlätta felsökningen.</li> 
<li>Anpassa era användarroller och behörigheter efter era företagsdata <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">integritetspolicy</a>?</li></td>
  </tr>
  <tr> 
   <td>Supportanvändare</td> 
   <td><li>Har du ställt in rätt <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">auktoriserade kontakter</a> i supportportalen?</li></td>
  </tr>
  <tr> 
   <td>Intern dokumentation</td> 
   <td><li>Är användare och roller tydligt definierade i din organisation?</li>
<li>Hur lägger du till en ny användare/administratör?</li></td>
  </tr>
  <tr> 
   <td>Sandlåda (om tillämpligt)</td> 
   <td><li>Har du en <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox-instans</a>?
   <br/>  I så fall kan du granska kategorierna ovan för din sandlåda.</li>
<li>Är <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Programimport</a> länkad till din sandlåda?</li></td>
  </tr>
 </tbody> 
</table>

## Granskningsspår {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Granskningsspår</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Vem arbetar?</a> i instansen?</li></td>
  </tr>
 </tbody> 
</table>

## Arbetsytor och partitioner {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Arbetsytor och partitioner</td> 
   <td><li>Hur många <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Arbetsytor och/eller partitioner</a> Har du?</li>
<li>Vad är det primära syftet med varje arbetsyta och partition?</li>
<li>Gör något av dina <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Arbetsytor</a> eller <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partitioner</a> Måste granskas/ändras?</li>
<li>Vilken är relationen mellan arbetsytor och partitioner?</li>
<li>Hur många användare <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">har åtkomst</a> till varje arbetsyta?</li></td>
  </tr>
  <tr> 
   <td>Intern dokumentation</td> 
   <td><li>Hur definieras arbetsytor och partitioner?</li>
<li>Hur lägger du till arbetsytor i instansen eller lägger till användare i en arbetsyta?</li></td>
  </tr>
 </tbody> 
</table>

## Smarta kampanjer {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Inställningar för smart kampanj</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Har du en begränsning?</a> på Smart Campaign-storleken? 
   <br/>Om inte, överväg att lägga till en. Vi rekommenderar att du begränsar Smart Campaign-gränsen till 25 % av databasen för att undvika överkommunikation eller att hela databasen behandlas i arbetsflöden. Detta skyddar inte bara varumärket, utan hjälper till att skydda instansens prestanda.</li></td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbegränsningar</td> 
   <td><li>Finns det <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">kommunikationsgränser</a> på plats? Har ert företag policyer där kommunikationsbegränsningar kan behövas?</li>
<p>Obs! Vi rekommenderar att du begränsar din kommunikation till 1 per dag och 3 per 7 dagar med <b>ej</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operativ</a> e-post blockerad.</td>
  </tr>
 </tbody> 
</table>

## Taggar {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Taggar</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-new-program-tag-and-tag-values.md" target="_blank">Hur många taggar</a> Är det där? Hur många taggar används? Behöver du lägga till något?</li>
<li>Krävs det taggar i programmen?</li></td>
  </tr>
  <tr> 
   <td>Kanaler</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Hur många kanaler</a> Är det där? Hur många används?</li>
<li>Är alla <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">status för kanalprogram lämplig</a>? Visas framsteg inom programmet?</li>
<li>Är era kanaler relaterade till specifika programtyper?</li>
<li>Vilka statusvärden anses vara framgångsrika för varje kanal? Anpassar de era marknadsföringsmål?</li>
<li>Används den operativa kanalen korrekt?</li>
<li>För Advanced Report Builder (Revenue Cycle Explorer/RCE), är kanalanalysbeteendet anpassat till era programrutiner med periodkostnader?</li></td>
  </tr>
  <tr> 
   <td>Marknadsföringskalender (om tillämpligt)</td> 
   <td><li>Hur många <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">kalenderposttyper</a> Är det där? Är de fortfarande relevanta?</li></td>
  </tr>
 </tbody> 
</table>

## Databashantering {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Fälthantering</td> 
   <td><li>Hur många fält finns det? 
   <br/>Klicka <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exportera fältnamn</a> om du vill granska en lista med fält, anpassade fält och deras API-namn.</li>
<li>Hur många <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">anpassade fält</a> Är det där?</li>
<li>Hur många fält används? 
<br/>Välj <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exportera som används av</a> i listrutan Fältåtgärder för att granska relaterade resurser i ett fält.</li>
<li>Hur många fält synkroniseras mellan Marketo Engage och CRM?</li>
<li>Synkroniseras CRM-fält med rätt objekt?</li>
<li>Finns det en <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">anpassad vyuppsättning</a> för persondetaljer? Borde det vara?</li>
<li>Har du en namngivningsregel för dina fält baserat på källa? 
<br/>Om inte, överväg att genomföra detta.</li>
<li>Finns det några fält <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">blockerad</a>? 
<br/>I så fall, se till att förstå varför de är det.</li></td>
  </tr>
  <tr> 
   <td>Anpassade aktiviteter</td> 
   <td><li>Finns det några <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">anpassade aktiviteter</a>?
<br/>Klicka i så fall igenom dem för att förstå vilka aktiviteter som inte är relaterade till ett Marketo-formulär, e-postmeddelande eller en landningssida.</li></td>
  </tr>
  <tr> 
   <td>Anpassade objekt</td> 
   <td><li>Hur många <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">anpassade objekt</a> Är det där? Hur synkroniseras de med din CRM?</li>
<li>Hur används dessa anpassade objekt av program och listfrågor?</li></td>
  </tr>
 </tbody> 
</table>

## Integreringar {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Vilken CRM synkroniserar du med? Salesforce? MS Dynamics? Veeva?</li>
<li>Använder du en <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">anpassad synkronisering</a>?</li>
<li>[Endast Salesforce] Har din instans anpassade synkroniseringsfilter implementerats? 
<p>Obs! Kontakta Marketo Support om du vill identifiera anpassade synkroniseringsfilter eller begära att en anpassad synkroniseringsregel implementeras.</li></td>
  </tr>
  <tr> 
   <td>Landningssidor</td> 
   <td><li>Vad är <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">domänuppsättning som</a>?</li>
   <li>Vad är hemsidan som?</li>
<li>Vad är <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">återfallsuppsättning som</a>?</li>
<li>Är förifyllning av formulär aktiverat?</li>
<li>är <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">personaliserade URL:er</a> aktiverad?</li>
<li>Finns det regler för <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">omdirigeringar</a>?</li>
<li>Har du befintliga domänalias? Följer du hur du använder domänalias?</li>
<li>Är <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Skyddade domäner för landningssidor</a> aktiverad? 
<br/>Bekräfta om dina resurser på landningssidan innehåller en http-URL.</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Är din <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin-spårningskod</a> på din webbplats (inte i Marketo)?</li>
<li>Är en <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Spåra inte</a> Webbläsarbegäran aktiverad?</li>
<li>Är din <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">Munchkin API</a> konfigurerad? 
<p>Tips! Om du saknar dokumentation om var munkinkoden finns på webbplatsen kan du visa alla URL:er genom att skapa en <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Aktivitetsrapport för webbsida</a>.</li></td>
  </tr>
  <tr> 
   <td>Webbtjänster</td> 
   <td><li>är <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP-begränsningar</a> aktiverad? Borde de vara det?</li>
<li>Vilka användare/appar gör API-anrop i din instans?</li>
<li>Stöter du eller är du nära att stöta på API-gränsen? 
<br/>Om så är fallet bör du överväga att öka den eller granska instansen för att få ned API-anropen.</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (om tillämpligt)</td> 
   <td><li>Har <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-paketet har installerats</a>?</li>
<li>Har du <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">uppgraderat till den senaste versionen av Sales Insight</a>?</li>
<li>Har du slutfört konfigurationen av Sales Insight? <br/>Företag/obegränsade användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">klicka här</a>, Professional-användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">klicka här</a>.</li>
<li>Har du <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">ger åtkomst till dina användare</a> baserat på hur många licenser du har köpt?</li>
<li>är <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Stjärnor och flamman</a> skräddarsydd?</li></td>
  </tr>
  <tr> 
   <td>Startpunkt (om tillämpligt)</td> 
   <td><li>Vilka tjänster har du konfigurerat (till exempel <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zooma</a>, osv.)? Har de snart gått ut?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Hur många API-anrop</a> Använder era integreringar?</li>
<li>Har ni rätt integreringar för era användningsfall?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (om tillämpligt)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Vilka anslutningar</a> Har du ställt upp?</li>
<li>Används inte längre?</li></td>
  </tr>
  <tr> 
   <td>Mobilappar (om tillämpligt)</td> 
   <td><li>som <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">mobilappar</a> Har du?</li>
<li>Har <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">testenheter</a>  har lagts till?</li></td>
  </tr>
 </tbody> 
</table>

## Treasure Chest {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Treasure Chest</td> 
   <td><li>Det som är aktiverat i <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Treasure Chest</a>?</li>
<li>Finns det funktioner som ska aktiveras eller inaktiveras?</li></td>
  </tr>
  <tr> 
   <td>Campaign Inspector</td> 
   <td><li>Är <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Campaign Inspector</a> aktiverad?
<br/>Om inte kan du aktivera det för att enkelt identifiera vilka kampanjer som är aktiva, synkronisera med CRM och/eller ta bort poster.</li></td>
  </tr>
 </tbody> 
</table>

## Varningar och uppdateringar {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Marketo Engage statusuppdateringar</td> 
   <td><li>Prenumererar din instans på <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage statusuppdateringar</a>?</li></td>
  </tr>
  <tr> 
   <td>Varningar</td> 
   <td><li>Finns det några <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">aktiva aviseringar</a> skickas ut till interna team från Marketo Engage?</li>
<li>Om ja, fungerar dessa aviseringar på rätt sätt?</li></td>
  </tr>
  <tr> 
   <td>Meddelanden</td> 
   <td><li>Prenumererar du på lämplig administratör? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">meddelanden</a>?</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[Granska en ärvd instans: Database ►](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-2.md)
