---
description: Versionsinformation - oktober 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - oktober 2021
exl-id: 6b363c9b-7abe-4576-a362-0ad5cf515c02
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# Versionsinformation: oktober 2021 {#release-notes-oct-21}

Följande funktioner ingår i versionen från 21 oktober. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att börja släppas den **22 oktober 2021**, med en fasad utrullning av alla funktioner under den följande veckan (om inget annat anges).

## AI-driven innovation {#ai-driven-innovation}

* **Prediktiva målgruppsförbättringar**: Nu får du mer insyn i de vanligaste beteendena som påverkar AI-prediktioner för de AI-baserade prediktiva modeller som används i händelse- och e-postprogram. Du kan granska kampanjmedlemmens beteenden som resulterar i registreringar av högre händelser och närvaro, samt vad som leder till att prenumerationen avbryts. AI-baserade lookalike-modeller kan nu användas i alla programtyper i Marketo Engage.

## Nästa generations upplevelser {#next-gen-experience}

* **Välj din egen upplevelse**: Växla enkelt till den upplevelse du föredrar med den nya växlingsknappen när du arbetar i Marketo Engage formulärinformation eller på landningssidans listvy utan att förlora sammanhang, resurser eller inställningar. Dessutom förbättrar den nya listvyn på landningssidor din upplevelse med nya filter och möjligheten att utföra massåtgärder.

* **Sök effektivt**: Hjälpmedelsförbättringar för global sökning omfattar uppdaterad tangentbordsnavigering och etikettbeskrivningar, en ny rullningsfunktion för resultat och mer synliga använda filter.

* **Övervaka aktiviteter**: Övervaka status för aktiviteter som körs i bakgrunden av den nya upplevelsen via det nya aktivitetsmeddelandefältet i det globala navigeringsfältet. Facket innehåller meddelanden om uppgifter som har initierats från den nya upplevelsevyn av formulärdetaljer och landningssidans lista, inklusive ändringar av status på landningssidor och allmänna massåtgärder med hjälp av den nya upplevelsen.

## Experience Automation {#experience-automation}

* **Stöd för anpassade fält för att skicka formulär-API-programmedlemmar**: API-slutpunkten för att skicka formulär har uppgraderats till stöd för anpassade fält för programmedlemmar, vilket gör att anpassade formulärintegreringar kan samla in programspecifika data.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

* **Inbyggd Adobe Experience Platform Connector för att dela målgrupper med Marketo Engage**: Aktivera flerkanalsmarknadsföring i Marketo Engage för målgruppssegment som skapats i Adobe Experience Platform via en intern målanslutning. Kopplingen använder e-postadresser eller ECID för att matcha Adobe Experience Platform-profiler med Marketo Engage personposter, vilket resulterar i segmentdelning mellan program. Marketo Engage statiska listor fylls i automatiskt så att marknadsförarna kan nå målgrupper med personaliserade meddelanden eller initierade arbetsflöden. Aktivera målgrupper genom att utnyttja sitt konto och sin säljsituation och en mer komplett, enhetlig realtidsprofil i Experience Platform.

* **Adobe Experience Platform Marketo Data Source Connector**: Användare av både Adobe Experience Platform och Marketo Engage kan använda Marketo Source Connector för att hämta data från Marketo till AEP. Ni kan strömma data (och ändringar av dessa) från Marketo inom AEP för att säkerställa att data är konsekventa mellan de två produkterna. Marketo Connector visas via katalogen Sources, som listas under &quot;Adobe Applications&quot;.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

**[!DNL Sales Insight]för [!DNL Microsoft Dynamics 365] Försäljning**

* **[!UICONTROL Best Bets]Förbättringar**: Fliken [!UICONTROL Best Bets] i [!DNL Sales Insight] ger säljarna en realtidsvy över de hetaste kontakterna och leads som prioriteras efter kvalitet och snabbhet. Vi har lagt till möjligheten för säljarna att vidta åtgärder, till exempel: granska en persons poäng, skicka ett e-postmeddelande eller lägga till potentiella kunder till utvalda Marketo Engage-kampanjer direkt från sidan [!DNL Best Bets], vilket ökar effektiviteten och snabbar upp svarstiden.

* **Ny e-post, webbaktivitet, anonyma instrumentpaneler för webbaktivitet**: Vi har lagt till de nya kontrollpanelerna för försäljning för att informera säljarna om deras leads och kontakter i de senaste e-post- och webbaktiviteterna. Med nya filtreringsfunktioner ger kontrollpanelerna nu insikt i öppning av e-post, klickningar och besök på webbsidor för en fullständig lista över konton eller ett specifikt konto. Marketo Engage spårar all webbaktivitet och tillhandahåller försäljning med viktig information, vilket omvandlar anonym trafik till leads. Säljarna kan personalisera engagemanget och konvertera leads till försäljning snabbare eftersom de får bättre information om ledande beteenden och agerar utifrån alla kontaktytor.

**[!DNL Sales Insight]för[!DNL Salesforce]**

* **Konto- och säljprojektsnivå[!UICONTROL Best Bets]**: [!DNL Sales Insight] erbjuder nu säljarna möjlighet att granska Bästa val för alla kontakter på kontot eller affärsmöjligheten de äger, även när kontakten har tilldelats en annan teammedlem. Detta ger konto- och affärsmöjlighetsägare fullständig insyn i relevanta kontakters aktiviteter och hjälper dem att agera utifrån en mer holistisk bild av kontot eller affärsmöjligheten.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Förbättrade insikter om försäljningsaktivitet**: En ny spårningsaktivitet för e-postsvar, Sälje-post besvarad, spårar mottagarnas interaktioner med ett e-postmeddelande som automatiskt synkroniseras med Marketo Engage. Dessutom har Source-attributet uppdaterats från&quot;Tout&quot; till&quot;Sales App&quot;. Den här aktiviteten kan exporteras och rapporteras via Marketo Engage REST API eller gruppexport och är tillgänglig för filter och utlösare som ytterligare begränsningar för smarta listor, vilket utökar personaliseringsalternativen i smarta kampanjer.

* **Effektiv användarupplevelse**: Den här uppdateringen innehåller nya teckensnitt, färger, knappar och moduler för [!DNL Sales Connect] som baseras på designsystemet i Adobe Spectrum. Med dessa uppdateringar levererar vi en effektivare upplevelse, där säljarna kan fokusera på det som behövs, när det behövs.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible]Integrering med Adobe Privacy Service (GA)**: [!DNL Bizible] integrering med Adobe Privacy Service centraliserar kompatibiliteten med viktiga sekretessbestämmelser, som GDPR (General Data Privacy Regulation) eller CCPA (California Consumer Privacy Act), mellan Adobe Experience Cloud-program. Du kan nu utnyttja den här tjänsten och hantera alla sekretessförfrågningar centralt via Adobe Privacy Service så att ändringsförfrågningar som kommer till [!DNL Bizible] och andra Adobe-produkter återspeglas i alla program.

## Meddelanden {#announcements}

* **Associate Lead Deprecation/Munchkin Beta 161 Update**: 7 september 2021 började version 161 av Munchkin att lansera till 10 % av prenumerationerna med Munchkin Beta aktiverat, följt av 50 % den 16 september och 100 % den 30 september. Ändringen påverkar Marketo Engage landningssidor och den version av filen munchkin-beta.js som används för externa landningssidor som läses in från prenumerationer som den senaste versionen har lanserats till. Den här versionen är helt inaktuell för metoden [!DNL Munchkin] Associate Lead, som är en funktion som tillåter att en persons data skickas till en Marketo Engage-prenumeration och associerade webbläsarhistorik med en känd personpost. Associate Lead tas bort med stöd för mer moderna och säkra alternativ, som Forms JS API, API:t för formulärsändning och Associate Lead REST API. [Läs mer om den här borttagningen här](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/).

* **[!DNL Sales Connect]Uppdatering**: En nyligen utförd ändring av användargränssnittet i [!DNL Sales Connect] har gjort att vissa modaler i [!DNL Salesforce] har klippts av. Utför en [paketuppdatering](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md) för att åtgärda detta.

**_Webbseminarium om produktreleaser_**

[Oktober 2021 Marketo Engage Release Webinar](https://engage.marketo.com/October_Release_Webinar_On-Demand.html)
