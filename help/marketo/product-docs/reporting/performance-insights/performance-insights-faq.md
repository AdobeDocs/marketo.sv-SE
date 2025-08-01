---
unique-page-id: 12979858
description: Performance Insights FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om prestandainsikter
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# Vanliga frågor om [!UICONTROL Performance Insights] {#performance-insights-faq}

## Vad är definitionen av &quot;lyckades&quot; på fliken [!UICONTROL Engagement]? {#what-is-the-definition-of-success-in-the-engagement-tab}

Success är ett mått på meningsfull interaktion i Marketo. Syftet med ett program är att skapa en meningsfull interaktion med personen eller den potentiella kunden. Lyckade markeras när en person når den status som uppnår det målet. Det kan vara att delta i ett webbinarium, klicka på en länk i ett e-postmeddelande eller fylla i ett webbformulär. Hur bra det är varierar beroende på programkanalen.

>[!NOTE]
>
>I ett webbinarium kan det finnas flera statusar, t.ex.: Inbjuden, Registrerad och Bifogad. Inbjudna eller registrerade är inte meningsfulla interaktioner eftersom folk egentligen inte tittar på webbinariet. I det här fallet anses det som lyckat.

## Fungerar MPI tillsammans med CRM? {#will-mpi-work-with-any-crm}

Ja. I praktiken interagerar inte MPI direkt med CRM för datasynkronisering. MPI använder data som lagras i Marketo Analytics Data Warehouse. Eftersom CRM-synkroniseringen görs i Lead Management-programmet visas data korrekt i alla CRM-system som Marketo stöder tillsammans med Lead Management-programmet. CRM-affärsmöjlighetsfälten måste dock mappas korrekt till Marketo affärsmöjlighetsfält.

## Jag har inga andra Marketing Analytics-produkter (ARB, RCE, RCA, Program Analysis). Fungerar MPI för mig? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI är ett oberoende tillägg till Lead Management-programmet. Inga andra analysprodukter behöver användas.

## RCA visar även prestandadata för programmet. Finns det någon skillnad mellan de data som visas i MPI och RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nej. MPI hämtar data från samma datalager som RCA. Därför kommer du inte att se några skillnader i data mellan de båda. Med RCA kan du skapa egna rapporter direkt. Med MPI får du tillgång till lättbegripliga visuella instrumentpaneler.

## Jag vill inte att vissa av mina program (t.ex. Operational) ska visas i MPI. Hur kontrollerar jag synligheten för specifika program? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Du kan styra visningen av dina program genom att ange Analytics-beteendet för dina program till Operational. Detta gör att programmet inte tas med i analysberäkningarna.

>[!NOTE]
>
>Läs mer om hur du ställer in analysbeteende [här](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Jag har en flerkanalskampanj för att lansera en ny produkt. Hur kan jag se resultatet för den här kampanjen i alla olika kanaler på ett och samma ställe? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Vi rekommenderar att ni använder programtaggar för program som ingår i en sådan kampanj. Programtaggar synkroniseras automatiskt till MPI, och du kan filtrera dem på alla MPI-kontrollpaneler för att se resultatet för din flerkanalskampanj.

## Har jag åtkomst till attribueringsinställningar om jag inte har någon RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Du får tillgång till attribueringsinställningar om du har MPI, oavsett om du har RCA eller inte.

## Jag får en varning i MPI när jag loggar in och säger att mina attribueringsinställningar är felaktiga. Vad är det för fel? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI beräknar om alla dina möjligheter inkluderas i analysen eller inte. Annars uppmanas du att överväga att ändra dina attribueringsinställningar (Explicit, Implicit, Hybrid) för att inkludera fler möjligheter.

Du kanske också saknar möjligheter på grund av att programkostnaden saknas i dina program. Granska Analytics-beteendet för era program. De kan vara:

1. Standard - Standardbeteendet är att programmet ENDAST inkluderas i MPI om det finns minst en periodkostnad, även en med noll dollar tilldelat.

1. Inkluderande - Det här alternativet ser till att programmet är tillgängligt i MPI oavsett om du har inkluderat en periodkostnad eller inte.

1. [Operativ](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Det här alternativet gör att programmet inte visas i MPI.

>[!NOTE]
>
>Periodkostnaden **har** att ställa in för rapportering av lyckade och nya namn på instrumentpanelen för engagemang. På den här instrumentpanelen används periodkostnadsdata för att samla framgångar och nya namn. Om periodkostnad inte är inställt kommer instrumentpanelen för engagemang inte att rapportera korrekt oavsett inställningarna för analysbeteendet ovan.

## Varför saknar jag vissa möjligheter i MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Två viktiga orsaker till varför du kanske saknar möjligheter i MPI är:

1. Attributinställningen är Explicit men affärsmöjligheterna har inte tilldelats kontaktroller
1. Periodkostnaden ingår inte i dina program

MPI beräknar om alla dina möjligheter inkluderas i analysen eller inte. Annars uppmanas du att överväga att ändra dina attribueringsinställningar (Explicit, Implicit, Hybrid) för att inkludera fler möjligheter.

Du kanske också saknar möjligheter på grund av att programkostnaden saknas i dina program. Varningen kommer att visas men pekar inte på vilka program som saknar kostnader. Granska din programkonfiguration så att den innehåller kostnader för att se till att alla program och möjligheter ingår i MPI.

## Varför visas inte anpassade fält, säljprojektstyp och ABM-filter på instrumentpanelen för engagemang? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Anpassade fält, säljprojektstyp och ABM-filter är alla attribut som är relaterade till en affärsmöjlighet. Med kontrollpanelen för engagemang kan ni mäta ert engagemang och få leads oavsett om de är kopplade till en affärsmöjlighet eller inte. Eftersom instrumentpanelen för engagemang inte tar hänsyn till affärsmöjligheter, gäller inte anpassade fält, säljprojektstyp och ABM-filter.

## Jag vill använda ett anpassat fält för Salesforce-säljprojekt för intäktsrapportering i stället för standardfältet för Salesforce-säljprojektsbelopp. Kommer MPI att tillåta mig att göra det? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Ja. [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) kan mappa om Marketo fält för säljprojektsbelopp till ett anpassat fält för Salesforce-säljprojekt så länge som fälttypen är valuta. Eftersom MPI pekar på beloppsfältet för Marketo-säljprojekt kan MPI använda data från det ommappade anpassade Salesforce-fältet.

>[!NOTE]
>
>Efter ommappningen visar MPI data framåt. Det historiska beloppet kommer inte att ändras.

## Kan jag ändå använda MPI om jag inte utnyttjar möjligheterna? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI är utformat för att du ska kunna mäta programmets prestanda från början av processen till intäktseffekten. Om du inte utnyttjar möjligheterna kan du fortfarande:

* Visa resultatet av era vårdsprogram för målgruppsengagemang.
* Visa resultatet för era program för värvning av leads.
* Visa resultatet för flerkanalskampanjer via programtaggar.
* Se målgruppsengagemangstrender för de senaste 12 månaderna.
* Spara och exportera prestandadata i PowerPoint.

## Kan jag mäta framgången med kontobaserade strategier i MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Ja. MPI integreras med [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) för att dra in ABM-kontolistor till MPI sömlöst. Du kan använda filtret ABM-kontolista för att välja önskad ABM-lista att filtrera data efter.

## Är attribuering direkt tillgängligt när jag köper MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Marketo Attribution-funktionerna är tillgängliga för våra kunder när de köper MPI. [korrekt konfiguration](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) krävs dock för att säkerställa att affärsmöjligheter och programdata flödar korrekt till MPI.

## Vad måste jag göra för att konfigurera attribuering? {#what-do-i-have-to-do-to-set-up-attribution}

1. Inställningar för affärsmöjlighet

   1. Se till att affärsmöjligheterna synkroniseras med CRM
   1. Om dina attribueringsinställningar är inställda på Explicit kontrollerar du att kontaktrollerna för affärsmöjligheterna är ifyllda
   1. Vi rekommenderar att du ändrar attributinställningen till Hybrid
   1. Programinställningar

      1. Inkludera programkostnader i dina program
      1. Granska analysbeteendet för att ange om ett program ska inkluderas i analysen
      1. Ange resultatkriterier för alla kanaler du har
      1. Koppla person till program

         1. Kontrollera att inköpsprogrammet och förvärvsdatumet har angetts för varje person i databasen för att First Touch Attribution ska fungera.
         1. Se till att dina program anger status som lyckade för personer i din databas

>[!TIP]
>
>Alla nödvändiga installationssteg beskrivs i [den här artikeln](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Vad är skillnaden mellan MPI och programanalysen? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Med Program Analyzer kan ni jämföra era program över så många som fyra åtgärder. Med MPI kan du analysera kanal- och programbidraget mot en vald mätmetod som Lyckades, Nya möjligheter skapade osv. Du kan även se trenden för 12-månaderskanalen baserat på ett specifikt mätvärde som du har valt.

## Vad är skillnaden mellan MPI och Advanced Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Advanced Report Builder (kallas ibland RCE) är utformat för självbetjäningsrapportering (eller ad hoc-rapportering), som vanligtvis utförs av Marketing Operations. MPI är utformat för att ge marknadsledare och marknadsförare tillgång till prestandaanalys med ett enda klick. Minimal installation krävs.

## Vad hände med alternativet Föregående år i bidragsfiltret? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Vi har tillfälligt tagit bort markeringen&quot;Föregående år&quot;. Du kan fortfarande visa hela årets prestandadata genom att använda alternativet Anpassat datumintervall.
