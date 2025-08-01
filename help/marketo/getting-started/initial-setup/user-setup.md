---
description: Innan du dyker in i din nya instans Marketo Engage måste du slutföra några grundläggande steg för kontinuerlig användning. Dessa steg omfattar konfiguration av användarkonton, konfiguration av supportadministratörer och prenumeration av pågående systemuppdateringar.
short-description: När du är klar med de första konfigurationsstegen får du lära dig hur du skapar grundläggande element för att säkerställa smidig kontinuerlig användning.
title: Checklista för användarinställningar
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 6%

---

# Checklista för användarinställningar {#user-setup-checklist}

Nu när du har slutfört alla [inledande konfigurationssteg](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"} är det dags att skapa några grundläggande element för att säkerställa smidig kontinuerlig användning. Detta kommer att lägga grunden för din resa med Marketo Engage och hjälpa dig att få ut det mesta av dess funktioner. Kom så börjar vi!

>[!NOTE]
>
>Du kan även hämta den här checklistan, [tillsammans med en lista över bästa praxis](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) för din nya instans, och du kan avmarkera stegen medan du arbetar.

## Marketo Engage på Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Dina nya Marketo Engage-prenumerationer är registrerade på [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=sv-SE). Gå vidare till följande granskning av användarhantering i Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och Marketo Engage produktadministratör</td>
    <td><li>Bekräfta att du har tilldelats en Adobe-produktadministratörsroll av Adobe Org System Admin.</li>
    <ul>
    <li>Kontakta Adobe Account Team (din kontohanterare) eller skicka ett e-postmeddelande till <code>marketocares@marketo.com</code> för att ta reda på vem i din organisation som har behörighet för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=sv-SE">Adobe Admin Console System Admin</a>.</li></ul>
    <li>Acceptera inbjudan till Marketo Engage Product Admin för att aktivera din Adobe ID. <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=sv-SE#create-a-product-profile">Välkomstmeddelandet</a> skickas när rollen tilldelas i Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler</td>
    <td><li>Tilldela alla önskade användare till Marketo Engage <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">produktprofil</a> i Adobe Admin Console.</li>
    <ul>
    <li>Du kan inte tilldela användarroller i Marketo Engage &gt; Admin &gt; Användare och roller innan du lägger till dem i en produktprofil.</li>
    <li>Varje prenumeration blir en fristående produktprofil. Om en oönskad användare läggs till i flera produktprofiler (t.ex. produktions- och testsandlådan) måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td><li>Skapa en profil för när du ska <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html?lang=sv-SE">skapa en användare</a>.</li> <li>Skapa en profil för när användare ska tas bort.</li>
    <p><img src="assets/note-icon.png" alt="anteckningsikon"> Obs! Du måste vara systemadministratör för att kunna ta bort användare.
    <li>Bestäm vem som ska ha behörighet för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=sv-SE">Adobe systemadministratör och Marketo Engage produktadministratör.</a> <li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Lägg till användare</a> i önskad produktprofil.</li>
    <li>Skapa en API-användare för varje API-användningsfall.</li></td>
  </tr>
  <tr>
    <td>API för användarhantering (om tillämpligt)</td>
    <td><li>Använd <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe API för användarhantering</a> för att bjuda in, uppdatera och ta bort användare.</li>
    <li>Använd <a href="https://developer.adobe.com/umapi/">Adobe API för användarhantering</a> för att lägga till eller ta bort roller (t.ex. administratörer, supportadministratörer och utvecklare).</li>
    </td>
  </tr>
  <tr>
    <td>Produktsupportadministratör</td>
    <td><li>Om du vill <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=sv-SE#create-a-support-ticket-with-admin-console">skicka en supportanmälan i Adobe Admin Console</a> måste du ha rollen Produktsupportadministratör tilldelad av en systemadministratör till de prenumerationer du hanterar. Endast en systemadministratör i din organisation kan <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=sv-SE#assign-the-support-admin-role">tilldela dig till den här rollen</a>.</li>
    <li>Du kan ha fått ett e-postmeddelande från systemadministratören om att du är supportadministratör för din Marketo Engage-prenumeration. I så fall klickar du på <a href="https://experienceleague.adobe.com/sv/docs/customer-one/using/home#assign-the-support-admin-role">'Kom igång'</a> i e-postmeddelandet för att gå med i organisationen.</li>
    <li>Bestäm lämpliga kontakter (med minst en kontaktperson för säkerhetskopiering) och låt systemadministratören tilldela rollen produktsupportadministratör på lämpligt sätt.</li></td>
  </tr>
</tbody>
</table>

## Installation av Dynamic Chat i Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Om du vill använda [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=sv-SE), den inbyggda konversationskanalen i Marketo Engage, fortsätter du med användarbehörighetsinställningarna enligt stegen nedan i [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Område</th>
    <th style="width:80%">Åtgärdsobjekt</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Prenumeration och Dynamic Chat produktadministratör (om tillämpligt)</td>
    <td><li>Bekräfta att du har tilldelats en Adobe-produktadministratörsroll av Adobe Org System Admin.</li>
    <ul><li>Kontakta Adobe Account Team (din kontohanterare) eller skicka ett e-postmeddelande till <code>marketocares@marketo.com</code> för att ta reda på vem i din organisation som har behörighet för <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=sv-SE">Adobe Admin Console System Admin</a>.</li></ul>
    <li>Acceptera inbjudan till <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=sv-SE">'Dynamic Chat produktadministratör'</a>. <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=sv-SE">Välkomstmeddelandet</a> skickas när Dynamic Chat är aktiverat i din Marketo Engage-instans och du är utsedd som systemadministratör.</li></td>
  </tr>
  <tr>
    <td>Produktprofiler</td>
    <td><li>Tilldela alla användare till Dynamic Chats produktprofil i Adobe Admin Console.</li>
    <ul>
    <li>Om en oönskad användare läggs till i flera produktprofiler måste du ta bort användaren från alla produktprofiler. Annars har de fortfarande tillgång till Dynamic Chat.</li>
    <li>Du kan <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">redigera produktprofiler i Dynamic Chat</a> och skapa en anpassad profil med en anpassad uppsättning <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">behörigheter som är tillgängliga i din prenumeration</a>.</li></td>
  </tr>
  <tr>
    <td>Användare</td>
    <td><li>Skapa en profil för när en chattanvändare ska läggas till och tas bort.</li>
    <li>Skapa en profil för vem som ska ha <a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat produktadministratörsbehörighet.</a></li>
    <li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Lägg till användare i önskad produktprofil</a>.</li></td>
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
    <td><li><a href="https://experienceleague.adobe.com/sv/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Prenumerera på administratörsmeddelanden</a> om du har allvarliga problem, till exempel fel i smarta kampanjer och kritiska problem med CRM-synkroniseringen.</li></td>
  </tr>
</tbody>
</table>

<p>

Nu när ditt Marketo Engage-konto är klart kan du gå igenom [Best Practices för en ny Marketo Engage-instans](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} för att få ut så mycket som möjligt av din investering och göra inställningar för att lyckas på lång sikt.
