---
description: Versionsinformation - juni 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - juni 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Versionsinformation: juni 2022 {#release-notes-june-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 juni. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

Följande funktioner kommer att börja släppas den **24 juni 2022**, med en fasad utrullning av återstående funktioner under de följande veckorna (om inget annat anges).

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **Visa CreatedAt/UpdatedAt-fält för anpassade objekt**: Ger dig möjlighet att inspektera dessa fält i personinformationsfönstret för att få ytterligare insikter.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Förbättrad strömning av Designer-användning för Dynamic Chat**: Lägg till kort direkt från strömmen på Designer arbetsyta utan att behöva dra och släppa. Gränssnittet i Dynamic Chat har också förbättrats så att innehåll i enskilda kort blir synligare.

* **Avancerade routningsregler för avtalad tid för Dynamic Chat**: Dynamic Chat erbjuder fler alternativ för riktad routning av avtalad tid. Ange vilka agentavtalade tider som ska dirigeras baserat på Marketo Engage-attribut, så att leads dirigeras till lämpliga agenter.

* **Avancerad dialograpportering för Dynamic Chat**: Visa resultatet för dina Dynamic Chat-kampanjer mer detaljerat med helt nya datavisualiseringar för engagemangs- och konverteringsmått.

* **Osynkroniserade oanvända Marketo Engage-attribut för Dynamic Chat**: Osynkroniserade Marketo Engage-attribut från din Dynamic Chat-prenumeration som inte används, vilket underlättar datarenhet och gör att alternativa attribut kan synkroniseras efter behov.

## Nästa generations upplevelser

**Nya Växla vy**: Vyerna nedan är nu tillgängliga i nästa generation av Experience:

* [Vyn E-postinformation](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Visa e-postlista](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Experience Automation {#experience-automation}

* **Undantag för regel för validering av globalt formulärfält**: Uteslut specifika formulär från reglerna för global formulärvalidering så att prenumerationscentraler och andra affärskritiska arbetsflöden kan acceptera alla värden.

* **Självbetjäningsflödessteg**: Utöka anslutningen mellan Marketo Engage och resten av stacken med möjligheten att skapa anpassade flödessteg för användning i smarta kampanjer. Både användare och partners i Marketo Engage kan utnyttja den här funktionen för att tillåta användning av externa webbtjänster i utlösar-, batch- och körbara kampanjer, i motsats till webbhooks, som bara kan användas i utlösarkampanjer.

* **Munchkin Protocol Agnostic Link Tracking**: Utöka stödet för spårning av `tel`- och `mailto`-länkar med Munchkin för att spåra utökade webbbeteenden.

* **Ytterligare HTTP-metoder för webhooks**: Ange PUT, PATCH och DELETE som begärandetyper för interaktion med webbtjänster.

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **Behörighetsuppsättning för Sales Insight i Salesforce**: Administratörer kan ge Sales Insight-åtkomst till en begränsad uppsättning personer på användarnivå i stället för på profilnivå via behörighetsuppsättningen för Marketo App, som är en del av Salesforce-paketet Sales Insight.

* **Min Marketo Tile Update - Sales Insight Actions**: Marketo Admins (och de användare de utser) kan nu snabbt navigera till sin instans Sales Insight Actions via en ny Sales Insight Actions-panel på My Marketo-sidan.

## Sales Connect {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Uppdatering för Salesforce-API**: I Salesforce sommar-versionen från 22 kommer äldre API-versioner 21-30 inte längre att stödjas av Salesforce. I den här Marketo Engage-versionen har alla Sales Connect-begäranden som använder äldre API-versioner uppdaterats så att de hålls i en version som stöds. Klicka [här](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"} om du vill ha fullständig information om återtagandeplaner för Salesforce API.

## API-förbättringar {#api-enhancements}

* **Nya filtreringsfunktioner för API:t för programmedlemsextraheringen**: Filtrera efter programmedlemskapsstatus, updatedAt, cadence eller slut på innehåll för att förfina den extraherade datauppsättningen.

* **Förbättring av API:t för extrahering av gruppprogrammedlem**: Ange upp till 10 program när jobb skapas för att förbättra genomströmningen.

## Meddelanden {#announcements}

* **Borttagning av Forms - Forms 1.0, lead Capture/save endpoint och no-script-versioner av formulär**: Stödet för Forms 1.0-resurser kommer att tas bort helt från Marketo Engage i oktober 2022. Alla befintliga Forms 1.0-resurser kommer inte längre att fungera. Marketo Engage-formulär kommer att kräva att JavaScript laddas på landningssidor och webbplatser.

**_Webbseminarium om produktreleaser_**

[Juniversion och augusti 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
