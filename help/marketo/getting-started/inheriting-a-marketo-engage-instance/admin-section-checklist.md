---
description: Ärvd kontrollista för instansadministratör - Marketo Docs - Produktdokumentation
title: Ärvd kontrollista för instansadministratör
feature: Getting Started
exl-id: 4840d1a8-306b-4b53-917d-2262ae903a42
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '1592'
ht-degree: 0%

---

# Ärvd instans: Admin Section Checklist {#inherited-instance-admin-section-checklist}

Checklistorna nedan (efterföljande checklistor länkade till längst ned i varje artikel) har sammanställts av Adobe Professional Services med synpunkter från Marketo Champions för att du snabbt ska komma igång. Du kan också [ladda ned checklistor](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) och spåra dina framsteg.

>[!TIP]
>
>Om du är nybörjare i Marketo Engage och inte känner till många av villkoren kan du läsa [Marketo Engage - ordlista](/help/marketo/getting-started/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Detta gäller endast prenumerationer på [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. If your Marketo Engage subscription has not onboarded Adobe IMS yet, proceed with the [legacy user roles and permissions experience](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} i Marketo Engage > Admin > Användare &amp; roller.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th> 
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Prenumeration och produktadministratör för Marketo Engage</td> 
   <td><li>Har din Marketo Engage-prenumeration migrerats till <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> ännu? 
<br/>     Om så är fallet, har du fått rollen "Adobe Admin Console Product Admin" av din "Adobe Admin Console System Admin"? Om du är osäker på vem i organisationen som har administratörsbehörighet i konsolen kontaktar du <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe kundtjänst</a>.</li>
<li>Har du accepterat inbjudan till produktadministratör för Marketo Engage? E-postmeddelandet skickas när rollen tilldelas i Adobe Admin Console.
<br/>     Om inte, sök efter <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">välkomstmeddelande</a> i din inkorg och acceptera inbjudan att aktivera din Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Produktprofil</td> 
   <td><li>Tilldelas alla lämpliga användare till Marketo Engage produktprofil i Adobe Admin Console?
<br/>     Om inte, se till att <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">lägga till och/eller ta bort användare</a> från Marketo Engage produktprofiler i Adobe Admin Console. Du kan inte tilldela användarroller i Marketo Engage &gt; Admin &gt; Användare och roller om de läggs till i en produktprofil.</li>
<p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Marketo Engage.</td>
  </tr>
  <tr> 
   <td>API för användarhantering</td> 
   <td><li>Använder din prenumeration några Marketo API:er för användarhantering?
<br/>     I så fall måste du använda <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API:er</a> om du vill bjuda in, uppdatera och ta bort användare framåt.</li>
<p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Rollhantering finns kvar i Marketo Engage och Marketo API:er för användarhantering kan fortfarande användas för rollhantering.</td>
  </tr>
 </tbody> 
</table>

## Användare och roller {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Om din prenumeration redan finns på Adobe IMS går du vidare till följande granskning av användarhantering i Adobe Admin Console. I annat fall går du till Admin &gt; Användare och roller &gt; Användare i Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Hur många användare</a> Är det där?</li>
<li>Finns det några användare som ska <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">borttagen</a>?</li>
<li>Har ditt företag policyer för att ta bort användare?</li> 
<li>Hur många användare har <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Administratörsbehörigheter</a>?</li>
<li>Bör någon av dessa användare ändras till <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">andra roller?</a></li> 
<li>Vilka är <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API-användare</a> i det här fallet?</li></td>
  </tr>
  <tr> 
   <td>Roller</td> 
   <td><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Oavsett om du använder Marketo med Adobe Identity eller inte kan du fortsätta med att granska rollbehörigheter i Marketo Engage under Admin &gt; Användare &amp; roller &gt; Roller.
   <p><li>Hur många roller finns det?</li>  
<li>Vad <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">behörigheter/åtkomst</a> har varje roll? Ska någon justeras?</li>
<li>Hur många användare finns det per roll?</li>
<li>Hur ofta är användare <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">logga in</a>?</li>
<li>Har varje API-användare sina <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">egen användarroll</a>? Om inte, bör du implementera den för att underlätta felsökningen.</li> 
<li>Anpassa era användarroller och behörigheter efter företagets integritetspolicyer för regelefterlevnad (t.ex. <a href="https://gdpr-info.eu/" target="_blank">GDPR</a>)? Gör företagsdata <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">integritetspolicy</a> tillåta användare att hämta och dela användardata för Marketo Engage? Är behörighetsverksamheten nödvändig?</li></td>
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
   <br/>     I så fall kan du granska kategorierna ovan för din sandlåda.</li>
<li>Är <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Programimport</a> länkad till din sandlåda?</li></td>
  </tr>
 </tbody> 
</table>

## Granskningsspår {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
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
   <th style="width:20%">Område</th>
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
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Smarta kampanjer</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Har du en begränsning?</a> på Smart Campaign-storleken? 
   <br/>     Om inte, överväg att lägga till en. Vi rekommenderar att du begränsar Smart Campaign-gränsen till 25 % av databasen för att undvika överkommunikation eller att hela databasen behandlas i arbetsflöden. Detta skyddar inte bara varumärket, utan hjälper till att skydda instansens prestanda.</li></td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbegränsningar</td> 
   <td><li>Finns det <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">kommunikationsgränser</a> på plats? Har ert företag policyer där kommunikationsbegränsningar kan behövas?</li>
<p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Vi rekommenderar att du begränsar din kommunikation till 1 per dag och 3 per 7 dagar med <b>ej</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operativ</a> e-post blockerad.</td>
  </tr>
 </tbody> 
</table>

## Taggar {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Taggar</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Hur många taggar</a> Är det där? Hur många taggar används? Behöver du lägga till något?</li>
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
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Fälthantering</td> 
   <td><li>Hur många fält finns det? 
   <br/>     Klicka <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exportera fältnamn</a> om du vill granska en lista med fält, anpassade fält och deras API-namn.</li>
<li>Hur många <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">anpassade fält</a> Är det där?</li>
<li>Hur många fält används? 
<br/>     Välj <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exportera som används av</a> i listrutan Fältåtgärder för att granska relaterade resurser i ett fält.</li>
<li>Hur många fält synkroniseras mellan Marketo Engage och CRM?</li>
<li>Synkroniseras CRM-fält med rätt objekt?</li>
<li>Finns det en <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">anpassad vyuppsättning</a> för persondetaljer? Borde det vara?</li>
<li>Har du en namngivningsregel för dina fält baserat på källa? 
<br/>     Om inte, överväg att genomföra detta.</li>
<li>Finns det några fält <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">blockerad</a>? 
<br/>     I så fall, se till att förstå varför de är det.</li></td>
  </tr>
  <tr> 
   <td>Anpassade aktiviteter</td> 
   <td><li>Finns det några <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">anpassade aktiviteter</a>?
<br/>     Klicka i så fall igenom dem för att förstå vilka aktiviteter som inte är relaterade till ett Marketo-formulär, e-postmeddelande eller en landningssida.</li></td>
  </tr>
  <tr> 
   <td>Anpassade objekt</td> 
   <td><li>Hur många <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">anpassade objekt</a> Är det där? Hur synkroniseras de med din CRM?</li>
<li>Hur används dessa anpassade objekt av program och listfrågor?</li></td>
  </tr>
 </tbody> 
</table>

## E-post {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>Standardinställningar för e-post</td> 
   <td><li>I Admin &gt; E-post är alla dina standardinställningar aktuella (t.ex. <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">"from", e-post/etikett</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">varumärkesdomän</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">avbeställ meddelande</a>, osv.)?</li></td>
  </tr>
 </tbody> 
</table>

## Integreringar {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Område</th>
   <th>Granska fokus</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Vilken CRM synkroniserar du med? Salesforce? MS Dynamics? Veeva?</li>
<li>Använder du en <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">anpassad synkronisering</a>?</li>
<li>[Endast Salesforce] Har din instans anpassade synkroniseringsfilter implementerats? 
<p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Kontakta Marketo Support om du vill identifiera anpassade synkroniseringsfilter eller begära att en anpassad synkroniseringsregel implementeras.</li></td>
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
<br/>     Bekräfta om dina resurser på landningssidan innehåller en http-URL.</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Är din <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin-spårningskod</a> på din webbplats (inte en landningssida för Marketo Engage)?</li>
<li>Är en <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Spåra inte</a> Webbläsarbegäran aktiverad?</li>
<li>Är din <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">Munchkin API</a> konfigurerad? 
<p><img src="assets/tip-icon.png" alt="ikonen för tips">TIPS: Om du saknar dokumentation om var munkinkoden finns på webbplatsen kan du visa alla URL:er genom att skapa en <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Aktivitetsrapport för webbsida</a>.</li></td>
  </tr>
  <tr> 
   <td>Webbtjänster</td> 
   <td><li>är <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP-begränsningar</a> aktiverad? Borde de vara det?</li>
<li>Vilka användare/appar gör API-anrop i din instans?</li>
<li>Stöter du eller är du nära att stöta på API-gränsen? 
<br/>     Om så är fallet bör du överväga att öka den eller granska instansen för att få ned API-anropen.</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (om tillämpligt)</td> 
   <td><li>Har <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-paketet har installerats</a>?</li>
<li>Har du <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">uppgraderat till den senaste versionen av Sales Insight</a>?</li>
<li>Har du slutfört konfigurationen av Sales Insight? <br/>     Företag/obegränsade användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">klicka här</a>, Professional-användare <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">klicka här</a>.</li>
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
   <th style="width:20%">Område</th>
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
   <th style="width:20%">Område</th>
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

[Granska en ärvd instans: Database ►](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/database-checklist.md)