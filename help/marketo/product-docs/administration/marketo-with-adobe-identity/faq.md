---
description: Adobe Identity Management FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 7a5440b3673c3ebbb181ee5e81ee202463291fe7
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# Vanliga frågor om Adobe Identity Management {#adobe-identity-management-faq}

**Vad är Adobe-identitet?**

Adobe Identity Management System består av tre komponenter.

* [!DNL Adobe Identity Service]: Hanterar autentisering och validering av slutanvändaren, inklusive federation och enkel inloggning (SSO) vid körning.

* Adobe Admin Console: Admin Console är en central plats för hantering av Adobe i hela organisationen. Den hanterar användarhantering, molntjänster, tillstånd för datorlicenser, federationskonfiguration och tillhandahåller säkerhetsfunktioner för att förhindra dataförlust.

* UMAPI (Adobe User Management API): Gör att organisationer kan hantera företagsanvändare och berättiganden i Adobe Admin Console på API-nivå.

**När kommer befintliga Marketo Engage-prenumerationer att integreras med IMS?**

Befintliga prenumerationer på Marketo Engage migreras för närvarande till Adobe IMS vid alla försäljningsevenemang, inklusive förnyelser, avtalsevenemang och/eller tillägg. Migreringar utanför ett försäljningsevenemang stöds nu från och med oktober 2024.

**Efter migreringen, kommer URL:er i Marketo Engage att vara desamma?**

Nej. URL:er ser annorlunda ut efter migrering.

**Behöver vi göra något för att förbereda oss för URL-ändringen?**

Ja. Efter migreringen kommer Marketo Engage att gå från experience.adobe.com till Adobe Experience Cloud. Du måste samarbeta med IT-teamet för att kunna tillåtslista alla Adobe-domäner som listas [ högst upp i den här artikeln](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} för att förhindra avbrott i åtkomsten till Marketo Engage.

Tidigare länkar och bokmärken till Marketo Engage-resurser på engage-xx.marketo.com _kommer_ att fortsätta fungera. Du måste dock först logga in på Marketo Engage-instansen för den URL som du navigerar till. Om du till exempel vill navigera till ett bokmärke för en Smart Campaign-instans med Munchkin ID 123-ABC-456 måste du först logga in på Marketo Engage-instansen med Munchkin ID 123-ABC-456.

**Vad är skillnaden mellan en produktadministratör för Adobe och en Marketo Engage-administratör?**

* Adobe produktadministratör är en ny roll för Marketo.
* Adobe produktadministratörsroll ges till användare som lagts till som produktadministratör i Adobe Admin Console
* Adobe produktadministratör är skrivskyddad och kan inte redigeras eller tas bort från Marketo Engage.
* Adobe produktadministratör har samma rättigheter och behörigheter som en vanlig Marketo-administratör.
* Marketo Engage Admins roll är fortfarande en administratör och beviljas en användare i Marketo Engage.

**Har det skett någon förändring i klientstödet för API:t för användarhantering?**

Ja. De som har anslutit sig till Adobe IMS kan inte utnyttja alla befintliga API:er för Marketo användarhantering. För åtgärder för att bjuda in, uppdatera och ta bort användare bör API:erna ](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} för Adobe [IMS användas. För rollhantering gäller fortfarande Marketo API:er för användarhantering. Utöver detta finns det inga andra förändringar i klientstödet för Marketo REST API.

**Vem kontaktar vi om vi är integrerade med IMS?**

* Migrering före användare: supportärenden för filer i [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) eller e-post `customercare@marketo.com`.

* Migrering efter användare: supportärenden för filer i [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) eller e-post `customercare@marketo.com`.

* Slutförande av migrering efter support: Produktsupportadministratörer kan arkivera ärenden via supportportalen för Experience League.

Om du har Ultimate Success har du tillgång till tjänsten Admin Console Migration White Glove. Kontakta kontoteamet (din kontoansvarige) på Adobe om du behöver hjälp.

**Om jag använder en Adobe-identitet för att få åtkomst till andra Adobe-program, kan jag använda den för att få åtkomst till Marketo?**

Även om du har andra Adobe-produkter kan du inte komma åt Marketo med Adobe Identity förrän prenumerationen migreras till IMS.

**Hanteras Marketo användarroller (i arbetsytor) i Adobe Admin Console?**

Nej. Hanteringen av användarroller (i arbetsytor) slutförs i Marketo Engage.

**Jag är Marketo-administratör i en IMS-integrerad prenumeration och har inte tillgång till Admin Console. Hur får jag åtkomst?**

Alla Adobe-system eller produktadministratörer som har tillgång till din organisations Admin Console kan ge dig åtkomst. Om du är osäker på vem i din organisation som har administratörsbehörighet i konsolen kontaktar du [Adobe kundtjänst](https://helpx.adobe.com/contact.html){target="_blank"}.

**Hur lägger en administratör till användare i Marketo [!DNL Sales Connect]?**

Även om det kommer att finnas ett produktkort i Admin Console för [!DNL Sales Connect] bör Admin Console inte användas för att lägga till/hantera användare. Med följande länk kan administratörer hantera användare via Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Var kan jag läsa mer om Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/se/enterprise/admin-guide.html){target="_blank"}.

**Går jag fortfarande till avsnittet Administratör i Marketo för att göra ändringar i användarkontot för mitt konto?**

Nej, du måste navigera till [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Hur fungerar detta med Marketo Universal ID?**

De som har anslutit sig till Adobe-identiteten kan enkelt komma åt alla IMS-aktiverade prenumerationer via prenumerationsväljaren i produkten.

**Fungerar detta med enkel inloggning?**

Ja. Marketo-integrering med Adobe IMS stöder universella ID-användare och SSO. SSO styrs nu av Adobe IMS och konfigureras på organisationsnivå i Adobe Admin Console. [Läs mer här](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Jag har redan anslutit mig till Adobe Identity och nu vill jag implementera enkel inloggning. Vad ska jag göra?**

Om du vill implementera enkel inloggning och din prenumeration har registrerats på Adobe Identity utan enkel inloggning (SSO) implementerad i Adobe Org, skickar du en biljett till [Marketo Support](https://nation.marketo.com/){target="_blank"} och anger ämnet som&quot;Marketo på Admin Console, implementera enkel inloggning&quot;.

**Hur fungerar enhetsauktorisering?**

Adobe IMS har för närvarande inte stöd för något som Marketo autentiseringsfunktion.

**Är det fortfarande möjligt att använda funktionen &quot;Logga in i dialogrutan Bjud in användare&quot; för att göra användarens inloggning unik från sin e-postadress?**

Nej. Arbetsflödet för användarinbjudan är inte längre aktivt när en prenumeration är IMS-aktiverad, så funktionen är inte längre giltig. Adobe-identitet kräver att användarens identitet styrs av användarens e-postadress.

**För Adobe IMS, har vi möjlighet att använda Adobe ID, Enterprise ID eller Federated ID?**

Ja, du bestämmer vilken typ av identitet som din organisation ska stödja. Mer information finns här: [Identitetsöversikt](https://helpx.adobe.com/enterprise/using/identity.html) och här: [Konfigurera identitet](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Vilka produktkort stöds i Adobe Admin Console?**

Följande produktkort stöds: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect och Marketo Sales Insight Actions.

**Vad händer om min användarinloggning inte matchar min e-postadress när jag migreras till en Adobe-identitet?**

Användare av Marketo Engage som har andra inloggningar än sin e-postadress loggar inte längre in med de inloggningsuppgifterna när de väl har migrerats till en Adobe-identitet. Adobe-identiteter autentiseras alltid med en användares e-postadress. Du kan uppdatera en e-postadress för en Adobe-identitet på [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Vad händer efter migreringen av Adobe-identitet om min prenumeration använder inställningar för IP-begränsning?**

När prenumerationer placeras på Adobe Identity migreras inte IP-restriktionsinställningarna till Adobe Admin Console. Marketo inställningar för IP-begränsningar innefattar att endast tillåta åtkomst från specifika IP-adresser och blockera specifika IP-adresser från åtkomst. För närvarande stöder inte Adobe Identity Management-systemet IP-begränsningsfunktioner.

I början av 2025 kommer Adobe Identity Management System att släppa en funktion som bara tillåter specifika IP-adresser, vilket stöder en övergång för Marketo-användare som för närvarande använder den här funktionen. De som för närvarande använder den här funktionen migreras inte förrän funktionen släpps. När funktionen har levererats meddelas användarna om att migreringen schemaläggs. Mer information om funktionen finns när den blir tillgänglig.

Användare som för närvarande använder IP-begränsningen, som blockerar specifika adresser från åtkomst, kommer inte längre att kunna använda den här funktionen efter att de har migrerats till Adobe Identity, eftersom den inte stöds av Adobe Identity Management System.

**Vad händer efter migrering av Adobe-identitet om jag har användare med en roll som har alternativet Åsidosätta enkel inloggning?**

När prenumerationer placeras på Adobe Identity, ställs enkel inloggning (SSO) in på organisationsnivå Adobe för alla användare. När enkel inloggning har konfigurerats kommer den att tillämpas för alla Marketo-användare/alla Marketo-instanser i den Adobe-organisationen. Tidigare hade Marketo stöd för att tillåta att en användarroll konfigureras att ha alternativet Åsidosätta enkel inloggning. Detta stöds inte av Adobe Identity Management System.

**Jag har fler än en prenumeration, men inte alla har enkel inloggning aktiverad. Vad händer efter migrering av Adobe-identitet?**

När prenumerationer placeras på Adobe Identity, ställs enkel inloggning (SSO) in på organisationsnivå i Adobe. Detta innebär att enkel inloggning gäller för alla produktinstanser i Adobe Org. När enkel inloggning har konfigurerats gäller den alla Marketo-instanser i den Adobe-organisationen. Tidigare hade Marketo stöd för den här inställningen på förekomstnivå. Detta stöds inte av Adobe Identity Management System.

**Jag måste nu navigera till Experience Cloud för att komma åt Marketo Engage. Finns det ett sätt att effektivisera det här flödet?**

Ja. Du kan skapa ett webbläsarbokmärke för länken som startas efter att du har klickat på knappen **Starta** på Marketo Engage-instansens startsida, så att du kan gå förbi den sidan.

![](assets/faq-1.png)
