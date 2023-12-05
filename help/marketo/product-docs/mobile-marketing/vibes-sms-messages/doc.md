---
description: Dok - Marketo Docs - produktdokumentation
title: Dok
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 0%

---

# Dok {#doc}

Text

## Vibes SMS-ordlista {#vibes-sms-glossary}

<table>
<thead>
  <tr>
    <th>Villkor</th>
    <th>Definition</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Anskaffningskampanj</td>
    <td>En kampanj för att få nya prenumeranter på dina prenumerationslistor. En prenumerant kan läggas till i en värvningskampanj via ett Marketo-webbformulär eller genom att skriva ett nyckelord.</td>
  </tr>
  <tr>
    <td>Campaign Manager</td>
    <td>Campaign Manager finns på Vibes-plattformen och är där du kan skapa en prenumerationslista och en anskaffningskampanj. Användare med en fullständig Vibes-plattformslicens har tillgång till ytterligare kampanjtyper.</td>
  </tr>
  <tr>
    <td>Företagsnyckel</td>
    <td>company_key är en unik alfanumerisk identifierare för ditt plattformskonto. Om du har flera företagskonton på Vibes-plattformen (till exempel underordnade konton) kan du ha flera company_keys. Varje instans av Marketo Engage kan endast mappas till en Vibes company_key.</td>
  </tr>
  <tr>
    <td>CTA (uppmaning)</td>
    <td>Digitala eller fysiska skyltar eller ordningstecken för att få abonnenter att delta i ett återkommande textmeddelandeprogram eller en prenumerationslista. Kan placeras online, på sociala medier, i e-post, i tryck osv.</td>
  </tr>
  <tr>
    <td>Anpassad, kort domän</td>
    <td>Om du använder länkförkortningen Vibes visas den förkortade URL:en som standard under den korta URL:en för Vibes: https://vbs.cm/xxxxxx. En anpassad, kort domän är en unik domän för ert varumärke. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Läs mer om anpassade korta domäner</a>.<p>
    Detta gäller endast meddelanden som skickas från den vibes-plattformen, särskilt kundvärvningskampanjmeddelanden och standardmeddelanden med kort kod.<p>
    Marketo URL-förkortningen rekommenderas för att du ska kunna få klickdata i ditt Marketo-program.</td>
  </tr>
  <tr>
    <td>Standardmeddelanden</td>
    <td>Obligatoriska meddelanden för den korta koden som ska svara på förfrågningar om HELP, STOP och okända meddelanden.</td>
  </tr>
  <tr>
    <td>Koppla från</td>
    <td>Frånkopplingar är en form av avanmälan på grund av att mobilnumret tas bort från ett bärarnätverk. Orsaker till en frånkoppling är bland annat: ett konto har stängts helt, ett förbetalt konto har slut på medel eller så har numret tagits bort från transportföretagets nätverk av andra okända orsaker. Mobilnummer som inte är anslutna och som inte porteras till något annat mobilföretag tas bort från alla prenumerationslistor på Vibes-plattformen.</td>
  </tr>
  <tr>
    <td>Dubbel anmälan</td>
    <td>En förvärvsmetod som kräver att en potentiell prenumerant bekräftar sitt samtycke till att läggas till i en prenumerationslista med ett svarskommando som"Y" eller deras postnummer. Genom att använda en uppmaning om dubbel anmälan kan du följa riktlinjer för textmeddelanden på delstatsnivå och federationsnivå.</td>
  </tr>
  <tr>
    <td>Händelse</td>
    <td>En händelse är en definierad förekomst som kan skickas till Vibes-plattformen och användas för att utlösa API-utlösta åtgärder, inklusive meddelandeutskick. Varje händelse innehåller data som är specifika för händelsen, inklusive en event_type, som används för att avgöra vilken API-utlöst meddelandekampanj den motsvarar. Händelse-API:t kan utlösas via Webkrok i Marketo Engage. Läs mer om våra <a href="https://developer-platform.vibes.com/reference/event-api">Händelse-API-referens</a>.</td>
  </tr>
  <tr>
    <td>Nyckelord</td>
    <td>Ett kort ord eller en alfanumerisk sträng som konsumenten skickar till den korta koden för att initiera en mobilupplevelse.</td>
  </tr>
  <tr>
    <td>Lång kod (10DLC)</td>
    <td>Ett avsändar-ID från vilket tvåvägsmeddelanden skickas mellan varumärket och konsumenten. Amerikanska långa koder är tio numeriska siffror.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Mobilkatalognummer eller en persons telefonnummer. MDN och mobiltelefonnummer är inte unika identifierare i Marketo.</td>
  </tr>
  <tr>
    <td>Mobildatabas</td>
    <td>Mobildatabasen är den databas där Vibes lagrar prenumerantdata. Varje prenumerant har en unik"personpost" där mobilnumret och tillhörande anpassade fält fylls i.</td>
  </tr>
  <tr>
    <td>Deltagare</td>
    <td>En person som har en eller flera mobilinteraktioner (till exempel att skicka ett textmeddelande) med ditt mobilprogram, men som inte har prenumererat på någon prenumerationslista.</td>
  </tr>
  <tr>
    <td>Personpost</td>
    <td>En personpost är en samling data för ett visst mobiltelefonnummer. Varje personpost tilldelas också en unik person_key för identifiering. Marketo ID:n länkas till Vibes med hjälp av fältet external_person_id. Läs mer om personposter i <a href="https://developer-platform.vibes.com/reference/person-api">Vibes Person API-dokumentation</a>.</td>
  </tr>
  <tr>
    <td>Kort kod</td>
    <td>Ett avsändar-ID från vilket tvåvägsmeddelanden skickas mellan varumärket och konsumenten. Amerikanska korta koder är 5-6 siffror. Kanadensiska korta koder är 4-6 siffror. Marketo LaunchPoint-integreringen till Vibes har stöd för en kort kod per instans.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Kort meddelandetjänst. Det här är ett meddelande som bara innehåller text.</td>
  </tr>
  <tr>
    <td>Prenumerationslistor</td>
    <td>En lista över mobilnummer (och deras motsvarande personposter) som gett tillåtelse att ta emot återkommande meddelanden från ditt program.</td>
  </tr>
  <tr>
    <td>Prenumerant</td>
    <td>Ett mobilnummer som prenumererar på en eller flera prenumerationslistor.</td>
  </tr>
  <tr>
    <td>Vibes Platform</td>
    <td>Webbplatsen du loggar in på för att hantera kampanjer. Gå till <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> för att få tillgång till Vibes plattform.</td>
  </tr>
</tbody>
</table>

## SMS-rapportering {#sms-reporting}

Text

Klicka på SMS-meddelandets lokala resurs > Visa instrumentpanel; rapporter på meddelandenivå

SCREENSHOT

SMS-progression - visar totalt antal skickade och totalt levererade. Beloppen visas till höger och om du håller pekaren över fältet visas procentvärdet.

SCREENSHOT

I diagrammet Sammanfattning visas den beräknade studsfrekvensen i procent. Håll pekaren över stapeln om du vill visa leveransfrekvensen per belopp och procent. Håll muspekaren över den orangefärgade studsfrekvensen i fältet för att visa beloppen och procentsatserna för den mjuka studsfrekvensen och den hårda studsfrekvensen.

SCREENSHOT

Med diagrammet Aktivitet över tid kan du välja Totalt skickat eller Totalt levererat. Välj ett lämpligt intervall från datumintervallväljaren.

SCREENSHOT
