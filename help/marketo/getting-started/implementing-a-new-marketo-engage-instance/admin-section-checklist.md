---
description: Konfigurera administratörsavsnittet för din nya Marketo Engage-instans.
title: God praxis för nya instanser - checklista för administratörsavsnitt
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# God praxis för nya instanser: Checklista för administratörsavsnitt {#new-instance-best-practices-admin-section-checklist}

Som ny administratör som navigerar i en ny Marketo Engage-instans kan du använda checklistan nedan som hjälp i implementeringsprocessen. Precis som med alla dessa guider kan du även [hämta checklistorna](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) och spåra dina framsteg.

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
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=sv-SE#create-a-new-role" target="_blank">Skapa en ny roll</a> eller <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=sv-SE#edit-a-role" target="_blank">redigera rollerna</a> baserat på organisationens behov.</li>
    <li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Tilldela användare till lämpliga roller</a>. Användarna måste läggas till i prenumerationen i Adobe Admin Console innan de kan tilldela sina roller i Roller. Se avsnittet Användare i checklistan <a href="/help/marketo/getting-started/initial-setup/user-setup.md">Inledande installation</a>.</li>
    <li>Granska antalet användare per roll när du har tilldelat rollerna.</li>
    <li>Implementera en unik roll för varje API-användare för enkel felsökning.</li></td>
  </tr>
  <tr>
    <td>Sandlåda (om tillämpligt)</td>
    <td><li>Granska kategorierna ovan för din <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandlåda</a>.</li></td>
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
    <td><li>Bestäm antalet <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=sv-SE" target="_blank"> arbetsytor</a> och/eller partitioner som din organisation behöver och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=sv-SE" target="_blank">hur många användare som har åtkomst till varje arbetsyta.</a></li>
    <li>Definiera det primära syftet med varje arbetsyta och partition.</li>
    <li>Definiera relationen mellan arbetsytorna och partitionerna.</li></td>
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
    <td><li>Lägg till en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=sv-SE" target="_blank">begränsning för storleken på den smarta kampanjen</a> så att hela databasen inte kan skickas med e-post av misstag.</li></td>
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
    <td><li>Implementera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=sv-SE" target="_blank">kommunikationsbegränsningar</a>.</li>
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
    <td><li>Definiera hur <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=sv-SE" target="_blank">kanaler</a> ska användas.</li></td>
  </tr>
  <tr>
    <td>Taggar</td>
    <td><li>Definiera hur <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=sv-SE" target="_blank">taggar</a> ska användas.</li></td>
  </tr>
  <tr>
    <td>Kalender<br>
    (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=sv-SE" target="_blank">Utfärda licenser för marknadsföringskalender</a> till dem som behöver åtkomst.</li>
    <li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=sv-SE" target="_blank">kalendern</a>.</li></td>
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
    <td><li>Implementera en namnkonvention för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=sv-SE" target="_blank">anpassade fält</a> (till exempel från"MKTO").</li>
    <li>Var selektiv när det gäller de fält du synkroniserar. Ju fler fält du synkroniserar, desto långsammare blir synkroniseringscykeln.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=sv-SE" target="_blank">Blockera uppdateringar av fält</a> som du vill skriva till en gång (t.ex. ursprunglig lead-källa, ursprunglig lead-källinformation, första berörings-UTM-fält osv.).</li></td>
  </tr>
  <tr>
    <td>Anpassade aktiviteter</td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=sv-SE" target="_blank">anpassade aktiviteter</a> som är specifika för ditt företag.</li></td>
  </tr>
  <tr>
    <td>Anpassade objekt</td>
    <td><li>Granska hur många <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=sv-SE" target="_blank">anpassade objekt</a> du behöver.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=sv-SE" target="_blank">Synkronisera de anpassade objekten</a> med CRM.</li></td>
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
    <td><li>Identifiera de behörigheter du behöver för att komma åt CRM.</li>
    <li>Identifiera CRM-administratören för felsökning.</li></td>
  </tr>
  <tr>
    <td>Webbtjänster</td>
    <td><li>Bestäm vilka användare/appar som kan göra <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=sv-SE" target="_blank">API-anrop</a> i din instans.</li>
    <li>Granska alla program som ska göra API-anrop och kontrollera om det behövs fler eller färre API-anrop.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=sv-SE" target="_blank">LaunchPoint</a>-tjänster för ditt företag. Varje LaunchPoint ska kombineras med en unik API-användare för att underlätta felsökning.</li></td>
  </tr>
  <tr>
    <td>Interaktiva webbinarier (om tillämpligt)</td>
    <td><li>När du skapar interaktiva webbinarier lägger Marketo Engage inbyggda webbinariefunktion till <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">användare i användaravsnittet</a> på fliken Interaktivt webbinarium.</li>
    <p><img src="assets/note-icon.png" alt="anteckningsikon"> OBS! Interaktiva webbinarier tillhandahålls endast till produktionsinstanser.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (om tillämpligt)</td>
    <td><li>Tilldela användare till <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'Åtkomst till Dynamic Chat'-roller</a> i Marketo Engage &gt; Admin &gt; Användare &amp; roller.</li></td>
  </tr>
  <tr>
    <td>Försäljningsinsikter (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Ställ in Sales Insight-åtgärd</a> i Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=sv-SE#invite-individual-users-to-msi-actions" target="_blank">Utfärda licenser</a> till lämpliga användare.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=sv-SE" target="_blank">Konfigurera API</a>.</li>
    <li>Anpassa <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=sv-SE" target="_blank">lead-poängen</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (om tillämpligt)</td>
    <td><li>Bjud in lämpliga Marketo Engage-administratörer till <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect-instansen</a>.</li>
    <li>Slutför de <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">extra administratörsinställningarna för Sales Connect</a> i Sales Connect och Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=sv-SE" target="_blank">Skapa eventuella nödvändiga webbhooks</a> för ditt företag.</li>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=sv-SE" target="_blank">Aktivera skattetesten</a> om du vill experimentera med piltningsfunktioner.</li>
    <li>Bestäm vilka funktioner du vill aktivera eller inaktivera.</li></td>
  </tr>
  <tr>
    <td>Campaign Inspector </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=sv-SE" target="_blank">Aktivera Campaign Inspector</a> om du vill visa alla smarta kampanjer på ett och samma ställe.</li></td>
  </tr>
</tbody>
</table>
