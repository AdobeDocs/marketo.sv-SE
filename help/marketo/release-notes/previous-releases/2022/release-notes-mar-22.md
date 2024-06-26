---
description: Versionsinformation - mars 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - mars 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Versionsinformation: Mars 2022 {#release-notes-mar-22}

Följande funktioner finns i mars 22. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att lanseras den **11 mars 2022**, med en fasad utrullning av alla funktioner under de följande veckorna (om inget annat anges).

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Dynamiskt chatt**: Maximera alla möjligheter på er webbplats genom att rikta in er på både leads och konton med proaktiva, engagerande och personliga konversationer. [Dynamiskt chatt](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} gör att användare av Marketo Engage kan börja utnyttja chatt som en viktig del i integrerade flerkanalsupplevelser för B2B-marknadsföring och säljtillfällen. Funktioner: möjlighet att boka möten direkt i chatten, lead-routning, startmallar, dra-och-släpp-konversation och mycket annat. Dynamic Chat ingår i alla paket med Marketo Engage och kommer att lanseras för alla användare av Marketo Engage i år.

* **Förbättring av filtrering av e-poststartaktivitet**: Som en förbättring av tidigare släppta [Filtrering av startaktivitet för e-post](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} kan du nu välja att logga aktiviteter som identifieras som bottar. Du kan sedan filtrera och utlösa åtgärder baserat på aktiviteter som identifieras som utförda av bots.

## Nästa generations upplevelse {#modern-ux}

* **Uppdaterade skärmar i nästa generation**: Vi levererar nya, uppdaterade skärmar i nästa generation av upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Formulärlistvy i Design Studio (inklusive nya massåtgärder)

* **Uppdatera importprogramarbetsflöde**: Arbetsflödet för importprogram levereras i nästa generation med uppdaterade design- och användarförbättringar. Detta blir en automatisk ändring utan en växlingsknapp.

* **Administratörskontroll för nästa generations växel för Experience Toggle**: Hantera lanseringen av nästa generation av upplevelser på ett sätt som fungerar för dina användare och gör det möjligt för administratörer att välja vilka användartyper som kan få åtkomst till växlingsfunktionen.

## Experience Automation {#experience-automation}

* **Självbetjäningsflödessteg (beta)**: Utöka anslutningsmöjligheterna mellan Marketo Engage och resten av högen med möjligheten att skapa anpassade flödessteg som kan användas i smarta kampanjer. Både Marketo användare och partners kan utnyttja den här funktionen för att möjliggöra användning av externa webbtjänster i både gruppkampanjer och körbara kampanjer, i motsats till webbhooks, som bara kan användas i utlösarkampanjer.

* **Resursens förfallodatum**: Behåll kontrollen över era tidskänsliga resurser och kampanjer genom att schemalägga deras automatiska inaktivering vid ett visst datum och en viss tidpunkt i den klassiska användarupplevelsen.

* **Åsidosättning av prioritet för smart kampanj**: Se till att högprioriterade Smart Campaigns körs så snart som möjligt med möjlighet att åsidosätta standardprioritetsordningen för kampanjer. Smarta kampanjer med lägre prioritet kan också minskas i prioritet för att frigöra bearbetningsresurser för andra högprioriterade uppgifter.

## API-förbättringar {#api-enhancements}

* **Returnera inaktiverad status för e-postspårning vid öppen spårning**: Tillåter läsning av e-postmeddelanden med statusen öppen spårning via API
* **Hämta ämnesrader för dynamiskt innehåll från e-post**: Gör det möjligt för marknadsförare att analysera dynamiska ämnesrader i BI-verktyg
* **Anpassade fält för programmedlemmar**: Låter marknadsförare programmässigt skapa anpassade fält för programmedlemmar
* **Export av anpassat objekt i grupp uppdaterad vid filter**: Låter marknadsförare programmässigt synkronisera anpassade objekt
* **Dispose Head Start Setting for Email Programs**: Gör att marknadsförare kan konfigurera e-postprogram med förstartsstart via API
* **Selektiv programtagguppdatering**: Marknadsförarna kan pusha selektiva tagguppdateringar utan att skjuta på alla taggar samtidigt
* **ÅtgärdResultatfält för massaktivitetsextrahering**: Låter marknadsförarna identifiera vilka aktiviteter som hoppades över eller misslyckades

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## Bizible {#bizible}

![(stjärna)](assets/yellow-star.png)

* **BI-mallar**: Bizible kommer nu att innehålla nedladdningsbara, grundläggande rapporteringsartefakter och exempelrapporter för Tableau och Power BI för snabb utveckling av anpassade rapporter som är anpassade för just era affärsbehov.

## Sales Connect {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Begränsning av e-postanslutning (GA)**: Begränsning av e-postanslutning gör att Sales Connect-administratörer kan konfigurera sändningsfrekvensen för e-postmeddelanden när Gmail eller Exchange används som leveranskanal, så att den hastighet med vilken e-postmeddelanden skickas till leveranskanalleverantören inte överskrider de tvingande gränserna.

## Meddelanden {#announcements}

* **Borttagning av Marketo Sky**: I mars kommer Marketo Sky inte längre att vara tillgänglig eftersom vi fokuserar på att leverera nästa generations användarupplevelser. I ett försök att behålla åtkomst till funktioner som är exklusiva för Marketo Skyn idag, tar vi bort förfallodatum för resurser och åsidosättning av Smart Campaign-prioritet i den klassiska upplevelsen. [Klicka här](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) om du vill veta mer.

**_Product Release Webinar_**

[Mars och maj 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
