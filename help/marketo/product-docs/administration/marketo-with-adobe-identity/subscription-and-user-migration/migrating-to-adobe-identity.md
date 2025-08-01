---
description: Migrera till Adobe Identity - Marketo Docs - produktdokumentation
title: Migrera till Adobe Identity
feature: Marketo with Adobe Identity
exl-id: a7969204-0ec9-45aa-a206-eff2df8adcd0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2319'
ht-degree: 0%

---

# Migrera till Adobe Identity {#migrating-to-adobe-identity}

När Adobe schemalägger en prenumerations användarmigrering får Marketo Engage produktadministratörer tillgång till migreringskonsolen, som finns på navigeringsmenyn i administratörsområdet under Integrering.

![](assets/migrating-to-adobe-identity-1.png)

## Före migrering {#pre-migration}

Innan migreringen börjar kan en administratör ändra startdatumet för användarmigreringen för sin prenumeration genom att gå till skärmen Före migrering på migreringskonsolen. Om du vill ändra datumet kan administratören klicka på knappen **Redigera**.

![](assets/migrating-to-adobe-identity-2.png)

Administratören kan välja ett datum mellan 8 och 30 dagar i framtiden. När ett datum är markerat måste administratören klicka på **Spara** för att göra ändringen.

![](assets/migrating-to-adobe-identity-3.png)

>[!NOTE]
>
>Om du vill begära ett datum före 8 dagar eller efter 30 dagar, eller om du behöver justera datumet efter att konsolen före migrering är låst, skickar du ett e-postmeddelande till `marketocares@marketo.com`.

## Migrering till Adobe Identity {#migrations-to-adobe-identity}

Alla Marketo-prenumerationer med en tidszon i USA migreras från och med midnatt, Pacific Standard Time, efter startdatumet för användarmigreringen. Migreringen av användare för alla andra prenumerationer börjar vid midnatt i prenumerationens angivna tidszon. När en prenumerations användarmigrering börjar är användarhantering inte längre tillgänglig i Marketo Admin, utan bara i Adobe Admin Console. Rollhantering finns kvar på fliken Användare och roller i Marketo Admin-området samt lokal (endast API) användarhantering.

Adobe migrerar automatiskt alla Marketo-administratörer (med en standardadministratörsroll) med verifierade e-postmeddelanden först. När Marketo-administratörer migreras till Adobe Identity läggs de till i prenumerationens Adobe Admin Console som produktadministratör för Marketo-prenumerationen och tilldelas Adobe produktadministratörsrollen i Marketo-programmet (tillsammans med andra roller de tidigare haft) och har sin Adobe ID berättigad till prenumerationen. Administratörerna får två e-postmeddelanden. Den ena anger att de har utsetts till produktadministratör för Admin Console och den andra anger att de har rätt till Marketo-produkten.

>[!IMPORTANT]
>
>Du måste klicka på knappen **Acceptera inbjudan** i tillståndsmeddelandet för att få tillgång till Marketo Engage med din Adobe ID.

**E-postadress till Marketo produktadministratör**

![](assets/migrating-to-adobe-identity-4.png)

**E-postadress för Marketo Entitlement**

![](assets/migrating-to-adobe-identity-5.png)

**Om din Marketo-prenumeration inte har enkel inloggning i Marketo och/eller din Adobe-organisation** migrerar Adobe automatiskt resten av dina användare. Det här arbetsflödet ger den högsta nivån av automatisering och ingen åtgärd krävs för att utföra migreringen. När migreringen är klar visas inte Marketo migreringskonsol längre i navigeringsområdet i Marketo Admin och alla användare kommer att få åtkomst till Marketo via en Adobe ID.

**Om din Marketo-prenumeration har enkel inloggning i Marketo och/eller din Adobe-organisation** får Marketo-administratörer tillgång till självbetjäningsverktyget för migreringskonsolen när användarmigreringen startar och varnas via banner vid inloggning på sidan My Marketo. Administratören ansvarar för att slutföra användarmigreringen med verktyget för självbetjäningsanvändarmigrering.

![](assets/migrating-to-adobe-identity-6.png)

## Marketo Self-Service User Migration {#marketo-self-service-user-migration}

Verktyget Marketo Self-Service User Migration Console består av två flikar.

* **Fliken Migreringsstatus**
* **Fliken Användarmigrering**

Det krävs tre huvudsteg för att slutföra en migrering till självbetjäning.

1. Migrera alla önskade berättigade e-postadressverifierade användare (fliken Användarmigrering)
1. Hoppa över alla icke berättigade användare och alla oönskade berättigade användare (fliken Användarmigrering)
1. När steg 1 och 2 är klart slutför du migreringsbekräftelsen (fliken Migreringsstatus)

### Fliken Migreringsstatus {#migration-status-tab}

Fliken Migreringsstatus innehåller övergripande mätvärden för förloppet för användarens e-postverifiering, användarens migrering och aktivering samt slutförande av prenumerationsmigreringen.

![](assets/migrating-to-adobe-identity-7.png)

Överst i migreringsstatusen visas prenumerationsmigreringens förfallodatum och knappen för att förlänga förfallotiden. Mer information om förfallodatum för migrering finns i avsnittet [Förfallotid för användarmigrering](#user-migration-expiration).

I nästa avsnitt på fliken Migreringsstatus finns två förloppsindikatorer. Den första förloppsindikatorn är att visa förloppet när användarens e-postverifiering är klar. Den andra förloppsindikatorn visar förloppet för slutförd användarmigrering.

Därefter visas tre avsnitt av statusen för administratören.

* **Verifiering av användarens e-post**: verifieringsstatus för användare i prenumerationen.
* **Användarmigrering och aktivering**: användarmigrering och aktivering (migrering och tillstånd till Marketo Engage-produkten) för användarna i prenumerationen.
* **Bekräftelse av migrering**: Status för prenumerationens slutförande av migreringen.

#### Verifiering av användarens e-postadress {#user-email-verification}

I avsnittet Verifiering av e-post för användare kan en administratör hitta den aktuella statusen för e-postverifiering för användarna i prenumerationen, innan migrering till Adobe Identity.

En administratör kan visa prenumerationens e-postverifieringsstatus, hur många användare i prenumerationen som har slutfört e-postverifieringen och hur många användare som har markerats som ignorerade. Status rapporteras för alla användares e-postverifieringstillstånd i prenumerationen. Administratören kan klicka på antalet användare som hoppats över och navigeras till fliken Användarmigrering för att visa de användare som hoppats över.

Bekräftelsemeddelandet kan skickas igen av en administratör på fliken Användarmigrering på migreringskonsolen och på fliken Användare och roller i området Marketo Admin, eller av användaren i deras kontoinställningar. Länken i bekräftelsemeddelandet upphör, precis som med e-postmeddelanden från användare, om 3 dagar. Mer information om e-postverifiering finns på [användarforumet](https://nation.marketo.com/) och i [e-postverifieringsdokumentationen](/help/marketo/product-docs/administration/users-and-roles/email-verification.md).

>[!IMPORTANT]
>
>Om en Marketo Engage-användare inte verifierar sin e-postadress kan de inte migreras till en Adobe ID och förlorar åtkomsten till Marketo-prenumerationen när migreringen är klar. För att återfå åtkomst måste en Marketo-produktadministratör lägga till dem som en ny användare.

#### Migrering och aktivering av användare {#user-migration-and-activation}

I avsnittet Användarmigrering och aktivering hittar en administratör aktuell status för total användarmigrering och behörighet till Adobe Identity Management System.

En administratör kan visa procentandelen användare i prenumerationen som har migrerats till en Adobe ID eller markerats som Överhoppad. Status rapporteras för alla användares migreringstillstånd till en Adobe ID i prenumerationen, eller markeras som Överhoppad och kommer inte att migreras. När användare migreras och har rätt till Marketo Engage, eller hoppas över, uppdateras den här statusen.

#### Bekräftelse av migrering {#migration-confirmation}

I avsnittet Bekräftelse av migrering måste en administratör bekräfta att användarmigreringen har slutförts för prenumerationen.

När alla användare i prenumerationen har tagits med (antingen migrerats eller hoppats över) visas knappen för att slutföra migreringen.

![](assets/migrating-to-adobe-identity-8.png)

Administratören som utför migreringen måste slutföra migreringsbekräftelsen genom att klicka på knappen **Slutför migrering** . De uppmanas att **bekräfta**.

![](assets/migrating-to-adobe-identity-9.png)

När användarmigreringen är klar tas migreringskonsolen bort från navigeringsmenyn i Admin.

### Förfallotid för användarmigrering {#user-migration-expiration}

Adobe kräver att man slutför självbetjäningsmigreringar inom 30 dagar. Administratörer kommer inte att blockeras från att migrera användare eller slutföra migreringen om utgångsdatumet har passerat, men de kommer bara att kunna migrera användare på begäran. Om en administratör behöver mer tid kan de förlänga prenumerationens förfallodatum.

![](assets/migrating-to-adobe-identity-10.png)

När du klickar på knappen **Utöka förfallodatum** uppdateras datumet till en vecka senare. En administratör kan förlänga giltigheten upp till tre gånger.

![](assets/migrating-to-adobe-identity-11.png)

![](assets/migrating-to-adobe-identity-12.png)

Adobe kommer att kontakta dig om du inte är klar med migreringen före förfallodatumet.

### Fliken Användarmigrering {#user-migration-tab}

På fliken Användarmigrering kan administratörer ha fullständig kontroll över användarmigreringen.

Administratörer kan välja att:

* Utlös verifieringsmeddelanden för overifierade användare via knappen Verifiera e-post
* Hoppa över användarmigrering för användare som administratören vet kan/inte kan verifiera sin e-postadress eller ska inte migreras via knappen Hoppa över migrering
* Migrera valda användare vid behov via knappen Migrera nu
* Schemalägg användarmigrering för valda användare för ett specifikt datum med knappen Schemalägg migrering
* Migrera alla berättigade användare på begäran (inget användarval behövs) via knappen Migrera alla användare

![](assets/migrating-to-adobe-identity-13.png)

**Verifiera e-post**

E-postverifiering krävs för att en användare ska kunna migreras till en Adobe ID. Om det finns användare som inte har verifierat sin e-postadress och behöver migreras, kan administratören utlösa bekräftelsemeddelandet som skickas till användaren igen. Om du väljer en overifierad användare blir knappen Bekräfta e-post klickbar.

![](assets/migrating-to-adobe-identity-14.png)

När administratören klickar på knappen **Verifiera e-post** får de ett meddelande om att e-postmeddelandet har skickats.

![](assets/migrating-to-adobe-identity-15.png)

**Hoppa över och ångra användarmigrering**

Under användarmigreringen måste alla användare antingen migreras eller hoppas över. Adobe kräver att administratörer bekräftar att en användare inte migreras och att en administratör måste markera användaren som överhoppad. Om administratören inte gör det kan de inte bekräfta att användarmigreringen har slutförts. Alla användare som hoppats över kommer inte längre att ha tillgång till Marketo när migreringen är klar.

>[!IMPORTANT]
>
>En administratör måste hoppa över alla användare med overifierade e-postmeddelanden. Om det finns användare som har verifierat sina e-postmeddelanden, men administratören inte vill migrera dem av någon anledning, bör de markeras som ignorerade.

Om du vill hoppa över en användare kan administratören välja önskad användare. Knappen Hoppa över migrering blir klickbar. När du klickar på knappen **Hoppa över migrering** uppdateras sidan och den valda användarens verifieringsstatus och migreringsstatus uppdateras till Överhoppad.

![](assets/migrating-to-adobe-identity-16.png)

En administratör kan ångra hoppet över en användare som hoppats över, om det är fastställt att användaren måste migreras.

Administratören kan välja önskad användare om användaren ska ångras. Knappen för att ångra migrering kan klickas. När du klickar på knappen **Ångra migrering** uppdateras sidan.  Den valda användarens verifieringsstatus uppdateras till den aktuella statusen, antingen Verifierad eller Overifierad, och användarens migreringsstatus uppdateras till Inte startad.

![](assets/migrating-to-adobe-identity-17.png)

>[!NOTE]
>
>Knappen Ångra migrering är bara aktiv om alla valda användare har migreringsstatusen Överhoppad.

### Migrera Marketo-användare till Adobe ID:n {#migrating-marketo-users-to-adobe-ids}

Marketo produktadministratörer kan välja vilka användare som ska migreras gruppvis, eller alla berättigade användare samtidigt. När användarna har valts kan administratörerna välja att migrera nu eller Schemalägg migrering för ett senare datum, vilket ger administratörerna flexibilitet och kontroll över vilka användare som migreras och när. Administratörer kan också välja att migrera alla användare i en prenumeration.

En administratör kan till exempel välja en grupp med&quot;avancerade användare&quot; som de vill migrera först. När dessa användarmigreringar har slutförts kan de välja olika användargrupper baserat på variabler som arbetsyta/företag eller funktion/roll för att batchmigrera användare ytterligare. Eller så kan de bestämma sig för att migrera resten av användarna i prenumerationerna efter att den första gruppen har slutförts. Målet är att tillhandahålla största möjliga flexibilitet när det gäller att distribuera Adobe ID:n till användare.

Alla användarmigreringar sker samtidigt och bör slutföras inom sextio sekunder. När en användarmigrering sker för en viss användare kan användaren förlora åtkomsten i upp till en minut, och det är bara om användaren är inloggad i programmet. När migreringen är klar får användaren ett e-postmeddelande om hur man loggar in på Marketo Engage med en Adobe-identitet. Användaren måste acceptera inbjudan via knapplänken i e-postmeddelandet _innan_ de kan logga in med en Adobe ID. Instruktioner om hur du loggar in på Marketo Engage med en Adobe ID [finns här](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md).

![](assets/migrating-to-adobe-identity-18.png)

Användarmigreringar behandlas oberoende av varandra, så om en användarmigrering misslyckas kommer Adobe att fortsätta att bearbeta andra användarmigreringar. Om ett migreringsfel inträffar krävs ingen åtgärd av en administratör. Administratören får ett e-postmeddelande om felet och får ett meddelande om att Adobe arbetar med att lösa problemet omedelbart. Om en användares migrering misslyckas och den användaren är inloggad på Marketo Engage, kan användaren förlora åtkomsten i upp till två minuter medan migreringsförsök sker igen. Om en användares migrering misslyckas kan användaren fortsätta få åtkomst till Marketo Engage med sin Marketo-identitet tills han/hon får ett e-postmeddelande om att migreringen lyckades och han/hon uppmanas att logga in med en Adobe ID.

![](assets/migrating-to-adobe-identity-19.png)

**Migrera nu**

En administratör kan välja en eller flera användare att migrera på begäran. Detta kommer att utlösa migreringen av användarna omedelbart. Om du vill migrera en eller flera användare kan administratören välja önskade användare och knappen Migrera nu kan klickas.

![](assets/migrating-to-adobe-identity-20.png)

>[!NOTE]
>
>Knappen Migrera nu är bara aktiv om alla valda användare har Verified-status.

När du klickar på knappen **Migrera nu** uppmanas administratören att bekräfta migreringen av de valda användarna. När administratören har bekräftat börjar användarmigreringen bearbetas så snart som möjligt.

![](assets/migrating-to-adobe-identity-21.png)

**Schemalägg migrering**

En administratör kan välja en eller flera användare att schemalägga migrering vid ett senare datum. Om du vill schemalägga migrering för en eller flera användare väljer administratören önskade användare och knappen Schemalägg migrering blir klickbar.

![](assets/migrating-to-adobe-identity-22.png)

>[!NOTE]
>
>Knappen &quot;Schemalagd migrering&quot; är bara aktiv om alla användare har verifieringsstatusen &quot;Verifierad&quot; och migreringsstatusen &quot;Inte startad&quot; eller &quot;Adobe ID skapad&quot;.

När du klickar på knappen **Schemalägg migrering** uppmanas administratören att välja önskat migreringsdatum för de valda användarna. Administratören kan bara välja datum före prenumerationens förfallodatum för migrering. När administratören bekräftar det schemaläggs användarmigreringen(en) att börja bearbetas det valda datumet.

![](assets/migrating-to-adobe-identity-23.png)

>[!NOTE]
>
>Alla Marketo-prenumerationer med en tidszon i USA migreras från och med midnatt, Pacific Standard Time, från migreringens startdatum. Migreringen av användare för alla andra prenumerationer börjar vid midnatt i prenumerationens angivna tidszon.

**Migrera alla användare**

En administratör kan när som helst välja att migrera alla berättigade användare i en prenumeration. Detta kommer att utlösa migreringen av de berättigade användarna omedelbart. Berättigade användare är användare med verifierade e-postmeddelanden som ännu inte har migrerats.

![](assets/migrating-to-adobe-identity-24.png)

När du klickar på knappen **Migrera alla användare** uppmanas administratören att **bekräfta**-migrering för alla berättigade användare. När administratören bekräftar det kommer användarmigreringen att börja bearbeta så snart som möjligt.

![](assets/migrating-to-adobe-identity-25.png)
