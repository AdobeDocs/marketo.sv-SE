---
unique-page-id: 14745730
description: Salesforce Diagnostics - Marketo Docs - produktdokumentation
title: Salesforce-diagnostik
exl-id: a2b5bd10-bc92-4fd4-bc1b-4e02b48c9d83
feature: Marketo Sales Connect
source-git-commit: 9384d72b335a4b975b190816ea999ad067fddeda
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# Salesforce-diagnostik {#salesforce-diagnostics}

En del av vår Salesforce-integrering innehåller en Salesforce-diagnostiksida i webbprogrammet. Den här sidan fångar upp fel från misslyckad dataloggning till Salesforce. Felen kan vara användbara, men de är inte alltid läsbara. Därför sammanställer vi ett kalkylblad som förklarar felmeddelandena.

**Fel:** API_CURRENTLY_DISABLED\
**Kategori:** Åtkomst/validering\
**Meddelande:** API är inaktiverat för den här användaren\
**Vad händer:** Användaren har inte API-åtkomst\
**Felsökningssteg:** Salesforce Admin måste ge användarens API-åtkomst.

<br> 

**Fel:** AUTHENTICATION_FAILURE\
**Kategori:** Autentisering\
**Meddelande:** invalid_grant: autentiseringsfel\
**Vad händer:** Autentiseringen misslyckades\
**Felsökningssteg:** Koppla från Salesforce och anslut sedan igen.

<br> 

**Fel:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Kategori:** Åtkomst/validering\
**Meddelande:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessionen har upphört eller är ogiltig&quot;}\
**Vad händer:**

1 - Utlösarkoden gör att uppdateringen misslyckas.\
2 - Användaren har inte skrivbehörighet på objektnivå för det angivna objektet.

**Felsökningssteg:**

1 - Granskningsutlösare som misslyckas.\
2 - Bevilja skrivåtkomst till användaren för objektet ELLER inaktivera funktionen som försöker skriva till objektet.

<br> 

**Fel:** CANNOT_UPDATE_CONVERTED_LEAD\
**Kategori:** Annan\
**Meddelande:** kan inte referera till konverterad lead\
**Vad händer:** Vi försöker logga till ett konverterat lead under loggning av senaste aktivitet för kontakter och leads. Jag har också sett ett par av de här.\
**Felsökningssteg:** Rapportera eventuella instanser av detta till vårt [supportteam](https://nation.marketo.com/t5/Support/ct-p/Support).

<br> 

**Fel:** ENTITY_IS_LOCKED\
**Kategori:** Åtkomst/validering\
**Meddelande:** entiteten är låst för redigering\
**Vad händer:** Posten är i en godkännandeprocess där den är låst för ytterligare redigeringar tills den antingen godkänns eller nekas av en person som äger godkännandet.\
**Felsökningssteg:** Se ovan.

<br> 

**Fel:** EXPIRED_ACCESS
**Kategori:** Autentisering
**Meddelande:** invalid_grant: utgången åtkomsttoken/uppdateringstoken
**Vad händer:** Åtkomst- eller uppdateringstoken har upphört att gälla. Tokens förfaller baserat på [sessionsinställningarna i Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Felsökningssteg:** Du måste autentisera igen. Koppla från Salesforce-anslutningen och återanslut.

<br> 

**Fel:** FAILED_WRITE\
**Kategori:** Intermittent\
**Meddelande:** filslut har nåtts\
**Vad händer:** Prestandaproblem med Salesforce, troligen på grund av suboptimala utlösare på kundsidan.\
**Felsökningssteg:** Återförsökslogiken bör hantera detta. Om det fortfarande inte fungerar kan du tillsammans med Salesforce-administratören felsöka en problematisk utlösare.

<br> 

**Fel:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Kategori:** Åtkomst/validering
**Meddelande:** Varierar från kund till kund.
**Vad händer:** En anpassad valideringsregel för objektet misslyckades.
**Felsökningssteg:** Kontrollera den anpassade verifieringsregel som orsakar det här felet. Eftersom detta är en anpassad regel måste felet hanteras en gång i taget.

<br> 

**Fel:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Kategori:** Åtkomst/validering\
**Meddelande:** Värdet finns inte eller matchar inte filtervillkoren\
**Vad är det som händer:** Befintliga felaktiga data i Salesforce kommer att framtvingas vid uppdatering.\
**Felsökningssteg:** Se ovan.

<br> 

**Fel:** FIELD_INTEGRITY_EXCEPTION\
**Kategori:** Åtkomst/validering\
**Meddelande:** Det befintliga landet/territoriet känner inte igen delstatsvärdet för fältet: Landskod/landskod\
**Vad är det som händer:** Befintliga felaktiga data i Salesforce kommer att framtvingas vid uppdatering.\
**Felsökningssteg:** Se ovan.

<br> 

**Fel:** INACTIVE_ORGANIZATION\
**Kategori:** Autentisering\
**Meddelande:** invalid_grant: inaktiv organisation\
**Vad händer:** Salesforce-organisationen är inte längre aktiv.\
**Felsökningssteg:** Koppla från och återanslut sedan från Salesforce.

**Fel:** INACTIVE_USER
**Kategori:** Autentisering
**Meddelande:** invalid_grant: inaktiv användare
**Vad händer:** Salesforce-användaren är inte längre aktiv
**Felsökningssteg:** Koppla från och återanslut sedan från Salesforce.

**Fel:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Kategori:** Intermittent\
**Meddelande:** (inget ytterligare meddelande)\
**Vad händer:** Salesforce-instansen är i underhållsläge.\
**Felsökningssteg:** Vänta tills systemunderhållet är klart och försök sedan logga igen.

**Fel:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Kategori:** Åtkomst/validering
**Meddelande:** Otillräckliga åtkomsträttigheter för objekt-ID
**Vad händer:** Ingen åtkomst till den överordnade posten för en aktivitet.
**Felsökningssteg:** Se ovan.

<br> 

**Fel:** INSUFFICIENT_ACCESS_OR_READONLY\
**Kategori:** Åtkomst/validering
**Meddelande:** Otillräckliga åtkomsträttigheter för objekt-ID
**Vad händer:** Loggning av senaste aktivitet kan inte redigera den specifika posten eftersom användaren inte har skrivåtkomst.\
**Felsökningssteg:** Bevilja användaråtkomst i Salesforce ELLER inaktivera loggning av senaste aktivitet för det objektet för den användaren.

**Fel:** INVALID_FIELD\
**Kategori:** Intermittent\
**Meddelande:** Net::ReadTimeout\
**Det som händer:** Begäran väntar. Detta beror troligen på för många långsamma transaktioner.\
**Felsökningssteg:** Granska befintliga anpassningar för att se om det finns potentiella orsaker till latensproblem och/eller inaktivera loggning av senaste aktivitet för ett eller alla objekt för att minska belastningen.

**Fel:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Kategori:** Åtkomst/validering\
**Meddelande:** Det gick inte att skapa/uppdatera fält: ToutApp__Tout_Last_Replied__c. Kontrollera säkerhetsinställningarna för det här fältet.
**Vad händer:** Användare har inte skrivåtkomst till anpassade Tout-fält som behövs för att utföra loggningstransaktionen Senaste aktivitet. Team kan ha installerat paket men har inte aktiverat rätt fält för användarna.\
**Felsökningssteg:** Salesforce Admin måste ge åtkomst till anpassade fält ELLER inaktivera loggning av senaste aktivitet.

**Fel:** INVALID_GRANT\
**Kategori:** Autentisering\
**Meddelande:** invalid_grant: ip begränsad\
**Vad händer:** Vi försöker komma åt din Salesforce, men du har IP-begränsningar som hindrar oss från att göra det.\
**Felsökningssteg:** Din Salesforce-administratör måste tillåtslista våra IP-adresser. Användare bör kontakta supporten för att få tillgång till IP-adresserna.

**Fel:** INVALID_TYPE\
**Kategori:** Åtkomst/validering\
**Meddelande:** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject` type &#39;Lead&#39; stöds inte. Om du försöker använda ett anpassat objekt måste du lägga till &#39;__c&#39; efter enhetsnamnet. Please reference your WSDL or the describe call for the appropriate names
**Vad händer:** Vi försöker fråga en objekttyp från Salesforce som användaren inte har åtkomst till. Detta är troligen relaterat till att användaren inte har rätt åtkomst till Lead-objektet.\
**Felsökningssteg:** Bevilja läsnings- och uppdateringsåtkomst till lead-objektet i Salesforce, eller inaktivera e-postloggning och loggning av senaste aktivitet för lead-poster.

**Fel:** QUERY_TIMEOUT\
**Kategori:** Intermittent\
**Meddelande:** Din frågebegäran kördes för länge\
**Vad händer:** Se ovan.\
**Felsökningssteg:** Återförsökslogiken bör hantera detta. Om det fortfarande inte fungerar kan du tillsammans med din Salesforce-administratör felsöka en problematisk utlösare.

**Fel:** REQUEST_LIMIT_EXCEEDED\
**Kategori:** Intermittent\
**Meddelande:**
1 - ConcurrentPerOrgLongTxn-gränsen har överskridits\
2 - TotalRequests-gränsen har överskridits\
3 - ConcurrentRequest\
**Vad händer:**
1 - Gränsen för samtidiga begäranden har överskridits, troligen på grund av ineffektiv utlösarkod.\
2 - För många integreringar placerar organisationen utanför det 24 timmar långa rullande fönstret.\
**Felsökningssteg:**
1 - Granska befintliga utlösare för de påverkade objekten. Det kan vara möjligt att inaktivera sammanslagningsloggning för ett eller flera objekt.\
2 - Köp fler API-anrop från Salesforce. Det kan vara möjligt att inaktivera sammanslagningsloggning för ett eller flera objekt.

**Fel:** REQUIRED_FIELD_MISSING\
**Kategori:** Åtkomst/validering\
**Meddelande:** Obligatoriska fält saknas: `[Amount_Committed_Private_Capital__c]`
**Vad händer:** Detta händer vanligtvis vid loggning av senaste aktivitet. Anpassade fält har konfigurerats för att vara obligatoriska men har tomma värden. Detta kan inträffa om posten har skapats med ett tomt värde för det anpassade fältet och sedan har gjorts till obligatorisk. Kravet upprätthålls när vi försöker uppdatera posten, även om vi inte rör det anpassade fältet.\
**Felsökningssteg:** Uppdatera värdena för de saknade fälten manuellt. Du kan sedan försöka med meddelandet igen från ToutApp.

**Fel:** SERVER_UNAVAILABLE\
**Kategori:** Intermittent\
**Meddelande:**-servern är upptagen\
**Vad händer:** Prestandaproblem med Salesforce, troligtvis på grund av att kunden inte har optimalt resultat\
**Felsökningssteg:** Återförsökslogiken bör hantera detta. Om det fortfarande inte fungerar kan du tillsammans med din Salesforce-administratör försöka skjuta en problematisk utlösare.

**Fel:** TXN_SECURITY_NO_ACCESS\
**Kategori:** Åtkomst/validering\
**Meddelande:** Den begärda åtgärden tillåts inte på grund av en säkerhetsprincip i organisationen. Kontakta administratören.<br/>
**Vad händer:** Någon typ av säkerhetsbegränsning har konfigurerats - se https://developer.salesforce.com/forums/?id=&quot;post-ID&quot;\
**Felsökningssteg:** Tala med din Salesforce-administratör och se vad den specifika begränsningen kan vara.

**Fel:** UNABLE_TO_LOCK_ROW\
**Kategori:** Intermittent\
**Meddelande:** kan inte få exklusiv åtkomst till den här posten eller 1 post: &quot;post-ID&quot;\
**Vad händer:** Sannolikt finns det en utlösare som gör att flera försök görs att få åtkomst till samma post, möjligen för gruppmeddelanden via e-post.\
**Felsökningssteg:** Återförsökslogiken bör hantera detta. Om det fortfarande inte fungerar kan du tillsammans med din Salesforce-administratör felsöka en problematisk utlösare.

**Fel:** UNKNOWN_EXCEPTION
**Kategori:** Annan\
**Meddelande:** Ett okänt undantag inträffade\
**Vad händer:** Ohanterat undantag i Salesforce.\
**Felsökningssteg:** Arkivera ett ärende med Salesforce och kopiera de numeriska värdena i felmeddelandet. Det här är Salesforce-koden som inte hanterar ett fel korrekt.
