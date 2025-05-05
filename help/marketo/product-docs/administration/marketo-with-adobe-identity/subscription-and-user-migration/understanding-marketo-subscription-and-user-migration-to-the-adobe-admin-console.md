---
description: Understanding Marketo Subscription and User Migration to the Adobe Admin Console - Marketo Docs - Product Documentation
title: Förstå Marketo prenumeration och användarmigrering till Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: d6cf2b994f56a0fa4f2118fb3da3fd874644d8ae
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# Förstå Marketo prenumeration och användarmigrering till Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe förbättrar hur du hanterar dina Adobe Marketo Engage-prenumerationer och -användare och ökar produktiviteten för dig och din organisation. Som en del av denna förändring migrerar Adobe dina Marketo Engage-prenumerationer och -användare till Adobe Admin Console. Detta är en nödvändig migrering och påverkar inte något marknadsföringsarbetsflöde, innehåll, integreringar eller resurser.

>[!TIP]
>
>Lär dig hur du kan använda Adobe Admin Console för att hantera dina Adobe-berättiganden i hela organisationen med [Enterprise and Teams Admin Guide](https://helpx.adobe.com/se/enterprise/admin-guide.html){target="_blank"}.

## Vad är Changing? {#what-is-changing}

Som en del av migreringen kommer din prenumeration och användarhantering att gå över från Marketo till Adobe Admin Console.

* **Systemadministratörer hanterar prenumerationer på Adobe Admin Console**. Se alla dina Adobe-produkter i en och samma konsol.

* **Produktadministratörer hanterar användare och deras åtkomst på Adobe Admin Console**. Lägg till och ta bort användare för alla Adobe-prenumerationer. Adobe Admin Console stöder inte användarbaserad förfallotid för åtkomst. Användare som har Marketo Engage-åtkomst som är schemalagd att upphöra efter migreringen kommer fortfarande att migreras och beviljas åtkomst som inte upphör att gälla. Efter migreringen måste de tas bort manuellt (eller före) det önskade förfallodatumet.

* **Användare loggar in med Adobe Identity**. Adobe migrerar befintliga användare till Adobe Admin Console. Användare loggar in på sina Marketo-prenumerationer med sin nya Adobe Identity - antingen en Adobe ID eller Adobe Federated ID (SSO).

* **URL:er ser annorlunda ut efter migrering**. Efter migreringen kommer Marketo Engage att gå från experience.adobe.com till Adobe Experience Cloud. Du måste samarbeta med IT-teamet för att tillåtslista alla Adobe-domäner som listas [ överst i den här artikeln](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} för att förhindra avbrott i åtkomsten till Marketo Engage.

ID-numren för dina resurser ändras inte. Och tidigare länkar och bokmärken till Marketo Engage-resurser på engage-xx.marketo.com _kommer_ att fortsätta fungera. Du måste dock först logga in på Marketo Engage-instansen för den URL som du navigerar till. Om du till exempel vill navigera till ett bokmärke för en Smart Campaign-instans med Munchkin ID 123-ABC-456 måste du först logga in på Marketo Engage-instansen med Munchkin ID 123-ABC-456.

## Vad ändras inte? {#what-is-not-changing}

* **Det finns ingen förändring i hur du hanterar alla andra funktioner** i själva Marketo Engage-programmet, inklusive hantering av funktioner, användarroller, arbetsytor, funktioner och beteende.

## Tidslinje för migreringsresa {#migration-journey-timeline}

Adobe migrerar dina Marketo Engage-prenumerationer till Adobe Admin Console först och migrerar sedan alla befintliga användare med verifierade e-postadresser. Om du är systemadministratör eller Marketo produktadministratör får du e-postmeddelanden som vägleder dig genom migreringsresan. Här är en tidslinje för vad du kan förvänta dig:

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Prenumerationsmigreringen är klar {#subscription-migration-complete}

Systemadministratörer får ett e-postmeddelande när prenumerationsmigreringen till Adobe Admin Console är klar.

Systemadministratörer kan behöva utföra några nödvändiga steg innan användarmigreringen börjar för att minimera påverkan för Marketo-användare:

* Om dina Marketo-användare loggar in med enkel inloggning måste du konfigurera enkel inloggning på Adobe Admin Console så att dina användare kan fortsätta att logga in med enkel inloggning. Om dina Marketo-användare för närvarande inte använder enkel inloggning, men du vill konfigurera den på Adobe Admin Console, kan du göra det nu under migreringsresan.

* Om du redan hanterar andra Adobe-produkter i din Adobe Admin Console kan Adobe begära ditt samtycke för att automatiskt migrera användare till din befintliga konsol. Klicka på knappen &quot;Kom igång&quot; i e-postmeddelandet för att navigera till godkännandesidan.

Användarhanteringen förändras inte just nu. Även om Marketo-produkter visas i Admin Console fortsätter Marketo-administratörer att hantera användare i Marketo Admin-området, och användare fortsätter att logga in med sin Marketo Identity tills deras användarmigrering är klar. Under denna tid kan Marketo-produkter inte administreras i Admin Console förrän migreringen av användare påbörjas. Detta inkluderar den Dynamic Chat-instans som är kopplad till prenumerationen.

>[!NOTE]
>
>Om du för närvarande inte använder enkel inloggning, men funderar på att implementera den, rekommenderar vi att du gör det innan användarmigrering sker. Om du vill implementera enkel inloggning och din prenumeration har registrerats på Adobe Identity utan enkel inloggning (SSO) implementerat i Adobe Org skickar du en biljett till [Marketo Support](https://nation.marketo.com/){target="_blank"} och anger ämnet som&quot;Marketo on Admin Console, implement SSO&quot;.

### Schemalägg användarmigrering {#schedule-user-migration}

När systemadministratören har slutfört de krav som beskrivs i föregående avsnitt schemalägger Adobe automatiskt din användarmigrering 30 dagar framåt och kommunicerar med Marketo produktadministratörer för att hantera användarmigreringen.

Marketo produktadministratörer kan:

* Få ett e-postmeddelande med startdatum för den schemalagda användarmigreringen 30 dagar framåt.

* Få tillgång till Marketo migreringskonsol, som finns i Marketo Admin, där de kan ändra ett prenumerations migreringsdatum.

>[!NOTE]
>
>På grund av migreringens komplexitet begränsas datumändringar till högst 30 dagar efter det schemalagda datumet. Skicka ett e-postmeddelande till `marketocares@marketo.com` om du behöver ett senare datum.

* Se en banderoll i Min Marketo som visar en nedräkning till startdatumet för användarmigreringen.

* Få en påminnelse via e-post dagen före startdatumet för användarmigreringen.

### Förbered användare för migreringsdagen {#prepare-users-for-migration-day}

Som Marketo produktadministratör bör du se till att alla användare är förberedda för migreringsdagen.

* Kontrollera [e-postverifieringsstatus](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} för alla användare i Marketo Admin. Uppmuntra användare som inte har verifierat sin e-postadress att göra det, och hjälpa användare att lösa eventuella problem när de slutför verifieringsprocessen.

* Sök i din e-postinkorg efter&quot;utelåsta&quot; användarmeddelanden. Be användare som har låsts ut att återställa sitt lösenord att återupprätta åtkomst till Marketo Engage före migreringsdagen.

* Förbered alla användare för den kommande migreringen till Adobe Identity.

>[!IMPORTANT]
>
>Om en Marketo Engage-användare inte verifierar sin e-postadress eller är utlåst när användaren migreras, migreras de inte till en Adobe ID och förlorar åtkomsten till Marketo-prenumerationen när migreringen av prenumerationen är klar. För att återfå åtkomst måste en Marketo-produktadministratör lägga till dem som en ny användare.

### Vad man kan förvänta sig på migreringsdagen {#what-to-expect-on-migration-day}

Alla Marketo-prenumerationer med en tidszon i USA migreras från och med midnatt, Pacific Standard Time, från migreringens startdatum. Migreringen av användare för alla andra prenumerationer börjar vid midnatt i prenumerationens angivna tidszon.

**Adobe migrerar automatiskt Marketo-administratörer först**. När Marketo-administratörer migreras till Adobe Identity tilldelas de Adobe produktadministratörsroll i Marketo-programmet tillsammans med andra roller de tidigare haft.

**Om din Marketo-prenumeration har färre än 75 användare och inte har enkel inloggning i Marketo och/eller din Adobe-organisation** migrerar Adobe automatiskt resten av dina användare. Det här arbetsflödet ger den högsta nivån av automatisering för att minimera overheadkostnader för användare av Adobe Marketo. Du behöver inte göra något för att utföra migreringen.

**Om din Marketo-prenumeration har över 75 användare eller har enkel inloggning i Marketo och/eller din Adobe-organisation** får Marketo produktadministratörer tillgång till självbetjäningsmigreringsområdet för Marketo migreringskonsol, som finns i Marketo Admin Area. För dem som behöver större kontroll under användarmigreringsprocessen kan Marketo produktadministratörer börja välja användare att migrera gruppvis eller alla samtidigt. När användarna har valts kan administratörerna välja att migrera nu eller Schemalägg migrering för ett senare datum, vilket ger administratörerna fullständig flexibilitet och kontroll över vilka användare som migreras när de gör det.

>[!NOTE]
>
>Åtkomsten till produkten kommer inte att gå förlorad under migreringen av användaren. Om en användare är inloggad när användaren migreras, loggas användaren ut och uppmanas att logga in igen inom några minuter med Adobe Identity när migreringen är klar. Användaren måste acceptera inbjudan genom att klicka på länken i det tillståndsmeddelande som skickas när migreringen är klar.

När användare migreras får de ett e-postmeddelande från Adobe som informerar dem om ändringen av det sätt på vilket de loggar in på Marketo. Användare **måste** acceptera en inbjudan om att logga in med Adobe Identity för första gången, antingen genom att logga in med en befintlig Adobe ID eller genom att konfigurera en ny Adobe ID med samma e-postadress.

Mer information finns i [Migrering till Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Användarinloggning med Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} och [Adobe Identity Management - frågor och svar](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Användarmigreringen är klar {#user-migration-complete}

Adobe meddelar alla systemadministratörer och produktadministratörer via e-post när alla administratörer och användare har migrerats. Alla Marketo-användare för den prenumerationen loggar nu in på Marketo med Adobe Identity och produktadministratörer hanterar endast användare på Adobe Admin Console.

## Få support {#get-support}

Om du vill ha ytterligare support för din prenumeration eller din användarmigrering kan du skicka ett e-postmeddelande till `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migrerar till Adobe Identity Overview](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Användarinloggning med Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Adobe Identity Management - frågor och svar](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Migrerar till Adobe Identity Management-självstudiekurs](https://experienceleague.adobe.com/sv/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
