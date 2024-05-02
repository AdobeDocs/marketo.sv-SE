---
description: Ställ in administratörsavsnittet för den nya Marketo Engage-instansen.
title: God praxis för nya instanser - checklista för administratörsavsnitt
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: fa5b686aabd3aab2d9020758fde00ed06564c76c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# God praxis för nya instanser: Checklista för administratörsavsnitt {#new-instance-best-practices-admin-section-checklist}

När en ny administratör navigerar i en ny Marketo Engage-instans kan du använda checklistan nedan som hjälp i implementeringsprocessen. Precis som med alla dessa guider kan du hämta checklistorna [LÄNK] och spåra dina framsteg.

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
    <td><li>Granska de färdiga rollerna och bekräfta vilka behörigheter/behörigheter varje roll har.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Skapa en ny roll</a> eller <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">redigera rollerna</a> baserat på organisationens behov.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Tilldela användare till lämpliga roller</a>. Användarna måste läggas till i prenumerationen i Adobe Admin Console innan de kan tilldela roller i roller. Se avsnittet "Användare" i <a href="/help/marketo/getting-started-2/initial-setup/user-setup.md">Inledande installationschecklista</a>.</li>
    <li>Granska antalet användare per roll när du har tilldelat rollerna.</li>
    <li>Implementera en unik roll för varje API-användare för enkel felsökning.</li></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Definiera användare och roller för din organisation.</li>
    <li>Definiera processen för att lägga till en ny användare/administratör.</li></td>
  </tr>
  <tr>
    <td>Sandlåda (om tillämpligt)</td>
    <td><li>Granska kategorierna ovan för <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">sandlåda</a>.</li></td>
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
    <td><li>Bestäm antalet<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> arbetsytor</a> och/eller partitioner som din organisation behöver och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">hur många användare som har åtkomst till varje arbetsyta.</a></li>
    <li>Definiera det primära syftet med varje arbetsyta och partition.</li>
    <li>Definiera relationen mellan arbetsytorna och partitionerna.</li></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Dokumentera hur arbetsytor definieras och hur det relaterar till databaspartitioner (t.ex. en global arbetsyta som visar alla kontra affärssektorer).</li>
    <li>Importera nya poster till rätt partition.</li>
    <li>Definiera värdet i CRM som placerar användarna i rätt partition.</li></td>
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
<tbody>
  <tr>
    <td>Inställningar för smart kampanj</td>
    <td><li>Lägg till en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">begränsning av storleken på Smart Campaign</a>, vilket förhindrar att hela databasen skickas med e-post.</li></td>
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
    <td><li>Under Varumärkesdomän väljer du din domän och lägger till din e-post-CNAME. Detta ska vara i formatet: [EmailTrackingCNAME].[CompanyDomain].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Kontakta Marketo support</a> för att skydda den med SSL-certifikat. Den här processen kan ta upp till tre arbetsdagar att slutföra.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Konfigurera SPF och DKIM</a> för e-postleverans.</li></td>
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
    <td><li>Initiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">kommunikationsgränser</a>.</li>
    <li>Kontrollera om ditt företag behöver en policy för kommunikationsgränser.</li></td>
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
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">kanaler</a>.</li></td>
  </tr>
  <tr>
    <td>Taggar</td>
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">taggar</a>.</li></td>
  </tr>
  <tr>
    <td>Kalender (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Utfärda licenser för marknadsföringskalender</a> till dem som behöver åtkomst.</li>
    <li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Kalender</a>.</li></td>
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
    <td><li>Implementera en namnkonvention för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">anpassade fält</a> (till exempel från"MKTO").</li>
    <li>Var selektiv när det gäller de fält du synkroniserar. Ju fler fält du synkroniserar, desto långsammare blir synkroniseringscykeln.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blockera uppdateringar av fält</a> du vill skriva till en gång (t.ex. ursprunglig lead-källa, information om ursprunglig lead-källa, första berörings-UTM-fält osv.).</li></td>
  </tr>
  <tr>
    <td>Anpassade aktiviteter</td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Anpassade aktiviteter</a> som är specifika för ditt företag.</li></td>
  </tr>
  <tr>
    <td>Anpassade objekt</td>
    <td><li>Granska hur många <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Anpassade objekt</a> du behöver.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Synkronisera de anpassade objekten till CRM</a>.</li></td>
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
    <td><li>Initiera CRM-synkronisering. Välj något av följande, beroende på vilken CRM ditt företag använder: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>Identifiera vilken typ av åtkomst du behöver för att komma åt CRM.</li>
    <li>Identifiera CRM-administratören för felsökning.</li></td>
  </tr>
  <tr>
    <td>Webbtjänster</td>
    <td><li>Bestäm vilka användare/appar som kan göra <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">API-samtal</a> i din instans.</li>
    <li>Granska alla program som ska göra API-anrop och kontrollera om det behövs fler eller färre API-anrop.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> tjänster för ditt företag. Varje LaunchPoint ska kombineras med en unik API-användare för att underlätta felsökning.</li></td>
  </tr>
  <tr>
    <td>Interaktiva webbinarier (om tillämpligt)</td>
    <td>OBS! Interaktiva webbinarier tillhandahålls endast till produktionsinstanser.
    <li>Den inbyggda webbinariefunktionen för interaktiva webbinarier <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">lägga till användare i avsnittet Användare</a> på fliken Interactive Webinar.</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (om tillämpligt)</td>
    <td><li>Tilldela användare till <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Dynamic Chat-roller i Access</a> i Marketo Engage &gt; Admin &gt; Användare &amp; roller.</li></td>
  </tr>
  <tr>
    <td>Försäljningsinsikter (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Ställ in Sales Insight-åtgärd</a> i Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Utfärda licenser till lämpliga användare</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Konfigurera API:t</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Anpassa leadpoängen</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Bjud in lämpliga Marketo Engage-administratörer till Sales Connect-instansen</a>.</li>
    <li>Slutför <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">ytterligare inställningar för Sales Connect-administratör</a> i Sales Connect och Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html">Skapa de webbhotell som behövs</a> för er verksamhet.</li>
    </td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Aktivera skattetest</a> för att experimentera med pilottfunktioner.</li>
    <li>Bestäm vilka funktioner du vill aktivera eller inaktivera.</li></td>
  </tr>
  <tr>
    <td>Campaign Inspector </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Aktivera Campaign Inspector</a> för att visa alla smarta kampanjer samtidigt.</li></td>
  </tr>
</tbody>
</table>
