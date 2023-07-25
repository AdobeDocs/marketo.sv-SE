---
description: Versionsinformation - maj 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - maj 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Versionsinformation: Maj 2021 {#release-notes-may-21}

Följande funktioner finns i majversionen från 21. Se om det finns funktioner i din Marketo-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den **7 maj 2021**.

## Kontobaserade upplevelser {#Account-based-eaperiences}

* **Smarta kontolistor (allmän tillgänglighet)** ![](assets/yellow-star.png): Identifiera och kvalificera konton dynamiskt med önskade konto- och personattribut för att nå ut till flerkanaliga marknadsföringskampanjer och skicka aviseringar i god tid till försäljningen för att slutföra avtal snabbare. Denna nya funktion möjliggör robust automatisering av kontobaserade marknadsföringsstrategier. Smarta kontolistor är tillgängliga för kunder med Target Account Management som är med i nästa generations användarupplevelser.

## Nästa generations användarupplevelse {#next-generation-user-experience}

Med en global förhandsgranskning kan marknadsförarna snabbt se var det finns en delad resurs i deras instans. Webbläsarflikarna visar platsen för att förbättra navigeringen i Marknadsföringsaktiviteter eller Design Studio. Ytterligare filter för träd och global sökning hjälper dig att förfina sökvillkoren. Dra-och-släpp-funktionen i trädet har återställts så att du kan flytta mappar och resurser snabbt och effektivt inom huvudprogramområdena. Med nya uppdaterade ikoner (som uppfyller Adobe tillgänglighetsstandarder) och statusmärken kan marknadsförarna snabbt och enkelt skilja mellan mappar och resurser i trädet och identifiera status för program och resurser.

## Experience Automation {#experience-automation}

* **Kör steg för kampanjflöde**: Effektivisera arbetsflödena för att skapa kampanjer och förbättra kampanjresultaten med ett nytt flödessteg för smarta kampanjer. Skapa och spara centraliserade, mallkampanjer för repetitiva uppgifter på arbetsytan, till exempel normalisering av landskoder, som ska anropas och köras från alla smarta kampanjer via det nya flödessteget Kör kampanj. Länkade kampanjer körs i den angivna ordningen och säkerställer att uppgiften är slutförd innan du går vidare till nästa flödessteg. Redigera snabbt flödet i en enda centraliserad kampanj för att uppdatera alla smarta kampanjer som använder den för att effektivisera datahanteringen, poängsättningen för leads och flödena för routning.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Känsliga datafält i Forms**: Protect-kundens personligt identifierbara information (PII) kan inte visas i Adobe Marketo Engage-formulär genom att definiera datafält som känsliga och begränsa formulärförifyllning för dessa fält. När en besökare tittar på ett formulär på landningssidan, kommer de fält som definieras som känsliga inte att visa några förfyllda data.

* **Blockera inskickning av skräppostformulär**: Protect din Adobe Marketo Engage-databas från skräppostdata som kan orsaka ogiltiga varningar för försäljning, utlösa kampanjeftersläpningar och skapa oönskade aktiviteter. Den nya valideringsfunktionen avvisar ogiltiga formulärinskickningar och stoppar robotattacker. Era data är renare och era marknadsföringskampanjer fungerar som de ska, vilket minimerar risken för att skicka okvalificerade leads till försäljning.

* **Varning om godkännande av e-postprogram**: Förhindra att felaktiga e-postmeddelanden skickas när de nya ändringarna görs i ett tidigare godkänt program.  Varningen fungerar som en garanti när en marknadsförare gör ändringar i ett e-postmeddelande som redan har godkänts, men sedan glömmer att godkänna de senaste ändringarna och skickar e-postmeddelandet till en stor publik utan innehåll, dåligt innehåll eller gammalt innehåll.

* **Aktivitet för att filtrera bort e-poststarter**: Förhindra oönskade säljvarningar och felaktig e-postrapportering med den nya funktionen för filtrering av e-postrobotar. Identifiera och filtrera bort öppningar och klick som kan kopplas till e-postbots inspektera länkar som leder till falska utlösare och försäljningsvarningar, eller felaktig rapportering.

## API-förbättringar {#api-enhancements}

Flera viktiga uppdateringar av API:er för Bulk och Lead, bland annat möjlighet att exportera anpassade objektdata i bulk, associera företag med lead in bulk, möjlighet att filtrera extrahering av massaktivitet baserat på ett primärt attribut samt möjlighet att skapa och uppdatera programmedlemskap.

* **Kapsla händelseprogram**: I Adobe Marketo Engage kan du skapa, klona eller flytta händelseprogram under andra programtyper. Den här funktionen är nu tillåten i resurs-API:t.

* **Förbättrat API för att ta bort program**: Tillåter integrerade program att ta bort program som innehåller ytterligare typer av resurser, utan att användare behöver göra det manuellt från Adobe Marketo Engage.

* **Programmedlemskap**: Marknadsförarna kan fråga alla programmedlemsposter om ett visst program med olika villkor, t.ex. programmedlemmens status. Dela informationen med ett externt program, verktyg för affärsinformation eller Adobe Experience Cloud för att förbättra segmenteringen och skapa mer målinriktat engagemang.

* **Extrahera anpassat objekt gruppvis**: Export av gruppdata kompletterar de importfunktioner som dataanalytiker redan använder i Adobe Marketo Engage. Nu kan de extrahera data som lagras på den första nivån av Adobe Marketo Engage anpassade objekt i grupp, läsa in dessa data i ett annat program, data warehouse eller BI (Business Intelligence) för att få bättre insikt i data i Adobe Marketo Engage-instansen.  Anpassad massdataförflyttning av objekt är dubbelriktad och kan schemaläggas vid en lämplig tidpunkt.

* **API för metadata för anpassade fält**: Spara tid genom att automatisera skapandet av anpassade fält och samtidigt skapa Adobe Marketo Engage-integrationer med ett program från tredje part. Den här automatiseringen är särskilt användbar för kunder med flera Adobe Marketo Engage-instanser som nu kan effektivisera skapandet av anpassade fält som tidigare krävde manuellt arbete i varje instans. Effektivisera skapandet av anpassade fält och spara tid på den här resurskrävande aktiviteten.

* **API för extrahering av gruppaktivitet**: Få kontroll över mängden och typen av data när du utför massextraheringar. Filtrera bort onödiga datapunkter och kontrollera antalet API-anrop som krävs för att extrahera aktivitetsdata i grupp.  Du kan till exempel välja öppna e-postmeddelanden, besöka en webbsida eller ändra ledspår och låta andra värdeförändringar som du inte vill analysera ligga bakom. Effektivisera processen för att minska antalet API-anrop och datarensning.

* **Lead-API**: Identifiera leads i Adobe Marketo Engage som är associerade med Adobe ECID (Experience Cloud ID).  Adobe Marketo Engage-kunder kan skapa en lista med leads från en viss kampanj och använda ECID:n (Experience Cloud-ID) för att skapa rapporter i Adobe Analytics för den specifika listan. Integrationen mellan Adobe Marketo Engage och Adobe Experience Cloud ger obegränsade möjligheter till segmentering, målinriktning och rapportering.

* **API för massutaimport**: Styr import av bulkleads och resurser som krävs. Den här förbättringen skapar associationer mellan lead och företag under bulklead-importprocessen. Öka effektiviteten och arbeta med data och minska användningen om API anropar.

* **Webb-API-baserad integrering för Microsoft Dynamics Online-kunder**: MS Dynamics Web API introducerades med version 8.0 REST-protokoll och implementerar OData (Open Data Protocol) v4. OData är en OASIS-standard (Organization for the Advanced of Structured Information Standards) för att bygga upp och använda RESTful-tjänster framför omfattande data. Adobe Marketo Engage-kunder som behöver integreras med Microsoft Dynamics med den här metoden migreras för närvarande till en webb-API-baserad anslutning från SOAP (Simple Object Access Protocol).

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **XLSX-export**: Vi uppgraderade exportfunktionerna i hela produkten för att stödja XLSX istället för XLS. Det innebär att var som helst i produkten där det finns stöd för XLS-export ersätts det här alternativet med ett alternativ för att exportera till XLSX i stället. Den här ändringen påverkar filnamnen för all Excel-export av rapporter och andra data från Adobe Marketo Engage.

* **Sök efter lead-ID**: Hitta snabbt lead-poster genom att söka med Adobe Marketo Engage lead-ID i lead-databasen eller den statiska listan. I fönstret Snabbsökning skriver du `[id]` med motsvarande nummer visas leadinformationen. Användarna kan snabbt granska information om lead, företag och affärsmöjligheter.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integrering med LinkedIn Lead Gen Forms (beta)**: Få djupare insyn i era LinkedIn-kanalinvesteringar och avkastning med Bizible Premium-attribueringslösningen. Genom den senaste integreringen med LinkedIn Lead Gen Forms får Bizible insikt i de blanketter som har skickats in inom LinkedIn. Dessa formulärfyllningar matchas mot leads från din CRM-instans (Customer Relationship Management) eller Adobe Marketo Engage-instans så att de är berättigade till attribuering och kan spåras mot dina övriga marknadsföringsåtaganden.

## Meddelanden {#announcements}

* **Marketo Product Docs Switching Platforms**: Vi är glada över att kunna meddela att Marketo Product Docs går med i Adobe Experience League fr.o.m. fredag 7 maj. Du kan fortfarande använda URL:en: docs.marketo.com, och om du har befintliga artiklar som bokmärkts omdirigeras du. Alla produktdokument är tillgängliga på den nya plattformen, med förbättringar som planeras för senare i år.

* **Effektiv användaradministration och enkel inloggning via Adobe Identity System**: Från och med juli 2021 kommer de nya Adobe Marketo Engage-kunderna att introduceras med användaruppgifter för Adobe. Migrering av befintliga kunder till det integrerade identitetssystemet kommer inte att ske förrän i mitten av 2022 och inga kundåtgärder krävs förrän ytterligare varningar om detta. Med enkel inloggning kan IT-/säkerhetsadministratörer hantera flera Adobe Marketo Engage-produktinstanser tillsammans med andra Experience Cloud-lösningar samt konfigurera enkel inloggning (Shared Services Organization) via en gemensam konsol. Administratörer kan enkelt hantera användargrupper och användarrättigheter via en gemensam Admin Console.

**_Product Release Webinar_**

[Webbinariet Marketo Engage från maj 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
