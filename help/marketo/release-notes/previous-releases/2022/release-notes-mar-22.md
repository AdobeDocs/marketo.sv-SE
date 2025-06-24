---
description: Versionsinformation - mars 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - mars 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Versionsinformation: mars 2022 {#release-notes-mar-22}

Följande funktioner finns i mars 22. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att börja släppas den **11 mars 2022**, med en fasad utrullning av alla funktioner under de följande veckorna (om inget annat anges).

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**: Maximera alla möjligheter på webbplatsen genom att rikta in er på både leads och konton med proaktiva, engagerande och personliga konversationer. Med [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} kan Marketo Engage-användare börja använda chatt som en viktig del av integrerade upplevelser över flera kanaler för B2B-marknadsföring och säljtillfällen. Funktioner: möjlighet att boka möten direkt i chatten, lead-routning, startmallar, dra-och-släpp-konversation med mera. Dynamic Chat ingår i alla Marketo Engage-paket och kommer att lanseras för alla Marketo Engage-användare i år.

* **Förbättring av filtrering av aktivitetsfiltrering via e-post**: Som en förbättring av den tidigare släppta funktionen [Filtrering av aktivitetsfiltrering via e-post](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} kan du nu välja att logga aktiviteter som identifieras som bottar. Du kan sedan filtrera och utlösa åtgärder baserat på aktiviteter som identifieras som utförda av bots.

## Nästa generations upplevelse {#modern-ux}

* **Uppdaterade Screens i nästa generations upplevelse**: Vi levererar nya, uppdaterade skärmar i nästa generations upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Formulärlistvy i [!UICONTROL Design Studio] (inklusive nya massåtgärder)

* **Uppdatering av arbetsflöde för import av program**: Arbetsflödet för import av program levereras i nästa generation med uppdaterade design- och användbarhetsförbättringar. Detta blir en automatisk ändring utan en växlingsknapp.

* **Administratörskontroll för nästa generations växling av upplevelseväxlingar**: Hantera utrullningen av nästa generation av upplevelser på ett sätt som fungerar för dina användare och gör det möjligt för administratörer att välja vilka användartyper som ska få åtkomst till växlingsväxeln.

## Experience Automation {#experience-automation}

* **Självbetjäningsflödessteg (Beta)**: Utöka anslutningen mellan Marketo Engage och resten av stacken med möjligheten att skapa anpassade flödessteg som kan användas i smarta kampanjer. Både Marketo användare och partners kan utnyttja den här funktionen för att möjliggöra användning av externa webbtjänster i både gruppkampanjer och körbara kampanjer, i motsats till webbhooks, som bara kan användas i utlösarkampanjer.

* **Resursförfallodatum**: Behåll kontrollen över dina tidskänsliga resurser och kampanjer med möjligheten att schemalägga deras automatiska inaktivering vid ett visst datum och en viss tidpunkt i den klassiska användarupplevelsen.

* **Åsidosättning av prioritet för smart kampanj**: Kontrollera att smarta kampanjer med hög prioritet körs så snart som möjligt med möjlighet att åsidosätta prioritetsordningen för standardkampanjer. Smarta kampanjer med lägre prioritet kan också minskas i prioritet för att frigöra bearbetningsresurser för andra högprioriterade uppgifter.

## API-förbättringar {#api-enhancements}

* **Returnera Inaktivera status för öppen spårning för e-postmeddelanden**: Tillåter att öppen spårningsstatus för e-postmeddelanden läses via API
* **Hämta ämnesrader för dynamiskt innehåll från e-post**: Gör att marknadsförare kan analysera dynamiska ämnesrader i BI-verktyg
* **Anpassade fält för programmedlemmar i CRUD**: Gör att marknadsförare kan skapa anpassade fält för programmedlemmar via programkod
* **Massexport av anpassade objekt uppdateradVid filter**: Låter marknadsförare programmässigt synkronisera anpassade objekt
* **Visa startinställning för HEAD för e-postprogram**: Gör att marknadsförare kan konfigurera e-postprogram med förstartsstart via API
* **Uppdatering av Selektiv programtagg**: Gör att marknadsförare kan skicka uppdateringar av selektiva taggar utan att alla taggar behöver skickas samtidigt
* **Åtgärd för extrahering av gruppaktivitetResultatfält**: Låter marknadsförare identifiera vilka aktiviteter som hoppades över eller misslyckades

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Bizible] {#bizible}

![(stjärna)](assets/yellow-star.png)

* **BI-mallar**: [!DNL Bizible] kommer nu att innehålla hämtningsbara, grundläggande rapportartefakter och exempelrapporter för Tableau och Power BI för att möjliggöra snabb utveckling av anpassade rapporter som är anpassade för dina specifika affärsbehov.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Begränsning av e-postanslutning (GA)**: Med begränsning av e-postanslutning kan [!DNL Sales Connect]-administratörer konfigurera sändningsfrekvensen för e-postmeddelanden när Gmail eller [!DNL Exchange] används som leveranskanal, så att den hastighet med vilken e-postmeddelanden skickas till leveransleverantören inte överskrider de tvingande gränserna.

## Meddelanden {#announcements}

* **Borttagning av Marketo Sky**: I mars kommer Marketo Sky inte längre att vara tillgängligt eftersom vi fokuserar våra resurser på att leverera nästa generations användarupplevelser. I ett försök att behålla åtkomsten till funktioner som är exklusiva för Marketo Sky idag, tar vi med åsidosättande av förfallodatum och prioritet för smarta kampanjer i den klassiska upplevelsen. [Klicka här](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) om du vill veta mer.

**_Webbseminarium om produktreleaser_**

[Mars och maj 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
