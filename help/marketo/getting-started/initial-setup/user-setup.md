---
description: Innan du kommer till den nya instansen av Marketo Engage måste du slutföra några grundläggande steg för att kunna använda produkten. Dessa steg omfattar konfiguration av användarkonton, konfiguration av supportadministratörer och prenumeration på pågående systemuppdateringar.
title: Checklista för användarinställningar
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Checklista för användarinställningar {#user-setup-checklist}

Nu när du är klar med alla [inledande installationssteg](/help/marketo/getting-started/initial-setup/setup-steps.md)är det dags att lägga till några grundläggande element för att säkerställa smidig kontinuerlig användning. Detta kommer att lägga grunden för din resa med Marketo Engage och hjälpa dig att få ut det mesta av dess funktioner. Kom så börjar vi!

>[!NOTE]
>
>Du kan även hämta den här checklistan, [tillsammans med en lista över bästa praxis](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) för den nya instansen och se hur du gör.

## Marketo Engage på Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Dina nya prenumerationer på Marketo Engage har gått med på [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Gå vidare till följande granskning av användarhantering i Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och produktadministratör för Marketo Engage</td>
    <td><li>Bekräfta att du har tilldelats en produktadministratörsroll för Adobe av systemadministratören för Adobe Org.</li>  
    <ul>
    <li>Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe kundtjänst</a> för att ta reda på vem i organisationen som har <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console systemadministratör</a> behörighet.</li></ul>
    <li>Acceptera inbjudan till produktadministratör för Marketo Engage för att aktivera din Adobe ID. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">välkomstmeddelande</a> skickas när rollen tilldelas i Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler</td>
    <td><li>Tilldela alla önskade användare till Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Produktprofil</a> i Adobe Admin Console.</li>
    <ul>
    <li>Du kan inte tilldela användarroller i Marketo Engage &gt; Admin &gt; Användare och roller innan du lägger till dem i en produktprofil.</li>
    <li>Varje prenumeration blir en fristående produktprofil. Om en oönskad användare läggs till i flera produktprofiler (t.ex. produktions- och testsandlådan) måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td><li>Skapa en profil för när <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">skapa en användare</a>.</li> <li>Skapa en profil för när användare ska tas bort.</li>
    <li>Bestäm vem som ska ha <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe systemadministratörsbehörighet och Marketo Engage produktadministratörsbehörighet.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Lägg till användare</a> till önskad produktprofil.</li>
    <li>Skapa en API-användare för varje API-användningsfall.</li></td>
  </tr>
  <tr>
    <td>API för användarhantering (om tillämpligt)</td>
    <td><li>Använd <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe API för användarhantering</a> om du vill bjuda in, uppdatera och ta bort användare.</li>
    <li>Använd <a href="https://developer.adobe.com/umapi/">Adobe API för användarhantering</a> för att lägga till eller ta bort roller (t.ex. administratörer, supportadministratörer och utvecklare).</li>
    </td>
  </tr>
  <tr>
    <td>Produktsupportadministratör</td>
    <td><li>Till <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">skicka en supportanmälan i Adobe Admin Console</a>måste du ha rollen 'Product Support Administrator' tilldelad av en systemadministratör till de prenumerationer du hanterar. Endast en systemadministratör i din organisation kan <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">tilldela dig till den här rollen</a>.</li>
    <li>Du kan ha fått ett e-postmeddelande från systemadministratören om att du är supportadministratör för din Marketo Engage-prenumeration. I så fall klickar du på <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">Kom igång</a> i e-postmeddelandet för att gå med i organisationen.</li>
    <li>Bestäm lämpliga kontakter (med minst en kontaktperson för säkerhetskopiering) och låt systemadministratören tilldela rollen produktsupportadministratör på lämpligt sätt.</li></td>
  </tr>
</tbody>
</table>

## Installationsprogram för Dynamic Chat i Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Används [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), den inbyggda konversationskanalen i Marketo Engage, fortsätter du med användarbehörighetsinställningarna enligt stegen nedan i [Adobe Admin Console](https://adminconsole.adobe.com/).

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och produktadministratör för Dynamic Chat (om tillämpligt)</td>
    <td><li>Bekräfta att du har tilldelats en produktadministratörsroll för Adobe av systemadministratören för Adobe Org. Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe kundtjänst</a> för att ta reda på vem i organisationen som har administratörsbehörighet i konsolen.</li>
    <li>Acceptera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Produktadministratör för Dynamic Chat</a> inbjudan. The <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">välkomstmeddelande</a> skickas när Dynamic Chat är aktiverat i din Marketo Engage-instans och du har utsetts till systemadministratör.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler</td>
    <td><li>Tilldela alla användare till Dynamic Chat produktprofil i Adobe Admin Console.</li> 
    <ul>
    <li>Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Dynamic Chat.</li>
    <li>Du kan <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">redigera produktprofiler i Dynamic Chat</a> och skapa en egen profil med en anpassad uppsättning <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">behörigheter som är tillgängliga i din prenumeration</a>.</li></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td><li>Skapa en profil för när en chattanvändare ska läggas till och tas bort.</li>
    <li>Skapa en profil för vem som ska ha <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat produktadministratörsbehörigheter.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Lägg till användare i önskad produktprofil</a>.</li></td>
  </tr>
</tbody>
</table>

## Konfigurera pågående systemuppdateringar och kommunikation {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Marketo statusuppdateringar</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Prenumerera på Adobe Marketo Engage statusuppdateringar</a>.</li></td>
  </tr>
  <tr>
    <td>Meddelanden</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Prenumerera på administratörsmeddelanden</a> för kritiska problem som fel i smarta kampanjer och kritiska problem som hittats i CRM-synkroniseringen.</li></td>
  </tr>
</tbody>
</table>

<p>

Nu när ditt Marketo Engage-konto är klart kan du gå igenom vår [Bästa praxis för en ny Marketo Engage-instans](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md) för att få ut så mycket som möjligt av er investering och göra er redo för långsiktiga framgångar.
