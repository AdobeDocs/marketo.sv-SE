---
description: NYTT OMRÅDE - Marketo Docs - produktdokumentation
title: NYTT OMRÅDE
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 0%

---

# NYTT OMRÅDE: Administratörschecklista {#new-area-admin-checklist}

Intro text.

## Roller {#roles}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Roller</td>
    <td><li>Granska de färdiga rollerna och bekräfta vilka behörigheter/behörigheter varje roll har.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Skapa en ny roll</a> eller <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">redigera rollerna</a> baserat på organisationens behov och hur ofta användarna loggar in.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Tilldela användare till lämpliga roller</a>.</li>
    <li>När du har tilldelat rollerna för användarna ska du granska antalet användare per roll.</li>  <li>Implementera en unik roll för varje API-användare för enkel felsökning.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td>Definiera användare och roller för din organisation. <br>Definiera processen för att lägga till en ny användare/administratör.</td>
    <td></td>
  </tr>
  <tr>
    <td>Sandlåda (om tillämpligt)</td>
    <td>Granska kategorierna ovan för din sandlåda om du har en sådan.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Arbetsytor och partitioner {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Arbetsytor och partitioner </td>
    <td><li>Bestäm antalet<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> arbetsytor</a> och/eller partitioner som din organisation behöver och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">hur många användare som har åtkomst till varje arbetsyta.</a></li>
    <li>Definiera det primära syftet med varje arbetsyta och partition.</li>
    <li>Definiera relationen mellan arbetsytorna och partitionerna.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Dokumentera hur arbetsytor definieras och hur relaterar det till databaspartitioner (dvs. en global arbetsyta som ser alla, jämfört med affärssektorer).</li>
    <li>Importera nya poster till lämplig partition.</li>
    <li>Definiera värdet i CRM som placerar användare i rätt partition.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Inställningar för smart kampanj {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Inställningar för smart kampanj </td>
    <td><li>Lägg till en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">begränsning av storleken på Smart Campaign</a>, vilket förhindrar att hela databasen postas av misstag.</li>
    <li>Aktivera personbegränsningar för smarta kampanjer</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## E-postinställningar {#email-settings}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-poststandard</td>
    <td><li>Under Varumärkesdomän väljer du din domän och lägger till din e-post-CNAME. Detta ska vara i formatet: [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Konfigurera SPF och DKIM</a> för e-postleverans.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kommunikationsbegränsningar</td>
    <td><li>Montera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Kommunikationsbegränsningar</a>.</li>
    <li>Kontrollera om ditt företag behöver en policy för kommunikationsbegränsningar.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Taggar {#tags}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kanaler</td>
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">kanaler</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Taggar </td>
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">taggar</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Kalender (om tillämpligt) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Utfärda licenser för marknadsföringskalender</a> till dem som behöver åtkomst.</li> 
    <li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Kalender</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Databashantering {#database-management}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Fälthantering</td>
    <td><li>Implementera namnkonvention för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">anpassade fält.</a> Börja till exempel med "MKTO".</li>
    <li>Var selektiv när det gäller de fält du synkroniserar. Ju fler fält du synkroniserar, desto långsammare blir synkroniseringscykeln.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blockera uppdateringar av fält</a> du vill skriva till en gång (d.v.s. ursprunglig lead-källa, information om ursprunglig lead-källa, första berörings-UTM-fält osv.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Anpassade aktiviteter </td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Anpassade aktiviteter</a> som är specifika för ditt företag.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Anpassade objekt </td>
    <td><li>Granska hur många <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Anpassade objekt</a> du behöver.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Synkronisera de anpassade objekten till CRM</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Integreringar {#integrations}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Initiera CRM-synkronisering. Välj något av följande, beroende på vilken CRM ditt företag använder: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Identifiera vilken typ av åtkomst du behöver för att komma åt CRM.</li>
    <li>Identifiera CRM-administratören för felsökning.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Försäljningsinsikter (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Ställ in Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Utfärda licenser till lämpliga användare.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Konfigurera API:t</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Anpassa poängen för leads.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Landningssidor </td>
    <td>Obs! Är du kund som lanseringspaket? Du kan hoppa över det här steget. Din konsult kommer att ge dig ett dokument med instruktioner för IT-konfiguration under samtalet. <br>Konfigurera landningssidans domän med en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">ange domän- och sidinformation</a>. Detta ska vara i formatet: [LandingPageCNAME].[CompanyDomain].com <br>Välj en CNAME för dina landningssidor. Några exempel: <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br>TIPS: Håll det kort! Kortare URL:er är enklare att komma ihåg. Vi föreslår "gå" som domän. <br>Lägg till analysspårningskod (t.ex. Google Analytics eller Adobe Analytics) i era landningssidmallar. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Redigera inställningar för landningssida</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">Obs! Om du är kund som använder Launch Pack hoppar du över det här steget. Din konsult kommer att ge dig instruktioner om Munchkins kod i ditt dokument med IT-konfigurationsinstruktioner. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Lägg till Munchkin-spårningskod</a> till er webbplats. Munchkin-kod kan vara <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">hårdkodad</a> eller via Google Tag Manager.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Lägg till Munchkin-spårkod på din webbplats</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Spårning av leads</a> </td>
  </tr>
  <tr>
    <td>Webbtjänster </td>
    <td>Aktivera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">IP-begränsningarna</a> om tillämpligt. <br>Bestäm vilka användare/appar som kan göra <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API-samtal</a> i din instans. <br>Granska alla program som ska göra API-anrop och kontrollera om en ökning eller en klippgräns behövs för API-anropen.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Skapa ett Tillåtelselista för IP-baserad API-åtkomst </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (om tillämpligt) </td>
    <td>För att använda <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, den inbyggda konversationskanalen i Marketo Engage, fortsätter du med inställningarna för användarbehörighet enligt stegen nedan <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Bekräfta om du har tilldelats en produktadministratörsroll för Adobe av systemadministratören för Adobe Org. Kontakt <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe kundtjänst</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> för att ta reda på vem i organisationen som har administratörsbehörighet i konsolen. <br>Acceptera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">inbjudan till produktadministratör för Dynamic Chat</a>. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">välkomstmeddelande</a> skickas när Dynamic Chat är aktiverat i din Marketo Engage-instans och du har utsetts till systemadministratör.  <br>Tilldela alla lämpliga användare till produktprofilen i Marketo Engage i Adobe Admin Console. <br>Du kan inte tilldela användarroller i Marketo Engage/Admin/Users &amp; Roles innan du lägger till dem i en produktprofil.  <br>Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Startpunkt (om tillämpligt) </td>
    <td>Ställ in alla nödvändiga <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> tjänster för ditt företag.  <br>OBS! Interaktiva webbinarier är en inbyggd webbinariefunktion med inbyggd integrering i Adobe Connect. Ingen ytterligare integrering behövs, men instansen måste <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">synkronisera till Adobe Connect som en LaunchPoint-tjänst.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Ytterligare integreringar</a> </td>
  </tr>
  <tr>
    <td>Webhooks (om tillämpligt)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Skapa de webbhotell som behövs</a> för er verksamhet.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Skapa en webbkrok</a> </td>
  </tr>
</tbody>
</table>

## Treasure Chest {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
    <th>Prioritet</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Treasure Chest</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Aktivera skattetest</a> för att experimentera med pilottfunktioner.  <br>Bestäm vilka funktioner du vill aktivera eller inaktivera.</td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Campaign Inspector </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Aktivera Campaign Inspector</a> för att visa alla smarta kampanjer samtidigt.</td>
    <td>Text</td>
  </tr>
</tbody>
</table>
