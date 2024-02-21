---
description: NYTT OMRÅDE - Marketo Docs - produktdokumentation
title: NYTT OMRÅDE
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 7d8cdb2da42769ee0326a3d585ad32a3405dfac1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# NYTT OMRÅDE: Administratörschecklista {#new-area-admin-checklist}

Intro text.

## Roller {#roles}

<table>
<thead>
  <tr>
    <th>Område </th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Roller </td>
    <td><li>Granska de färdiga rollerna och bekräfta vilka behörigheter/behörigheter varje roll har.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Skapa en ny roll</a> eller <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">redigera rollerna</a> baserat på organisationens behov och hur ofta användarna loggar in.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Tilldela användare till lämpliga roller</a>.</li>
    <li>När du har tilldelat rollerna för användarna ska du granska antalet användare per roll.</li>  <li>Implementera en unik roll för varje API-användare för enkel felsökning.</li></td>
  </tr>
  <tr>
    <td>Dokumentation </td>
    <td>Definiera användare och roller för din organisation. <br>Definiera processen för att lägga till en ny användare/administratör. </td>
  </tr>
  <tr>
    <td>Sandlåda (om tillämpligt) </td>
    <td>Granska kategorierna ovan för din sandlåda om du har en sådan. </td>
  </tr>
</tbody>
</table>

## Arbetsytor och partitioner {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Arbetsytor och partitioner </td>
    <td><li>Bestäm antalet<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> arbetsytor</a> och/eller partitioner som din organisation behöver och <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">hur många användare som har åtkomst till varje arbetsyta.</a></li>
    <li>Definiera det primära syftet med varje arbetsyta och partition.</li>
    <li>Definiera relationen mellan arbetsytorna och partitionerna.</li></td>
  </tr>
  <tr>
    <td>Dokumentation </td>
    <td><li>Dokumentera hur arbetsytor definieras och hur relaterar det till databaspartitioner (dvs. en global arbetsyta som ser alla, jämfört med affärssektorer).</li>
    <li>Importera nya poster till lämplig partition.</li>
    <li>Definiera värdet i CRM som placerar användare i rätt partition.</li></td>
  </tr>
</tbody>
</table>

## Inställningar för smart kampanj {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Inställningar för smart kampanj </td>
    <td><li>Lägg till en <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">begränsning av storleken på Smart Campaign</a>, vilket förhindrar att hela databasen postas av misstag.</li>
    <li>Aktivera personbegränsningar för smarta kampanjer</li></td>
  </tr>
</tbody>
</table>

## E-postinställningar {#email-settings}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-poststandard</td>
    <td><li>Under Varumärkesdomän väljer du din domän och lägger till din e-post-CNAME. Detta ska vara i formatet: [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Konfigurera SPF och DKIM</a> för e-postleverans.</li></td>
  </tr>
</tbody>
</table>

## Kommunikationsbegränsningar {#communication-limits}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kommunikationsbegränsningar</td>
    <td><li>Montera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Kommunikationsbegränsningar</a>.</li>
    <li>Kontrollera om ditt företag behöver en policy för kommunikationsbegränsningar.</li></td>
  </tr>
</tbody>
</table>

## Taggar {#tags}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kanaler</td>
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">kanaler</a>.</li></td>
  </tr>
  <tr>
    <td>Taggar </td>
    <td><li>Definiera hur du använder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">taggar</a>.</li></td>
  </tr>
  <tr>
    <td>Kalender (om tillämpligt) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Utfärda licenser för marknadsföringskalender</a> till dem som behöver åtkomst.</li> 
    <li>Konfigurera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Kalender</a>.</li></td>
  </tr>
</tbody>
</table>

## Databashantering {#database-management}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Fälthantering</td>
    <td><li>Implementera namnkonvention för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">anpassade fält.</a> Börja till exempel med "MKTO".</li>
    <li>Var selektiv när det gäller de fält du synkroniserar. Ju fler fält du synkroniserar, desto långsammare blir synkroniseringscykeln.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Blockera uppdateringar av fält</a> du vill skriva till en gång (d.v.s. ursprunglig lead-källa, information om ursprunglig lead-källa, första berörings-UTM-fält osv.).</li></td>
  </tr>
  <tr>
    <td>Anpassade aktiviteter </td>
    <td><li>Definiera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">Anpassade aktiviteter</a> som är specifika för ditt företag.</li></td>
  </tr>
  <tr>
    <td>Anpassade objekt </td>
    <td><li>Granska hur många <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">Anpassade objekt</a> du behöver.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">Synkronisera de anpassade objekten till CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## Integreringar {#integrations}

<table>
<thead>
  <tr>
    <th>Område</th>
    <th>Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Initiera CRM-synkronisering. Välj något av följande, beroende på vilken CRM ditt företag använder: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>Identifiera vilken typ av åtkomst du behöver för att komma åt CRM.</li>
    <li>Identifiera CRM-administratören för felsökning.</li></td>
  </tr>
  <tr>
    <td>Försäljningsinsikter (om tillämpligt)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Ställ in Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">Utfärda licenser till lämpliga användare.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">Konfigurera API:t</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">Anpassa poängen för leads.</a></li></td>
  </tr>
</tbody>
</table>
