---
description: Felsökningsguide för Adobe IMS - Marketo Docs - Produktdokumentation
title: Felsökningsguide för Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e5c6ac7df0f8f6e7726de1ced598d390a6cf1deb
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Felsökningsguide för Adobe IMS {#adobe-ims-troubleshooting-guide}

Under IMS-användarmigreringen skapas en Adobe-användare för varje Marketo Engage-användare som migreras. Ibland skapas den inte (av olika anledningar relateras till användarens post i Active Directory eller problem med e-postadressen). När detta inträffar kommer Marketo Engage-administratören att se orsakerna i användarens migreringsstatusfält på självmigreringskonsolen. Se hur du löser olika problem med att skapa Adobe-användare nedan.

## Felmeddelanden {#error-messages}

* <a href="#not-in-directory">Finns inte i katalogen</a>
* <a href="#gmail-invalid-character">Ogiltigt Gmail-tecken</a>
* <a href="#inactive-user">Inaktiv användare</a>
* <a href="#not-in-domain">Inte i domänen</a>
* <a href="#create-failure">Skapa fel</a>
* <a href="#type2e-user-failure">Type2e-användarfel</a>

<table>
<thead>
  <tr>
    <th style="width:20%">Felmeddelande</th>
    <th style="width:40%">Rotorsak</th>
    <th style="width:40%">Lösningar</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">Finns inte i katalogen</a></i></td>
    <td>Användaren finns inte i Active Directory (AD). För alla organ med enkel inloggning som har AD-synkronisering aktiverat tillåts bara att användare skapas via identitetsleverantören (IdP). Därför kunde användaren inte läggas till via Admin Console under användarmigreringen.</td>
    <td>Migrera - användaren måste läggas till i Active Directory med rätt behörigheter. Marketo-administratör för att köra användarmigreringen för den här användaren igen från migreringskonsolen. 
    <br>Inte migrera - Marketo-administratör hoppar över användaren i migreringskonsolen. Knappen"Slutförd migrering" visas när alla användare räknas som migrering eller hoppande. Klicka på den för att slutföra användarmigreringsprocessen.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Ogiltigt Gmail-tecken</a></i></td>
    <td>Enligt Adobe säkerhetspolicy, '.' och plustecknet (+) tillåts inte i en e-postadress endast i Gmail-domänen  
    <br>Båda specialtecknen tillåts i e-postadresser som inte är Gmail-domäner. </td>
    <td>Migrera - E-postadressen måste uppdateras i Marketo Engage för att uppfylla Adobe säkerhetspolicy. Marketo-administratör för att köra användarmigreringen för den här användaren på nytt från migreringskonsolen.<br>Inte migrera - Marketo-administratör hoppar över användaren i migreringskonsolen. Knappen"Slutförd migrering" visas när alla användare räknas som migrering eller hoppande. Klicka på den för att slutföra användarmigreringsprocessen.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Inaktiv användare</a></i></td>
    <td>AD Sync är aktiverat och användarens federerade konto finns men har inaktiv/inaktiverad status.</td>
    <td>Migrera - Användarens status och korrekta behörigheter måste återställas. Marketo-administratör för att köra användarmigreringen för den här användaren igen från migreringskonsolen.
    <br>Inte migrera - Marketo-administratör hoppar över användaren i migreringskonsolen. Knappen"Slutförd migrering" visas när alla användare räknas som migrering eller hoppande. Klicka på den för att slutföra användarmigreringsprocessen.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">Inte i domänen</a></i></td>
    <td>Domänkontroll är aktiverat i Admin Console, men domänen för användarens e-postadress är inte en av de tillåtna domänerna. 
    <br>Principer för domänkontroll anges på katalognivå.</td>
    <td>Migrera - E-postadressen måste uppdateras i Marketo Engage för att vara kompatibel med domänprincipen, eller så kan systemadministratören antingen <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    flytta domänen till en annan inaktiverad katalog för domäntvingande (DE) </a> eller <a href="https://helpx.adobe.com/enterprise/using/set-up-identity.html">skapa en ny katalog</a> som inte omfattas av DE-principen. Marketo-administratör för att köra användarmigreringen för den här användaren på nytt från migreringskonsolen. <br>Inte migrera - Marketo-administratör hoppar över användaren i migreringskonsolen. Knappen"Slutförd migrering" visas när alla användare räknas som migrering eller hoppande. Klicka på den för att slutföra användarmigreringsprocessen.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Skapa fel</a></i></td>
    <td>Olika orsaker i backend-objektet.</td>
    <td>Vänligen skicka in ett supportärende.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Type2e-användarfel</a></i></td>
    <td>Olika orsaker i backend-objektet.</td>
    <td>Vänligen skicka in ett supportärende.</td>
  </tr>
</tbody>
</table>
