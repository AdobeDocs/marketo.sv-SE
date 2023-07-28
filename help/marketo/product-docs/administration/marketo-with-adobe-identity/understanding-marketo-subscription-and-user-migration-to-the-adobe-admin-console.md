---
description: Understanding Marketo Subscription and User Migration to the Adobe Admin Console - Marketo Docs - Product Documentation
title: Förstå Marketo prenumeration och användarmigrering till Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 830b8d3fa4ca49834523eb4d5119a9bb9161e04d
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---

# Förstå Marketo prenumeration och användarmigrering till Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe förbättrar hur du hanterar dina Adobe Marketo Engage-prenumerationer och -användare och ökar produktiviteten för dig och din organisation. Som en del av den här förändringen migrerar Adobe dina Marketo Engage-prenumerationer och användare till Adobe Admin Console. Detta är en nödvändig migrering och påverkar inte något marknadsföringsarbetsflöde, innehåll, integreringar eller resurser.

Läs om hur du kan använda Adobe Admin Console för att hantera dina Adobe i hela organisationen med [Administratörshandbok för Enterprise och Teams](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

## Vad är Changing? {#what-is-changing}

Som en del av migreringen kommer din prenumeration och användarhantering att gå över från Marketo till Adobe Admin Console.

* **Systemadministratörer hanterar prenumerationer på Adobe Admin Console**. Se alla Adobe-produkter i en och samma konsol.

* **Produktadministratörer hanterar användare och deras åtkomst på Adobe Admin Console**. Lägg till och ta bort användare för alla Adobe-prenumerationer.

* **Användare loggar in med Adobe-identitet**. Adobe migrerar befintliga användare till Adobe Admin Console. Användare loggar in på sina Marketo-prenumerationer med sin nya Adobe Identity - antingen Adobe ID eller Adobe Federated ID (SSO).

* **Det finns ingen förändring i hur du hanterar alla andra funktioner** i själva Marketo Engage-programmet, inklusive hantering av funktioner, användarroller, arbetsytor, funktionalitet och beteende.


## Tidslinje för migreringsresa {#migration-journey-timeline}

Adobe migrerar dina Marketo Engage-prenumerationer till Adobe Admin Console först och migrerar sedan alla befintliga användare med verifierade e-postadresser. Om du är systemadministratör eller Marketo produktadministratör får du e-postmeddelanden som vägleder dig genom migreringsresan. Här är en tidslinje för vad du kan förvänta dig:

### Prenumerationsmigreringen är klar {#subscription-migration-complete}

Systemadministratörer får ett e-postmeddelande när prenumerationsmigreringen till Adobe Admin Console är klar.

Systemadministratörer kan behöva utföra några nödvändiga steg innan användarmigreringen börjar för att minimera påverkan för Marketo-användare:

* Om dina Marketo-användare loggar in med enkel inloggning måste du konfigurera enkel inloggning på Adobe Admin Console så att dina användare kan fortsätta att logga in med enkel inloggning. Om dina Marketo-användare för närvarande inte använder enkel inloggning, men du vill konfigurera den på Adobe Admin Console, kan du göra det nu under migreringsresan.

* Om du redan hanterar andra Adobe-produkter i din Adobe Admin Console kan Adobe begära ditt samtycke för att automatiskt migrera användare till din befintliga konsol. Klicka på knappen &quot;Kom igång&quot; i e-postmeddelandet för att navigera till godkännandesidan.

Användarhanteringen förändras inte just nu. Marketo-administratörer fortsätter att hantera användare i Marketo Admin, och användare fortsätter att logga in med sin Marketo Identity tills deras användarmigrering är klar.

### Schemalägg användarmigrering {#schedule-user-migration}

När systemadministratören har slutfört de krav som beskrivs i föregående avsnitt schemalägger Adobe automatiskt din användarmigrering 30 dagar framåt och kommunicerar med Marketo produktadministratörer för att hantera användarmigreringen.

Marketo produktadministratörer kan:

* Få ett e-postmeddelande med startdatum för den schemalagda användarmigreringen 30 dagar framåt.

* Få tillgång till Marketo migreringskonsol, som finns i Marketo Admin, där de kan ändra ett prenumerations migreringsdatum.

>[!NOTE]
>
>På grund av migreringens komplexitet begränsas datumändringar till högst 30 dagar efter det schemalagda datumet. Skicka ett e-postmeddelande till marketocares@adobe.com om du behöver ett senare datum.

* Se en banderoll i Min Marketo som visar en nedräkning till startdatumet för användarmigreringen.

* Få en påminnelse via e-post dagen före startdatumet för användarmigreringen.

### Förbered användare för migreringsdagen {#prepare-users-for-migration-day}

Som Marketo produktadministratör bör du se till att alla användare är förberedda för migreringsdagen.

* Kontrollera e-postverifieringsstatus för alla användare i området Marketo Admin. Uppmuntra användare som inte har verifierat sin e-postadress att göra det, och hjälpa användare att lösa eventuella problem när de slutför verifieringsprocessen

* Förbered alla användare för den kommande migreringen till Adobe Identity.

>[!NOTE]
>
>När användare migrerar får de ett e-postmeddelande från Adobe som meddelar dem om förändringen i det sätt de loggar in på Marketo. Användare kommer att uppmanas att acceptera en inbjudan att logga in med Adobe Identity för första gången, antingen genom att logga in med en befintlig Adobe ID eller genom att konfigurera en ny med samma e-postadress.

### Vad man kan förvänta sig på migreringsdagen {#what-to-expect-on-migration-day}

Användarmigreringen startar vid midnatt i den tidszon som anges i Marketo-prenumerationen.

**Adobe migrerar automatiskt Marketo Admins först**. När Marketo-administratörer migreras till Adobe Identity får de rollen som produktadministratör för Adobe i Marketo-programmet tillsammans med eventuella andra roller de tidigare hade.

**Om din Marketo-prenumeration har färre än 75 användare** migrerar Adobe automatiskt resten av dina användare. Det här arbetsflödet ger den högsta nivån av automatisering för att minimera overheadkostnader för användare av Adobe Marketo. Du behöver inte göra något för att utföra migreringen.

**Om din Marketo-prenumeration har över 75 användare** får Marketo produktadministratörer tillgång till självbetjäningsmigreringsområdet på Marketo migreringskonsol, som finns i Marketo Admin. För dem som behöver större kontroll under användarmigreringsprocessen kan Marketo produktadministratörer börja välja användare att migrera gruppvis eller alla samtidigt. När användarna har valts kan administratörerna välja att migrera nu eller Schemalägg migrering för ett senare datum, vilket ger administratörerna fullständig flexibilitet och kontroll över vilka användare som migreras när de gör det.

>[!NOTE]
>
>Åtkomsten till produkten kommer inte att gå förlorad under migreringen av användaren. Om en användare är inloggad under den tid användaren migreras, loggas användaren ut och uppmanas att logga in igen inom några minuter med hjälp av Adobe-identitet när migreringen är klar.

När användare migreras får de ett e-postmeddelande från Adobe som meddelar dem om ändringen av det sätt på vilket de loggar in på Marketo. Användare kommer att uppmanas att acceptera en inbjudan att logga in med Adobe Identity för första gången, antingen genom att logga in med en befintlig Adobe ID eller genom att konfigurera en ny Adobe ID med samma e-postadress. Mer information finns i [Användarinloggning med Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md) artikel.

## Användarmigreringen är klar {#user-migration-complete}

Adobe meddelar alla systemadministratörer och produktadministratörer via e-post när alla administratörer och användare har migrerats. Alla Marketo-användare för den prenumerationen loggar nu in på Marketo med Adobe Identity och produktadministratörer hanterar endast användare på Adobe Admin Console.

## Få support {#get-support}

Om du vill ha ytterligare support för din prenumeration eller din användarmigrering kan du skicka ett e-postmeddelande till marketocares@adobe.com.
