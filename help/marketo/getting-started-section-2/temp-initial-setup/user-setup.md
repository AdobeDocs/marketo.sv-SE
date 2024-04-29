---
description: Checklista för tidig installation - Marketo Docs - produktdokumentation
title: Checklista för tidig installation
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# NYTT OMRÅDE: Checklista för tidig installation {#early-setup-checklist}

Intro text.

## Marketo Engage på Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och produktadministratör för Marketo Engage </td>
    <td><li>Bekräfta att du har tilldelats en Adobe-produktadministratörsroll av systemadministratören för Adobe Org.</li>  
    <ul>
    <li>Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe kundtjänst</a> för att ta reda på vem i organisationen som har <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console systemadministratör</a> behörighet.</li></ul>
    <li>Acceptera inbjudan till produktadministratör för Marketo Engage för att aktivera din Adobe ID. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">välkomstmeddelande</a> skickas när rollen tilldelas i Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler</td>
    <td><li>Tilldela alla lämpliga användare till Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Produktprofil</a> i Adobe Admin Console.</li>
    <ul>
    <li>Du kan inte tilldela användarroller i Marketo Engage/Admin/Users &amp; Roles innan du lägger till dem i en produktprofil.</li>
    <li>Varje prenumeration blir en fristående produktprofil. Om en oönskad användare läggs till i flera produktprofiler (t.ex. produktions- och testsandlådan) måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td><li>Skapa en profil för när <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">skapa en användare</a>.</li> <li>Skapa en profil för när användare ska tas bort.</li>
    <li>Bestäm vem som ska ha <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe systemadministratörsbehörighet och Marketo Engage produktadministratörsbehörighet.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Lägg till användare</a> till önskad produktprofil.</li>
    <li>Skapa en API-användare för varje API-användningsfall.</li></td>
  </tr>
  <tr>
    <td>Produktsupportadministratör </td>
    <td><li>Till <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">skicka en supportanmälan i Adobe Admin Console</a>måste du ha rollen 'Product Support Administrator' tilldelad av en systemadministratör till de prenumerationer du hanterar. Endast en systemadministratör i din organisation kan <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">tilldela dig till den här rollen</a>.</li>
    <li>Du kan ha fått ett e-postmeddelande från systemadministratören om att du är supportadministratör för din Marketo Engage-prenumeration. I så fall klickar du på <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">Kom igång i e-postmeddelandet</a> för att gå med i organisationen.</li>
    <li>Bestäm lämpliga kontakter (med minst en kontaktperson för säkerhetskopiering) och låt systemadministratören tilldela rollen produktsupportadministratör i förväg.</li></td>
  </tr>
</tbody>
</table>

## Installationsprogram för Dynamic Chat i Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

TEXT

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och produktadministratör för Dynamic Chat (om tillämpligt) </td>
    <td><li>Bekräfta om du har tilldelats en produktadministratörsroll för Adobe av systemadministratören för Adobe Org. Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe kundtjänst</a> för att ta reda på vem i organisationen som har administratörsbehörighet i konsolen.</li>
    <li>Acceptera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">inbjudan till produktadministratör för Dynamic Chat</a>. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">välkomstmeddelande</a> skickas när Dynamic Chat är aktiverat i din Marketo Engage-instans och du har utsetts till systemadministratör.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler </td>
    <td><li>Tilldela alla lämpliga användare till Dynamic Chat produktprofil i Adobe Admin Console.</li> 
    <ul>
    <li>Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Dynamic Chat.</li>
    <li>Du kan <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">redigera produktprofiler i Dynamic Chat</a> och skapa en egen profil med en anpassad uppsättning <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">behörigheter som är tillgängliga i din prenumeration</a>.</li></td>
  </tr>
  <tr>
    <td>Användare </td>
    <td><li>Skapa en profil för när en chattanvändare ska läggas till och tas bort.</li>
    <li>Skapa en profil för vem som ska ha <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat produktadministratörsbehörigheter.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Lägg till användare i önskad produktprofil</a>.</li></td>
  </tr>
</tbody>
</table>

## Konfigurera kontinuerliga systemuppdateringar och kommunikation

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Marketo statusuppdateringar </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Prenumerera på Adobe Marketo Engage statusuppdateringar</a>.</li></td>
  </tr>
  <tr>
    <td>Meddelanden </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Prenumerera på administratörsmeddelanden</a> för kritiska problem som fel i smarta kampanjer och kritiska problem som hittats i CRM-synkroniseringen.</li></td>
  </tr>
</tbody>
</table>
