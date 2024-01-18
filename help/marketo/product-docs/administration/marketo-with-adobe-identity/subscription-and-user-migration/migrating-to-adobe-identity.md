---
description: Migrera till Adobe Identity - Marketo Docs - produktdokumentation
title: Migrerar till Adobe-identitet
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: a7969204-0ec9-45aa-a206-eff2df8adcd0
source-git-commit: e99fa6d25bcf3c4a03234ce48dd17dd7c396c430
workflow-type: tm+mt
source-wordcount: '2329'
ht-degree: 0%

---

# Migrerar till Adobe-identitet {#migrating-to-adobe-identity}

När Adobe schemalägger en prenumerations användarmigrering får produktadministratörer i Marketo Engage tillgång till migreringskonsolen, som finns på navigeringsmenyn i Admin-området under avsnittet Integrering.

SCREENSHOT

## Före migrering {#pre-migration}

Innan migreringen börjar kan en administratör ändra startdatumet för användarmigreringen för sin prenumeration genom att gå till skärmen Före migrering på migreringskonsolen. Om du vill ändra datumet kan administratören klicka på **Redigera** -knappen.

SCREENSHOT

Administratören kan välja ett datum mellan 8 och 30 dagar i framtiden. När ett datum har valts måste administratören klicka **Spara** för att göra ändringen.

SCREENSHOT

>[!NOTE]
>
>Om du vill begära ett datum före 8 dagar eller efter 30 dagar, eller om du behöver justera datumet efter att konsolen före migrering är låst, skickar du ett e-postmeddelande till `marketocares@marketo.com`.

## Migrering till Adobe-identitet {#migrations-to-adobe-identity}

Alla Marketo-prenumerationer med en tidszon i USA migreras från och med midnatt, Pacific Standard Time, efter startdatumet för användarmigreringen. Migreringen av användare för alla andra prenumerationer börjar vid midnatt i prenumerationens angivna tidszon. När en prenumerations användarmigrering börjar är användarhantering inte längre tillgänglig i Marketo Admin, utan bara i Adobe Admin Console. Rollhantering finns kvar på fliken Användare och roller i Marketo Admin-området samt lokal (endast API) användarhantering.

Adobe migrerar automatiskt alla Marketo-administratörer med verifierade e-postmeddelanden först. När Marketo-administratörer migreras till Adobe Identity läggs de till i prenumerationens Adobe Admin Console som produktadministratör för Marketo-prenumerationen och tilldelas Adobe produktadministratörsrollen i Marketo-programmet (tillsammans med andra roller de tidigare haft) och har sedan rätt till prenumerationen på Adobe ID. Administratörerna får två e-postmeddelanden. Den ena anger att de har utsetts till produktadministratör för Adobe och den andra anger att de har rätt till Marketo-produkten.

**Marketo Product Administrator Email**

SCREENSHOT

**Marketo berättigandee-post**

SCREENSHOT

**Om din Marketo-prenumeration har färre än 75 användare** migrerar Adobe automatiskt resten av dina användare. Det här arbetsflödet ger den högsta nivån av automatisering och ingen åtgärd krävs för att utföra migreringen. När migreringen är klar visas inte Marketo migreringskonsol längre i navigeringsområdet i Marketo Admin och alla användare kommer att få åtkomst till Marketo via en Adobe ID.

**Om din Marketo-prenumeration har 75 eller fler användare**, får Marketo produktadministratörer tillgång till migreringsverktyget för självbetjäningsanvändare i migreringskonsolen när användarmigreringen startar och varnas via banner vid inloggning på Min Marketo-sida. Administratören ansvarar för att slutföra användarmigreringen med verktyget för självbetjäningsanvändarmigrering.

SCREENSHOT

## Marketo Self-Service User Migration {#marketo-self-service-user-migration}

Verktyget Marketo Self-Service User Migration Console består av två flikar.

* **Fliken Migreringsstatus**
* **Fliken Användarmigrering**

### Fliken Migreringsstatus {#migration-status-tab}

Fliken Migreringsstatus innehåller övergripande mätvärden för förloppet för användarens e-postverifiering, användarens migrering och aktivering samt slutförande av prenumerationsmigreringen.

SCREENSHOT

Överst i migreringsstatusen visas prenumerationsmigreringens förfallodatum och knappen för att förlänga förfallotiden. Mer information om när migreringen upphör finns i [Avsnittet Förfallotid för användarmigrering](#user-migration-expiration).

I nästa avsnitt på fliken Migreringsstatus finns två förloppsindikatorer. Den första förloppsindikatorn är att visa förloppet när användarens e-postverifiering är klar. Den andra förloppsindikatorn visar förloppet för slutförd användarmigrering.

Därefter visas tre avsnitt av statusen för administratören.

Det första avsnittet handlar om e-postverifieringsstatus för användare i prenumerationen.

Det andra avsnittet gäller användarmigrering och aktivering (dvs. migrering och berättigande till Marketo Engage-produkten) för de användare som ingår i prenumerationen.

Det tredje avsnittet handlar om prenumerationens status för slutförande av migrering.

Verifiering av användarens e-postadress

I avsnittet Verifiering av användarens e-post kan en administratör hitta den aktuella statusen för e-postverifiering för användarna i prenumerationen, innan migrering till Adobe-identitet sker.

En administratör kan visa prenumerationens e-postverifieringsstatus, hur många användare i prenumerationen som har slutfört e-postverifieringen och hur många användare som har markerats som ignorerade. Status rapporteras för alla användares e-postverifieringstillstånd i prenumerationen. Administratören kan klicka på antalet användare som hoppats över och navigeras till fliken Användarmigrering för att visa de användare som hoppats över.

Bekräftelsemeddelandet kan skickas igen av en administratör på fliken Användarmigrering på migreringskonsolen och på fliken Användare och roller i området Marketo Admin, eller av användaren i deras kontoinställningar. Länken i bekräftelsemeddelandet upphör att gälla om 3 dagar, precis som i e-postmeddelanden med användarinbjudningar. Mer information om e-postverifiering finns i Community &lt;nation.marketo.com> och i e-postverifieringsdokumentationen &lt; https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/email-verification.html?lang=en>.

VIKTIGT

Om en Marketo Engage-användare inte verifierar sin e-postadress kan de inte migreras till en Adobe ID och förlorar åtkomsten till Marketo-prenumerationen när prenumerationen har migrerats. För att återfå åtkomsten när migreringen är klar måste en Marketo-produktadministratör lägga till dem som en ny användare.

Migrering och aktivering av användare

I avsnittet Användarmigrering och aktivering hittar en administratör den aktuella statusen för total användarmigrering och behörighet till Adobe Identity Management System.

En administratör kan visa procentandelen användare i prenumerationen som har migrerats till en Adobe ID eller markerats som Överhoppad. Status rapporteras för alla användares migreringstillstånd till en Adobe ID i prenumerationen, eller markeras som Överhoppad och kommer inte att migreras. När användare migreras och har rätt till Marketo Engage, eller hoppas över, uppdateras den här statusen.

Bekräftelse av migrering

I avsnittet Bekräftelse av migrering måste en administratör bekräfta att användarmigreringen har slutförts för prenumerationen.

När alla användare i prenumerationen har tagits med (antingen migrerats eller hoppats över) visas knappen för att slutföra migreringen.

SCREENSHOT

Administratören som utför migreringen måste slutföra migreringsbekräftelsen genom att klicka på knappen Slutför migrering. De uppmanas att bekräfta att migreringen har slutförts.

SCREENSHOT

När användarmigreringen är klar tas migreringskonsolen bort från navigeringsmenyn i Admin.

### Förfallotid för användarmigrering {#user-migration-expiration}

Adobe kräver att man slutför självbetjäningsmigreringar inom 30 dagar. Administratörer kommer inte att blockeras från att migrera användare eller slutföra migreringen om utgångsdatumet har passerat, men de kommer bara att kunna migrera användare på begäran.  Om en administratör behöver mer tid kan de förlänga prenumerationens förfallodatum.

SCREENSHOT

Genom att klicka på knappen &quot;Utöka förfallodatum&quot; uppdateras datumet till en vecka senare. En administratör kan förlänga giltigheten upp till tre gånger.

SCREENSHOT

SCREENSHOT

Adobe kommer att vara ute efter att en kund inte har slutfört migreringen före förfallodatumet.

### Fliken Användarmigrering {#user-migration-tab}

På fliken Användarmigrering kan administratörer ha fullständig kontroll över användarmigreringen.

Administratörer kan välja att:

Utlös verifieringsmeddelanden för overifierade användare via knappen Verifiera e-post

Hoppa över användarmigrering för användare som administratören vet inte kan/kommer inte att verifiera sin e-post eller ska inte migreras via knappen Hoppa över migrering

Migrera valda användare vid behov via knappen Migrera nu

Schemalägg användarmigrering för valda användare för ett specifikt datum med knappen Schemalägg migrering

Migrera alla berättigade användare på begäran (inget användarval behövs) via knappen Migrera alla användare

SCREENSHOT

Verifiera e-post

E-postverifiering krävs för att en användare ska kunna migreras till en Adobe ID. Om det finns användare som inte har verifierat sin e-postadress och behöver migreras, kan administratören utlösa bekräftelsemeddelandet som skickas till användaren igen. Om du väljer en overifierad användare aktiveras knappen Bekräfta e-post och meddelandet skickas.

SCREENSHOT

När administratören klickar på knappen Bekräfta e-post får de ett meddelande om att e-postmeddelandet har skickats.

SCREENSHOT

Hoppa över och ångra användarmigrering

Under användarmigreringen måste alla användare antingen migreras eller hoppas över. Adobe kräver att administratörer bekräftar att en användare inte migreras och att en administratör måste markera användaren som överhoppad. Om administratören inte gör det kan de inte bekräfta att användarmigreringen har slutförts. Alla användare som hoppats över kommer inte längre att ha tillgång till Marketo när migreringen är klar.

VIKTIGT

En administratör måste hoppa över alla användare med overifierade e-postmeddelanden. Om det finns användare som har verifierat sina e-postmeddelanden, men administratören inte vill migrera dem av någon anledning, bör de markeras som ignorerade.

Om du vill hoppa över en användare kan administratören välja önskad användare. Knappen Hoppa över migrering aktiveras. När du klickar på knappen Hoppa över migrering uppdateras sidan och den valda användarens verifieringsstatus och migreringsstatus uppdateras till Överhoppad.

SCREENSHOT

En administratör kan ångra hoppet över en användare som hoppats över, om det upptäcks att användaren måste migreras.

Administratören kan välja önskad användare om användaren ska ångras. Knappen för att ångra migrering aktiveras. När du klickar på knappen Ångra migrering uppdateras sidan.  Den valda användarens verifieringsstatus uppdateras till den aktuella statusen, antingen Verifierad eller Overifierad, och användarens migreringsstatus uppdateras till Inte startad.

SCREENSHOT

ANMÄRKNING

Knappen Ångra migrering är bara aktiv om alla valda användare har migreringsstatusen Överhoppad.

Migrera Marketo-användare till Adobe-ID:n

För kunder som vill ha större kontroll under användarmigreringen stöder Marketo självbetjäning för prenumerationer med 75 eller fler användare. Marketo produktadministratörer kan välja vilka användare som ska migreras gruppvis, eller alla berättigade användare samtidigt. När användarna har valts kan administratörerna välja att migrera nu eller Schemalägg migrering för ett senare datum, vilket ger administratörerna den flexibilitet och kontroll som behövs för att migrera och när användarna ska migreras. Administratörer kan också välja att migrera alla användare i en prenumeration.

En administratör kan t.ex. välja en grupp med&quot;avancerade&quot; användare som de vill migrera först. När dessa användarmigreringar har slutförts kan de välja olika grupper baserat på exempelvis arbetsyta eller affärsfunktion eller roll för att batchmigrera användare ytterligare. Eller så kan de bestämma sig för att migrera alla övriga användare i prenumerationerna efter att den första gruppbearbetningen har slutförts. Målet är att ge största flexibilitet när det gäller att distribuera Adobe ID till användare.

Alla användarmigreringar sker samtidigt och bör slutföras inom sextio sekunder. När en användarmigrering sker för en viss användare kan användaren förlora åtkomsten i upp till en minut, och det är bara om användaren är inloggad i programmet. När användarmigreringen är klar får användaren ett e-postmeddelande om hur man loggar in i Marketo Engage med en Adobe-identitet. Användaren måste acceptera inbjudan via knapplänken i e-postmeddelandet. När användaren har accepterat inbjudan bör han/hon logga in med en Adobe ID. Här finns instruktioner om hur du loggar in i Marketo Engage med en Adobe ID. &lt; https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.html>

SCREENSHOT

Användarmigreringar behandlas oberoende av varandra, så om en användarmigrering misslyckas kommer Adobe att fortsätta att bearbeta andra användarmigreringar. Om ett migreringsfel inträffar krävs ingen åtgärd av en administratör. Adobe Engineering kommer att arbeta för att åtgärda problemet så snart som möjligt. Administratören kommer att få ett e-postmeddelande om felet och få ett meddelande om att Adobe arbetar med att lösa problemet omedelbart. Om en användares migrering misslyckas och användaren är inloggad i Marketo Engage, kan användaren förlora åtkomsten i upp till två minuter, medan det görs nya migreringsförsök.  Om en användares migrering misslyckas kan användaren fortsätta få åtkomst till Marketo-identiteten i Marketo Engage tills han/hon får ett e-postmeddelande om att migreringen lyckades och han/hon uppmanas att logga in med en Adobe ID.

SCREENSHOT

Migrera nu

En administratör kan välja en eller flera användare att migrera på begäran. Detta kommer att utlösa migreringen av användarna omedelbart. Om du vill migrera en eller flera användare väljer administratören önskade användare och knappen Migrera nu aktiveras.

SCREENSHOT

ANMÄRKNING

Knappen Migrera nu är bara aktiv om alla valda användare har Verified-status.

När du klickar på knappen Migrera nu uppmanas administratören att bekräfta migreringen av de valda användarna. När administratören har bekräftat börjar användarmigreringen bearbetas så snart som möjligt.

SCREENSHOT

Schemalägg migrering

En administratör kan välja en eller flera användare att schemalägga migrering vid ett senare datum. Om du vill schemalägga migrering för en eller flera användare väljer administratören önskade användare och knappen Schemalägg migrering aktiveras.

SCREENSHOT

ANMÄRKNING

Knappen Schemalägg migrering är bara aktiv om alla valda användare har Verified-verifieringsstatus.

När du klickar på knappen Schemalägg migrering uppmanas administratören att välja önskat migreringsdatum för de valda användarna. Administratören kan bara välja datum före prenumerationens förfallodatum för migrering. När administratören har bekräftat kommer migreringen/migreringarna att schemaläggas att börja bearbetas det valda datumet.

SCREENSHOT

ANMÄRKNING

Alla Marketo-prenumerationer med en tidszon i USA migreras från och med midnatt, Pacific Standard Time, från migreringens startdatum. Migreringen av användare för alla andra prenumerationer börjar vid midnatt i prenumerationens angivna tidszon.

Migrera alla användare

En administratör kan när som helst välja att migrera alla berättigade användare i en prenumeration. Detta kommer att utlösa migreringen av de berättigade användarna omedelbart. Berättigade användare är användare med verifierade e-postmeddelanden som ännu inte har migrerats.

SCREENSHOT

När du klickar på knappen Migrera alla användare uppmanas administratören att bekräfta migreringen av alla berättigade användare. När administratören har bekräftat börjar användarmigreringen bearbetas så snart som möjligt.

SCREENSHOT
