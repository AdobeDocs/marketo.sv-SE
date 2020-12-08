---
unique-page-id: 12979858
description: Performance Insights FAQ - Marketo Docs - produktdokumentation
title: Vanliga frågor om prestandainsikter
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# Vanliga frågor om prestandainsikter {#performance-insights-faq}

## Vad är definitionen av&quot;framgång&quot; på fliken Engagement? {#what-is-the-definition-of-success-in-the-engagement-tab}

Success är ett mått på meningsfull interaktion i Marketo. Syftet med ett program är att skapa en meningsfull interaktion med personen eller den potentiella kunden. Lyckade markeras när en person når den status som uppnår det målet. Det kan vara att delta i ett webbinarium, klicka på en länk i ett e-postmeddelande eller fylla i ett webbformulär. Hur bra det är varierar beroende på programkanalen.

>[!NOTE]
>
>**Exempel**
>
>I ett webbinarium kan det finnas flera statusar, som: Inbjuden, registrerad och anmäld. Inbjudna eller registrerade är inte meningsfulla interaktioner eftersom folk egentligen inte tittar på webbinariet. I det här fallet anses det som lyckat.

## Fungerar MPI tillsammans med CRM? {#will-mpi-work-with-any-crm}

Ja. I praktiken interagerar inte MPI direkt med CRM för datasynkronisering. MPI använder data som lagras i Marketo Analytics Data warehouse. Eftersom CRM-synkroniseringen görs i Lead Management-programmet kommer alla CRM-system med stöd för Marketo som är integrerade med Lead Management-programmet att visa data korrekt. CRM-affärsmöjlighetsfälten måste dock mappas korrekt till Marketo-affärsmöjlighetsfälten.

## Jag har inga andra Marketing Analytics-produkter (ARB, RCE, RCA, Program Analysis). Fungerar MPI för mig? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI är ett oberoende tillägg till Lead Management-programmet. Inga andra analysprodukter behöver användas.

## RCA visar även prestandadata för programmet. Finns det någon skillnad mellan de data som visas i MPI och RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nej. MPI hämtar data från samma data warehouse som RCA. Därför kommer du inte att se några skillnader i data mellan de båda. Med RCA kan du skapa egna rapporter direkt. Med MPI får du tillgång till lättbegripliga visuella instrumentpaneler.

## Jag vill inte att vissa av mina program (till exempel Operational) ska visas i MPI. Hur kontrollerar jag synligheten för specifika program? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Du kan styra visningen av dina program genom att ange Analytics-beteendet för dina program till Operational. Detta gör att programmet inte tas med i analysberäkningarna.

>[!NOTE]
>
>Läs mer om hur du ställer in analysbeteende [här](http://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings).

## Jag har en flerkanalskampanj för att lansera en ny produkt. Hur kan jag se resultatet för den här kampanjen i alla olika kanaler på ett och samma ställe? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Vi rekommenderar att ni använder programtaggar för program som ingår i en sådan kampanj. Programtaggar synkroniseras automatiskt till MPI, och du kan filtrera dem på alla MPI-kontrollpaneler för att se resultatet för din flerkanalskampanj.

## Har jag åtkomst till attribueringsinställningar om jag inte har någon RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Du får tillgång till attribueringsinställningar om du har MPI, oavsett om du har RCA eller inte.

## Jag får en varning i MPI när jag loggar in och säger att mina attribueringsinställningar är felaktiga. Vad är det för fel? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI beräknar om alla dina möjligheter inkluderas i analysen eller inte. Annars uppmanas du att överväga att ändra dina attribueringsinställningar (Explicit, Implicit, Hybrid) för att inkludera fler möjligheter.

Du kanske också saknar möjligheter på grund av att programkostnaden saknas i dina program. Granska Analytics-beteendet för era program. De kan vara:

1. Standard - Standardbeteendet är att programmet ENDAST inkluderas i MPI om det finns minst en periodkostnad, även en med noll dollar tilldelat.
1. Inkluderande - Det här alternativet ser till att programmet är tillgängligt i MPI oavsett om du har inkluderat en periodkostnad eller inte.
1. [Operativ](http://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms) - Det här alternativet gör att programmet inte visas i MPI.

>[!NOTE]
>
>Periodkostnad **måste** ställas in för rapportering av lyckade och nya namn på instrumentpanelen för engagemang. På den här instrumentpanelen används periodkostnadsdata för att samla framgångar och nya namn. Om periodkostnad inte är inställt kommer instrumentpanelen för engagemang inte att rapportera korrekt oavsett inställningarna för analysbeteendet ovan.

## Varför saknar jag vissa möjligheter i MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Två viktiga orsaker till varför du kanske saknar möjligheter i MPI är:

1. Attributinställningen är Explicit men affärsmöjligheterna har inte tilldelats kontaktroller
1. Periodkostnaden ingår inte i dina program

MPI beräknar om alla dina möjligheter inkluderas i analysen eller inte. Annars uppmanas du att överväga att ändra dina attribueringsinställningar (Explicit, Implicit, Hybrid) för att inkludera fler möjligheter.

Du kanske också saknar möjligheter på grund av att programkostnaden saknas i dina program. Meddelandet kommer att visas men pekar inte på vilka program som saknar kostnader. Granska din programkonfiguration så att den innehåller kostnader för att se till att alla program och möjligheter ingår i MPI.

## Varför visas inte anpassade fält, säljprojektstyp och ABM-filter på instrumentpanelen för engagemang? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Anpassade fält, säljprojektstyp och ABM-filter är alla attribut som är relaterade till en affärsmöjlighet. Med kontrollpanelen för engagemang kan ni mäta ert engagemang och få leads oavsett om de är kopplade till en affärsmöjlighet eller inte. Eftersom instrumentpanelen för engagemang inte tar hänsyn till affärsmöjligheter, gäller inte anpassade fält, säljprojektstyp och ABM-filter.

## Jag vill använda ett anpassat Salesforce-säljprojektsfält för intäktsrapportering i stället för standardfältet Salesforce-säljprojektsbelopp. Kommer MPI att tillåta mig att göra det? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Ja. [Marketo Support](http://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) kan mappa om Marketos säljprojektsbelopp till ett anpassat Salesforce-säljprojektsfält så länge som fälttypen är valuta. Eftersom MPI pekar på fältet Marketo-säljprojektsbelopp kan MPI använda data från det ommappade anpassade Salesforce-fältet.

>[!NOTE]
>
>Efter ommappningen visar MPI data framåt. Det historiska beloppet kommer inte att ändras.

## Kan jag ändå använda MPI om jag inte utnyttjar möjligheterna? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI är utformat för att du ska kunna mäta programmets prestanda från början av processen till intäktseffekten. Om du inte utnyttjar möjligheterna kommer du fortfarande att kunna:

* Visa resultatet av era vårdsprogram för målgruppsengagemang.
* Visa resultatet för era program för värvning av leads.
* Visa resultatet för flerkanalskampanjer via programtaggar.
* Se målgruppsengagemangstrender för de senaste 12 månaderna.
* Spara och exportera prestandadata i PowerPoint.

## Kan jag mäta framgången med kontobaserade strategier i MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Ja. MPI integreras med [Marketo ABM](http://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) för att dra in ABM-kontolistor i MPI sömlöst. Du kan använda filtret ABM-kontolista för att välja önskad ABM-lista att filtrera data efter.

## Är attribuering direkt tillgängligt när jag köper MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Marketo Attribution-funktionerna är tillgängliga för våra kunder när de köper MPI. Det krävs dock [korrekt konfiguration](http://docs.marketo.com/x/mRPG) för att säkerställa att affärsmöjligheter och programdata flödar korrekt in i MPI.

## Vad måste jag göra för att konfigurera attribuering? {#what-do-i-have-to-do-to-set-up-attribution}

1. Inställningar för affärsmöjlighet

   1. Se till att affärsmöjligheterna synkroniseras med CRM
   1. Om dina attribueringsinställningar är inställda på Explicit kontrollerar du att kontaktrollerna för affärsmöjligheterna är ifyllda
   1. Vi rekommenderar att du ändrar attributinställningen till Hybrid
   1. Programinställningar

      1. Inkludera programkostnader i dina program
      1. Granska analysbeteendet för att ange om ett program ska inkluderas i analysen
      1. Ange resultatkriterier för alla kanaler du har
      1. Tie Person to Programs

         1. Kontrollera att inköpsprogrammet och förvärvsdatumet har angetts för varje person i databasen för att First Touch Attribution ska fungera.
         1. Se till att dina program anger status som lyckade för personer i din databas

>[!TIP]
>
>Alla nödvändiga installationssteg beskrivs i [den här artikeln](http://docs.marketo.com/x/mRPG).

## Vad är skillnaden mellan MPI och programanalysen? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Med Program Analyzer kan ni jämföra era program över så många som fyra åtgärder. Med MPI kan du analysera kanal- och programbidraget mot en vald mätmetod som Lyckades, Nya möjligheter skapade osv. Du kan även se trenden för 12-månaderskanalen baserat på ett specifikt mätvärde som du har valt.

## Vad är skillnaden mellan MPI och Advanced Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Advanced Report Builder (kallas ibland RCE) är utformat för självbetjäningsrapportering (eller ad hoc-rapportering), vanligtvis utförd av Marketing Operations. MPI är utformat för att ge marknadsledare och marknadsförare tillgång till prestandaanalys med ett enda klick. Minimal installation krävs.

## Vad hände med alternativet Föregående år i bidragsfiltret? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Vi har tillfälligt tagit bort markeringen&quot;Föregående år&quot;. Du kan fortfarande visa hela årets prestandadata genom att använda alternativet Anpassat datumintervall.
