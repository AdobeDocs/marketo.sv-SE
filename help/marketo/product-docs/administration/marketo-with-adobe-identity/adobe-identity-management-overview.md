---
description: Adobe Identity Management Overview - Marketo Docs - produktdokumentation
title: Adobe Identity Management - översikt
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 0%

---

# Adobe Identity Management - översikt {#adobe-identity-management-overview}

Om du har ett nytt konto hos Adobe Marketo Engage (nytt konto, inte bara en ny instans för ett befintligt konto) från och med den 15 februari 2022, kan det integreras med Adobe Identity Management System, beroende på vilket produktpaket som köpts. Om du vill ta reda på om du har det kontaktar du kontoteamet (din kontoansvarige) på Adobe.

Befintliga Marketo-prenumerationer kommer att börja migreras till Adobe Identity Management System under andra halvåret 2023.

>[!NOTE]
>
>Marketo Support kommer inte att kunna tillhandahålla några uppdateringar om migrering av Adobe IMS. Adobe Account Team kommer att nå ut med den beräknade tidslinjen de närmaste månaderna.

## Profilnivåer {#profile-levels}

Adobe Marketo Engage prenumerationer på Adobe Identity Management System har stöd för olika profiler. Följande typer av användarprofiler är relevanta för den här integreringen.

<table>
 <tr>
  <td><strong>Adobe Admin Console systemadministratör</strong></td>
  <td>Ansvarig för att skapa identitetskoncept för Adobe och Marketo Engage i Adobe Admin Console. Beviljad roll vid konfigurationen av Adobe-organisationen.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console produktadministratör</strong></td>
  <td>Ansvarig för att ge användare rätt till Marketo Engage-produkten i Adobe Admin Console. Beviljad roll i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administratör för Adobe Admin Console produktprofil</strong></td>
  <td>Ansvarig för att administrera användare i en produktprofil. De kan inte hantera användare utanför den specifika profilen. En produktprofiladministratör har inte åtkomst till Marketo-programmet om den inte läggs till i produktprofilen som en användare. Deras roll är fortfarande en standardanvändare (standardarbetsyta om de har fler än en arbetsyta).
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage produktadministratör</strong></td>
  <td>En person som har beviljats tillträde till Marketo Engage med administrativ behörighet. Beviljad roll i Marketo Engage, inte i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage-användare</strong></td>
  <td>En person som har fått tillträde till Marketo Engage. Inga administrativa behörigheter.</td>
 </tr>
</table>

## Vanliga frågor {#faq}

**Vad är Adobe Identity?**

Adobe Identity Management System består av tre komponenter.

* Identitetstjänst för Adobe: Hanterar autentisering och validering av slutanvändaren, inklusive federation och enkel inloggning (SSO) vid körning.

* Adobe Admin Console: Admin Console är en central plats för hantering av Adobe-berättiganden i hela organisationen. Den hanterar användarhantering, molntjänster, tillstånd för datorlicenser, federationskonfiguration och tillhandahåller säkerhetsfunktioner för att förhindra dataförlust.

* UMAPI (Adobe User Management API): Tillåter organisationer att hantera företagsanvändare och berättiganden i Adobe Admin Console på API-nivå.

**När kommer befintliga Marketo Engage-prenumerationer att integreras med IMS?**

Befintliga Marketo-prenumerationer kommer att migreras till Adobe Identity Management System senare i år. Marketo Support kommer inte att kunna tillhandahålla några uppdateringar om migrering av Adobe IMS. Adobe Account Team kommer att nå ut med den beräknade tidslinjen de närmaste månaderna.

**Vad är skillnaden mellan en produktadministratör för Adobe och en Marketo Engage-administratör?**

* Adobe produktadministratör är en ny roll för Marketo.
* Adobe produktadministratörsroll ges till användare som lagts till som produktadministratör i Adobe Admin Console
* Adobe produktadministratör är skrivskyddad och kan inte redigeras eller tas bort från Marketo Engage.
* Adobe produktadministratör har samma rättigheter och behörigheter som en vanlig Marketo-administratör.
* Marketo Engage Admins roll är fortfarande en administratör och beviljas en användare i Marketo Engage.

**Har stödet för API-klienten för användarhantering förändrats?**

Ja. De som har anslutit sig till Adobe IMS kan inte utnyttja alla befintliga API:er för Marketo användarhantering. Adobe för åtgärder för att bjuda in, uppdatera och ta bort användare [IMS API:er](https://www.adobe.io/apis/experienceplatform/umapi-new.html) ska användas. För rollhantering gäller fortfarande Marketo API:er för användarhantering. Utöver detta finns det inga andra förändringar i klientstödet för Marketo REST API.

**Vem kontaktar vi för support om vi är integrerade med IMS?**

Du följer då standardproceduren för att kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support).

**Om jag använder en Adobe-identitet för att få åtkomst till andra Adobe-program, kan jag använda den för att få åtkomst till Marketo?**

Även om du har andra Adobe-produkter kan du inte komma åt Marketo med Adobe Identity förrän prenumerationen migreras till IMS.

**Hanteras Marketo användarroller (i arbetsytor) i Adobe Admin Console?**

Nej. Hanteringen av användarroller (i arbetsytor) slutförs i Marketo Engage.

**Jag är Marketo-administratör i en IMS-integrerad prenumeration och har inte tillgång till Admin Console. Hur får jag åtkomst?**

Alla Adobe-system eller produktadministratörer som har tillgång till din organisations Admin Console kan ge dig åtkomst. Om du är osäker på vem i organisationen som har administratörsbehörighet i konsolen kontaktar du [Adobe kundtjänst](https://helpx.adobe.com/contact.html).

**Hur lägger en administratör till användare i Marketo Sales Connect?**

Även om det kommer att finnas ett produktkort i Admin Console för Sales Connect, bör Admin Console inte användas för att lägga till/hantera användare. Med följande länk kan administratörer hantera användare via Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Var kan jag läsa mer om Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Går jag fortfarande till avsnittet Admin i Marketo och gör ändringar i användarkontot för mitt konto?**

Nej, du måste navigera till [account.adobe.com](https://account.adobe.com).

**Hur fungerar detta med Marketo Universal ID?**

De som har anslutit sig till Adobe-identiteten kan enkelt komma åt alla IMS-aktiverade prenumerationer via prenumerationsväljaren i produkten.

**Fungerar detta med enkel inloggning?**

Ja. Marketo-integrering med Adobe IMS stöder universella ID-användare och SSO. SSO styrs nu av Adobe IMS och konfigureras på organisationsnivå i Adobe Admin Console. [Läs mer här](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Hur fungerar enhetsauktorisering?**

Adobe IMS har för närvarande inte stöd för något som Marketo autentiseringsfunktion.

**Går det fortfarande att använda funktionen&quot;Inbjudan till användardialogruta&quot; för att göra användarens inloggning unik från sin e-postadress?**

Nej. Arbetsflödet för användarinbjudan är inte längre aktivt när en prenumeration är IMS-aktiverad, så funktionen är inte längre giltig. Adobe-identitet kräver att användarens identitet styrs av användarens e-postadress.

**För Adobe IMS, har vi möjlighet att använda Adobe ID, Enterprise ID eller Federated ID?**

Ja, du bestämmer vilken typ av identitet som din organisation ska stödja. Mer information finns här: [Identitetsöversikt](https://helpx.adobe.com/enterprise/using/identity.html) och här: [Ställ in identitet](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Vilka produktkort stöds i Adobe Admin Console?**

Följande produktkort stöds: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect och Marketo Sales Insight Actions.

>[!MORELIKETHIS]
>
>* [Administratörsinställningar](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Lägg till eller ta bort en produktadministratör](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Lägg till eller ta bort en användare](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

