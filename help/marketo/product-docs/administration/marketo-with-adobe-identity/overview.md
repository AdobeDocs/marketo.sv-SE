---
description: Översikt - Marketo Docs - produktdokumentation
title: Översikt
hide: true
hidefromtoc: true
source-git-commit: 306e08b08bf63fe51778dc51ccb9cb971fed2f4b
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Översikt {#overview}

Om din prenumeration på Adobe Marketo Engage gjordes den 21/10-04 kommer den att integreras med Adobe Identity Management System. Med AIMS kan användare logga in på Marketo Engage och andra Experience Cloud-program med en gemensam Adobe-identitet.

## Profilnivåer

Det finns tre profilnivåer.

<table>
 <tr>
  <td><strong>Systemadministratör</strong></td>
  <td>Ansvarig för att skapa identitetskoncept för Adobe och Marketo Engage i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Produktadministratör</strong></td>
  <td>Ansvarig för att ge användare rätt till Marketo Engage-produkten i Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Användare</strong></td>
  <td>En person som har fått tillträde till Marketo Engage. Inga administrativa behörigheter.</td>
 </tr>
</table>

## Vanliga frågor

**Vad är Adobe Identity?**

Adobe Identity Management System består av tre komponenter.

* Identitetstjänst för Adobe: Hanterar autentisering och validering av slutanvändaren, inklusive federation och enkel inloggning (SSO) vid körning.

* Adobe Admin Console: Admin Console är en central plats för hantering av Adobe-berättiganden i hela organisationen. Den hanterar användarhantering, molntjänster, tillstånd för datorlicenser, federationskonfiguration och tillhandahåller säkerhetsfunktioner för att förhindra dataförlust.

* UMAPI (Adobe User Management API): Tillåter organisationer att hantera företagsanvändare och berättiganden i Adobe Admin Console på API-nivå.

**Vad är skillnaden mellan en produktadministratör för Adobe och en Marketo Engage-administratör?**

* Adobe produktadministratör är en ny roll för Marketo.
* Det är en skrivskyddad roll som inte kan redigeras eller tas bort från Marketo.
* Den har samma rättigheter och privilegier som Marketo-administratören.

**Har stödet för API-klienter förändrats?**

Ja. De som har anslutit sig till Adobe IMS kan inte utnyttja Marketo befintliga API:er för användarhantering. De använder API:erna [IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html).

**Vem kontaktar vi för support?**

Du följer standardproceduren för att kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support).

**Hanteras Marketo användarroller (i arbetsytor) i Adobe Admin Console?**

Nej. Hantering av användarroller (i arbetsytor) har slutförts i Marketo.

**Jag är Marketo-administratör och har inte tillgång till Admin Console. Hur får jag åtkomst?**

Alla system- och produktadministratörer som har tillgång till din organisations Admin Console kan ge dig åtkomst. Om du är osäker på vem i din organisation som har administratörsbehörighet i konsolen kan du kontakta [Adobe kundtjänst](https://helpx.adobe.com/contact.html).

**Hur lägger en administratör till användare i Marketo Sales Connect?**

Det kommer att finnas ett produktkort i AC för Sales Connect, men AC bör inte användas för att lägga till/hantera användare. Med följande länk kan administratörer hantera användare via Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Var kan jag läsa mer om Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Går jag fortfarande till administratörsavsnittet i Marketo för att göra kontoändringar?**

Nej, du måste navigera till [account.adobe.com](https://account.adobe.com).

**Hur fungerar detta med Marketo Universal ID?**

De som har anslutit sig till Adobe-identiteten kan enkelt komma åt alla IMS-aktiverade prenumerationer via prenumerationsväljaren i produkten.

**Fungerar detta med enkel inloggning?**

Ja. Marketo-integrering med Adobe IMS stöder universella ID-användare och SSO. SSO styrs nu av Adobe IMS och konfigureras på organisationsnivå i Adobe Admin Console. [Läs mer här](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Hur fungerar enhetsauktorisering?**

Adobe IMS har för närvarande inte stöd för något liknande som Marketo enhetsauktoriseringsfunktion.

**Går det fortfarande att använda funktionen&quot;Inbjudan till användardialogruta&quot; för att göra inloggningen unik från vårt e-postmeddelande?**

Nej. Arbetsflödet för användarinbjudan är inte längre aktivt när en prenumeration är IMS-aktiverad, så funktionen är inte längre giltig. Adobe-identitet kräver att användarens identitet styrs av deras e-postadress.

**För Adobe IMS, har vi möjlighet att använda Adobe ID, Enterprise ID eller Federated ID?**

Ja, du bestämmer vilken typ av identitet som din organisation ska stödja. Mer information [här](https://helpx.adobe.com/enterprise/using/identity.html) och [här](https://helpx.adobe.com/enterprise/using/set-up-identity.html).
