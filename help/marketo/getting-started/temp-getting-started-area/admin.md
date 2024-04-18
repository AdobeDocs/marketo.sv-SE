---
description: NYTT OMRÅDE - Marketo Docs - produktdokumentation
title: NYTT OMRÅDE
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 0%

---

# NYTT OMRÅDE: Administratörschecklista {#new-area-admin-checklist}

Intro text.

## Roller {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Roller</td>
    <td><li>Granska de färdiga rollerna och bekräfta vilka behörigheter/behörigheter varje roll har.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Skapa en ny roll</a> eller <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">redigera rollerna</a> baserat på organisationens behov och hur ofta användarna loggar in.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">Tilldela användare till lämpliga roller</a>. Användarna måste läggas till i prenumerationen i Adobe Admin Console innan de kan tilldela roller i roller. Se avsnittet Användare i checklistan Inledande installation [LINK]. <br>När du har tilldelat rollerna för användarna ska du granska antalet användare per roll.<br>Implementera en unik roll för varje API-användare för enkel felsökning.</td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td>Definiera användare och roller för din organisation.<br>Definiera processen för att lägga till en ny användare/administratör.</td>
  </tr>
  <tr>
    <td>Sandlåda (om tillämpligt)</td>
    <td>Granska kategorierna ovan för din sandlåda om du har en sådan.</td>
  </tr>
</tbody>
</table>

## Arbetsytor och partitioner {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Arbetsytor och partitioner (om tillämpligt)</td>
    <td>Bestäm antalet<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> arbetsytor</a> och/eller partitioner som din organisation behöver och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">hur många användare som har åtkomst till varje arbetsyta.</a><br>Definiera det primära syftet med varje arbetsyta och partition.<br>Definiera relationen mellan arbetsytorna och partitionerna.</td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td>Dokumentera hur arbetsytor definieras och hur relaterar det till databaspartitioner (dvs. en global arbetsyta som ser alla, jämfört med affärssektorer). <br>Importera nya poster till lämplig partition.<br>Definiera värdet i CRM som placerar användare i rätt partition.</td>
  </tr>
</tbody>
</table>

## Inställningar för smart kampanj {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Inställningar för smart kampanj</td>
    <td>Lägg till en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">begränsning av storleken på Smart Campaign</a>, vilket förhindrar att hela databasen postas av misstag.</td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td>Dokumentera hur arbetsytor definieras och hur relaterar det till databaspartitioner (dvs. en global arbetsyta som ser alla, jämfört med affärssektorer).  <br>Importera nya poster till lämplig partition.<br>Definiera värdet i CRM som placerar användare i rätt partition.</td>
  </tr>
</tbody>
</table>

## E-postinställningar {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-poststandard</td>
    <td>Under Varumärkesdomän väljer du din domän och lägger till din e-post-CNAME. Detta ska vara i formatet: [EmailTrackingCNAME].[CompanyDomain].com.  <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Kontakta Marketo support</a> för att skydda den med SSL-certifikat. Den här processen kan ta upp till tre arbetsdagar att slutföra.</td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Konfigurera SPF och DKIM</a> för e-postleverans.</td>
  </tr>
  <tr>
  </tr>
  <tr>
  </tr>
</tbody>
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kommunikationsbegränsningar</td>
    <td>Montera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank" rel="noopener noreferrer">Kommunikationsbegränsningar</a>.<br>Kontrollera om ditt företag behöver en policy för kommunikationsbegränsningar </td>
  </tr>
</tbody>
</table>

## Taggar {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kanaler</td>
    <td>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank" rel="noopener noreferrer">kanaler</a>.</td>
  </tr>
  <tr>
    <td>Taggar</td>
    <td>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank" rel="noopener noreferrer">taggar</a>.</td>
  </tr>
  <tr>
    <td>Kalender (om tillämpligt)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank" rel="noopener noreferrer">Utfärda licenser för marknadsföringskalender</a> till dem som behöver åtkomst. <br>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank" rel="noopener noreferrer">Kalender.</a></td>
  </tr>
</tbody>
</table>

## Databashantering {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Fälthantering</td>
    <td>Implementera namnkonvention för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">anpassade fält.</a> Börja till exempel med "MKTO".<br>Var selektiv när det gäller de fält du synkroniserar. Ju fler fält du synkroniserar, desto långsammare blir synkroniseringscykeln.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Blockera uppdateringar av fält</a> du vill skriva till en gång (d.v.s. ursprunglig lead-källa, information om ursprunglig lead-källa, första berörings-UTM-fält osv.)</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td>Anpassade aktiviteter</td>
    <td>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Anpassade aktiviteter</a> som är specifika för ditt företag.  </td>
  </tr>
  <tr>
    <td>Anpassade objekt</td>
    <td>Granska hur många <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Anpassade objekt</a> du behöver. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Synkronisera de anpassade objekten till CRM</a>. </td>
  </tr>
</tbody>
</table>

## Integreringar {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td>Initiera CRM-synkronisering. Välj något av följande, beroende på vilken CRM ditt företag använder: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>. <br>Identifiera vilken typ av åtkomst du behöver för att komma åt CRM. <br>Identifiera CRM-administratören för felsökning. </td>
  </tr>
  <tr>
    <td>Landningssidor</td>
    <td>Obs! Är du kund som lanseringspaket? Du kan hoppa över det här steget. Din konsult kommer att ge dig ett dokument med instruktioner för IT-konfiguration under samtalet. <br>Konfigurera landningssidans domän med en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">ange domän- och sidinformation</a>. Detta ska vara i formatet: [LandingPageCNAME].[CompanyDomain].com <br>Välj en CNAME för dina landningssidor. Några exempel: <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Kontakta Marketo support</a> för att starta processen med att etablera ett SSL-certifikat. Den här processen kan ta upp till tre arbetsdagar att slutföra. <br>TIPS: Håll det kort! Kortare URL:er är enklare att komma ihåg. Vi föreslår "gå" som domän. <br>Lägg till analysspårningskod (t.ex. Google Analytics eller Adobe Analytics) i era landningssidmallar. </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>Obs! Om du är kund som använder Launch Pack hoppar du över det här steget. Din konsult kommer att ge dig instruktioner om Munchkins kod i ditt dokument med IT-konfigurationsinstruktioner. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">Lägg till Munchkin-spårningskod</a> till er webbplats. Munchkin-kod kan vara <a href="https://developers.marketo.com/javascript-api/lead-tracking/">hårdkodad</a> eller via Google Tag Manager.  </td>
  </tr>
  <tr>
    <td>Webbtjänster</td>
    <td>Aktivera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html">IP-begränsningarna</a> om tillämpligt. <br>Bestäm vilka användare/appar som kan göra <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">API-samtal</a> i din instans. <br>Granska alla program som ska göra API-anrop och kontrollera om en ökning eller en klippgräns behövs för API-anropen.  </td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td>Ange obligatoriskt <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> tjänster för ditt företag. Varje LaunchPoint ska kombineras med en unik API-användare för att underlätta felsökning.  </td>
  </tr>
  <tr>
    <td>Interaktiva webbinarier (om tillämpligt)</td>
    <td>OBS! Interaktiva webbinarier tillhandahålls endast till produktionsinstanser. <br>Den inbyggda webbinariefunktionen för interaktiva webbinarier <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">lägga till användare i avsnittet Användare</a> på fliken Interactive Webinar. </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (om tillämpligt)</td>
    <td>För att använda <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>, den inbyggda konversationskanalen i Marketo Engage, fortsätter du med användarbehörighetsinställningarna enligt stegen nedan <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Bekräfta om du har tilldelats en produktadministratörsroll för Adobe av systemadministratören för Adobe Org. Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe kundtjänst</a> för att ta reda på vem i organisationen som har administratörsbehörighet i konsolen. <br>Acceptera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">inbjudan till produktadministratör för Dynamic Chat</a>. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">välkomstmeddelande</a> skickas när Dynamic Chat är aktiverat i din Marketo Engage-instans och du har utsetts till systemadministratör.  <br>Tilldela alla lämpliga användare till Dynamic Chat produktprofil i Adobe Admin Console. <br>Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Dynamic Chat. <br>Du kan <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">redigera produktprofiler i Dynamic Chat</a> och skapa en egen profil med en anpassad uppsättning <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">behörigheter som är tillgängliga i din prenumeration</a>. <br>Tilldela användare till <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Dynamic Chat-roller i Access</a> i Marketo Engage/Admin/Users &amp; Roles. </td>
  </tr>
  <tr>
    <td>Försäljningsinsikter (om tillämpligt)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Ställ in Sales Insight-åtgärd</a> i Sales Insight&gt;Actions Config.  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Utfärda licenser till lämpliga användare.</a>  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Konfigurera API:t</a>. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Anpassa poängen för leads.</a> </td>
  </tr>
  <tr>
    <td>Sales Connect (om tillämpligt)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Bjud in lämpliga Marketo Engage-administratörer till Sales Connect-instansen</a>. <br>Slutför <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">ytterligare inställningar för Sales Connect-administratör</a> i Sales Connect och Salesforce. </td>
  </tr>
</tbody>
</table>

## Treasure Chest {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Treasure Chest </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Aktivera skattetest</a> för att experimentera med pilottfunktioner.  <br>Bestäm vilka funktioner du vill aktivera eller inaktivera. </td>
  </tr>
  <tr>
    <td>Campaign Inspector </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Aktivera Campaign Inspector</a> för att visa alla smarta kampanjer samtidigt. </td>
  </tr>
</tbody>
</table>
