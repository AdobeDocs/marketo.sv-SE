---
description: Adobe Identity Management FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 0%

---

# Vanliga frågor om Adobe Identity Management {#adobe-identity-management-faq}

**Vad är Adobe Identity?**

Adobe Identity Management System består av tre komponenter.

* [!DNL Adobe Identity Service]: Hanterar autentisering och validering av slutanvändaren, inklusive federation och enkel inloggning (SSO) vid körning.

* Adobe Admin Console: Admin Console är en central plats för hantering av Adobe i hela organisationen. Den hanterar användarhantering, molntjänster, tillstånd för datorlicenser, federationskonfiguration och tillhandahåller säkerhetsfunktioner för att förhindra dataförlust.

* UMAPI (Adobe User Management API): Gör att organisationer kan hantera företagsanvändare och berättiganden i Adobe Admin Console på API-nivå.

**När kommer befintliga Marketo Engage-prenumerationer att integreras med IMS?**

Befintliga Marketo-prenumerationer kommer att migreras till Adobe Identity Management System senare i år. Marketo Support kommer inte att kunna tillhandahålla några uppdateringar om migrering av Adobe IMS. Adobe Account Team kommer att nå ut med den beräknade tidslinjen de närmaste månaderna.

**Vad är skillnaden mellan en produktadministratör för Adobe och en Marketo Engage-administratör?**

* Adobe produktadministratör är en ny roll för Marketo.
* Adobe produktadministratörsroll ges till användare som lagts till som produktadministratör i Adobe Admin Console
* Adobe produktadministratör är skrivskyddad och kan inte redigeras eller tas bort från Marketo Engage.
* Adobe produktadministratör har samma rättigheter och behörigheter som en vanlig Marketo-administratör.
* Marketo Engage Admins roll är fortfarande en administratör och beviljas en användare i Marketo Engage.

**Har stödet för API-klienten för användarhantering förändrats?**

Ja. De som har anslutit sig till Adobe IMS kan inte utnyttja alla befintliga API:er för Marketo användarhantering. Adobe för åtgärder för att bjuda in, uppdatera och ta bort användare [IMS API:er](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} ska användas. För rollhantering gäller fortfarande Marketo API:er för användarhantering. Utöver detta finns det inga andra förändringar i klientstödet för Marketo REST API.

**Vem kontaktar vi för support om vi är integrerade med IMS?**

Du följer då standardproceduren för att kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Om jag använder en Adobe-identitet för att få åtkomst till andra Adobe-program, kan jag använda den för att få åtkomst till Marketo?**

Även om du har andra Adobe-produkter kan du inte komma åt Marketo med Adobe Identity förrän prenumerationen migreras till IMS.

**Hanteras Marketo användarroller (i arbetsytor) i Adobe Admin Console?**

Nej. Hanteringen av användarroller (i arbetsytor) slutförs i Marketo Engage.

**Jag är Marketo-administratör i en IMS-integrerad prenumeration och har inte tillgång till Admin Console. Hur får jag åtkomst?**

Alla Adobe-system eller produktadministratörer som har tillgång till din organisations Admin Console kan ge dig åtkomst. Om du är osäker på vem i organisationen som har administratörsbehörighet i konsolen kontaktar du [Adobe kundtjänst](https://helpx.adobe.com/contact.html){target="_blank"}.

**Hur lägger en administratör till användare i Marketo? [!DNL Sales Connect]?**

Medan det kommer att finnas ett produktkort i Admin Console för [!DNL Sales Connect]ska Admin Console inte användas för att lägga till/hantera användare. Med följande länk kan administratörer hantera användare via Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Var kan jag läsa mer om Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

**Går jag fortfarande till avsnittet Admin i Marketo och gör ändringar i användarkontot för mitt konto?**

Nej, du måste navigera till [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Hur fungerar detta med Marketo Universal ID?**

De som har anslutit sig till Adobe-identiteten kan enkelt komma åt alla IMS-aktiverade prenumerationer via prenumerationsväljaren i produkten.

**Fungerar detta med enkel inloggning?**

Ja. Marketo-integrering med Adobe IMS stöder universella ID-användare och SSO. SSO styrs nu av Adobe IMS och konfigureras på organisationsnivå i Adobe Admin Console. [Läs mer här](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

* **Jag har redan anslutit mig till Adobe Identity och nu vill jag implementera enkel inloggning. Vad ska jag göra?**

Om du vill implementera enkel inloggning och din prenumeration har registrerats på Adobe Identity utan enkel inloggning (SSO) implementerad i Adobe Org skickar du en biljett till [Marketo Support](https://nation.marketo.com/){target="_blank"} och ange ämnet som&quot;Marketo on Admin Console, implementera enkel inloggning&quot;.

**Hur fungerar enhetsauktorisering?**

Adobe IMS har för närvarande inte stöd för något som Marketo autentiseringsfunktion.

**Går det fortfarande att använda funktionen&quot;Inbjudan till användardialogruta&quot; för att göra användarens inloggning unik från e-postmeddelandet?**

Nej. Arbetsflödet för användarinbjudan är inte längre aktivt när en prenumeration är IMS-aktiverad, så funktionen är inte längre giltig. Adobe-identitet kräver att användarens identitet styrs av användarens e-postadress.

**För Adobe IMS, har vi möjlighet att använda Adobe ID, Enterprise ID eller Federated ID?**

Ja, du bestämmer vilken typ av identitet som din organisation ska stödja. Mer information finns här: [Identitetsöversikt](https://helpx.adobe.com/enterprise/using/identity.html) och här: [Ställ in identitet](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Vilka produktkort stöds i Adobe Admin Console?**

Följande produktkort stöds: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect och Marketo Sales Insight Actions.

**Vad händer om min användarinloggning inte matchar min e-postadress när jag migreras till en Adobe-identitet?**

Nuvarande Marketo-användare med andra inloggningar än sin e-postadress kommer inte längre att logga in med dessa inloggningsuppgifter när de har migrerats till en Adobe-identitet. Adobe-identiteter autentiseras alltid med en användares e-postadress.

**Vad händer efter migreringen av Adobe-identitet om min prenumeration använder inställningar för IP-begränsning?**

När prenumerationer placeras på Adobe Identity migreras inte IP-restriktionsinställningarna till Adobe Admin Console. Marketo inställningar för IP-begränsningar innefattar att endast tillåta åtkomst från specifika IP-adresser och blockera specifika IP-adresser från åtkomst. För närvarande stöder inte Adobe Identity Management-systemet IP-begränsningsfunktioner.

Från och med 2024 kommer Adobe Identity Management System att släppa en funktion som bara tillåter specifika IP-adresser, vilket stöder en övergång för Marketo-användare som för närvarande använder den här funktionen. De som för närvarande använder den här funktionen migreras inte förrän funktionen släpps. När funktionen har levererats meddelas användarna om att migreringen schemaläggs. Mer information om funktionen finns när den blir tillgänglig.

Användare som för närvarande använder IP-begränsningen, som blockerar specifika adresser från åtkomst, kommer inte längre att kunna använda den här funktionen efter att de har migrerats till Adobe Identity, eftersom den inte stöds av Adobe Identity Management System.

**Vad händer efter migrering av Adobe-identitet om jag har användare med en roll som har alternativet Åsidosätta enkel inloggning?**

När prenumerationer placeras på Adobe Identity, ställs enkel inloggning (SSO) in på organisationsnivå Adobe för alla användare. När enkel inloggning har konfigurerats kommer den att tillämpas för alla Marketo-användare/alla Marketo-instanser i den Adobe-organisationen. Tidigare hade Marketo stöd för att tillåta att en användarroll konfigureras att ha alternativet Åsidosätta enkel inloggning. Detta stöds inte av Adobe Identity Management System.

**Jag har mer än en prenumeration, men inte alla har enkel inloggning aktiverad. Vad händer efter migrering av Adobe Identity?**

När prenumerationer placeras på Adobe Identity, ställs enkel inloggning (SSO) in på organisationsnivå i Adobe. Detta innebär att enkel inloggning gäller för alla produktinstanser i Adobe Org. När enkel inloggning har konfigurerats gäller den alla Marketo-instanser i den Adobe-organisationen. Tidigare hade Marketo stöd för den här inställningen på förekomstnivå. Detta stöds inte av Adobe Identity Management System.
