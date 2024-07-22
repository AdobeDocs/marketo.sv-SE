---
description: Dokumentera konfigurationen av din nya Marketo Engage-instans.
title: Nya instansmetodtips - Dokumentera dina inställningar
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Nya instansmetodtips: Dokumentera dina inställningar {#new-instance-best-practices-document-your-setup}

Nu när du har lärt dig de viktigaste produktområdena för att skapa en ny instans i Marketo Engage är nästa steg att skapa dokumentation för din instanskonfiguration och tekniska stack. Oavsett om du skapar det via kalkylblad eller en projektledningsapplikation är din dokumentation en bra resurs för att spåra framsteg och registrera detaljer, samt hålla instansen strukturerad och hållbar för framtida marknadsförare inom organisationen.

## Data {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listimport</td>
    <td><li>Samla in en lista med datakällor som poster hämtas från till <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">importera till Marketo Engage</a>.</li>
    <li>Om du importerar från flera datakällor kan det vara bra att använda huvudlistor eller <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">skapa ett anpassat fält</a> i personposten för att ange datakällan.</li></td>
  </tr>
  <tr>
    <td>Databasintegrering</td>
    <td><li>Om du använder den inbyggda synkroniseringen mellan Marketo Engage och CRM bör du noga tänka på vilka fält du vill synkronisera mellan systemen. Alla fält behöver inte synkroniseras, så var strategiska med dataflödena.</li></td>
  </tr>
</tbody>
</table>

## Dokumentation {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Användare</td>
    <td><li>Dokumentera de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">aktuella användarna</a> i din instans av säkerhetsskäl. Följande information bör inkluderas minst (och visas alla genom att gå till Admin &gt; Användare &amp; roller):</li>
    <ul>
    <li>Namn</li>
    <li>E-post</li>
    <li>Inloggning</li>
    <li>Roll</li>
    <li>Åtkomstens förfallodatum</li>
    <li>Skapad av användaren</li>
    <li>Senaste inloggningsdatum</li></ul>
    <p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Du kan även utöka den här för att inkludera dokumentation om roller/behörigheter.
    <p>
    <li>Som produktadministratör för Marketo Engage ska du utveckla en intern process för att granska och uppdatera användarlistan för Marketo Engage med jämna mellanrum. Om du vill göra ändringar i listan över användare i Adobe Admin Console bör du överväga <a href="https://helpx.adobe.com/enterprise/using/users.html" target="_blank">massåtgärder</a>, till exempel att överföra en .CSV-fil med REST-API:t för användarhantering.</li></td>
  </tr>
  <tr>
    <td>Organisation</td>
    <td><li>Dokumentera den överenskomna mappstrukturen, standardnamnkonventioner för program, resurser osv. och varför besluten fattas. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Läs mer om de bästa metoderna här.</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Skapa en ändringslogg där du kan dokumentera vad som ändras i instansen och varför ändringarna görs. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Läs mer om de bästa metoderna här.</a></li></td>
  </tr>
  <tr>
    <td>Playbooks</td>
    <td><li>Skapa en användarspelbok eller en admin-spelbok för att interna användare ska kunna komma igång med instansen.</li></td>
  </tr>
  <tr>
    <td>Konversationer med interna team</td>
    <td><li>Anpassa marknadsföringsteamets förväntningar på Marketo Engage med Marketo Engage.</li>
    <li>Identifiera de team som kommer att vara era intressenter i Marketo Engage och dokumentera deras mål för att uppnå användning av Marketo Engage som teknik.</li></td>
  </tr>
  <tr>
    <td>Arbetsytor och partitioner (om tillämpligt)</td>
    <td><li>Dokumentera hur arbetsytor definieras och hur det relaterar till databaspartitioner (t.ex. en global arbetsyta som visar alla kontra affärssektorer).</li>
    <li>Importera nya poster till rätt partition.</li>
    <li>Definiera värdet i CRM som placerar användarna i rätt partition.</li></td>
  </tr>
</tbody>
</table>
