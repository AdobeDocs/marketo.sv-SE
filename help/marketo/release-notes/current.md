---
description: Aktuell versionsinformation - Marketo Docs - produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 3fe29ccb26e72b593f8b410a45a4871e68fb5fa8
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Versionsinformation: Juni 2022 {#release-notes-june-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 juni. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

Följande funktioner kommer att lanseras den **24 juni 2022**, med en stegvis utrullning av återstående funktioner under de följande veckorna (om inget annat anges).

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **Visa CreatedAt/UpdatedAt-fält för anpassade objekt**: Ger dig möjlighet att inspektera de här fälten i personinformationsfönstret för att få ytterligare insikter.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Förbättrad användning av Stream Designer för dynamiskt chatt**: Lägg till kort direkt från arbetsytan i Stream Designer utan att behöva dra och släppa. Gränssnittet Dynamic Chat har också förbättrats så att innehåll i enskilda kort blir synligare.

* **Avancerade routningsregler för avtalad tid för dynamiskt chatt**: Dynamic Chat erbjuder fler alternativ för riktad routning av avtalade tider. Ange vilka agentavtalade tider som ska dirigeras baserat på Marketo Engage-attribut, så att leads dirigeras till lämpliga agenter.

* **Avancerad dialograpportering för dynamiskt chatt**: Se resultatet för era Dynamic Chat-kampanjer i detalj med helt nya datavisualiseringar för engagemang och konverteringsstatistik.

* **Osynkroniserade oanvända Marketo Engage-attribut för dynamiskt chatt**: Osynkroniserade Marketo Engage-attribut från din Dynamic Chat-prenumeration som inte används hjälper dig att rensa bort data och som gör det möjligt att synkronisera alternativa attribut efter behov.

## Experience Automation {#experience-automation}

* **Undantag för verifieringsregel för globalt formulärfält**: Undanta specifika formulär från Global Form Validation Rules så att prenumerationscentraler och andra affärskritiska arbetsflöden kan acceptera alla värden.

* **Självbetjäningsflödessteg**: Utöka anslutningsmöjligheterna mellan Marketo Engage och resten av högen med möjligheten att skapa anpassade flödessteg som kan användas i smarta kampanjer. Både användare och partners i Marketo Engage kan utnyttja den här funktionen för att tillåta användning av externa webbtjänster i utlösar-, batch- och körbara kampanjer, i motsats till webbhooks, som bara kan användas i utlösarkampanjer.

* **Munchkin Protocol-agentlänkspårning**: Utöka stödet för spårning av `tel` och `mailto` länkar med Munchkin för att spåra fler webbbeteenden.

* **Ytterligare HTTP-metoder för webhooks**: Ange PUT, PATCH och DELETE som begärandetyper för interaktion med webbtjänster.

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **Behörighetsuppsättning för försäljningsinsikter i Salesforce**: Administratörer kan ge Sales Insight åtkomst till en begränsad uppsättning personer på användarnivå i stället för på profilnivå via behörighetsgruppen Marketo App, som ingår i Sales Insight Salesforce-paketet.

* **Min Marketo Tile Update - Sales Insight Actions**: Marketo-administratörer (och de användare de utser) kan nu snabbt navigera till sin instans av Sales Insight Actions via en ny Sales Insight Actions-panel på My Marketo-sidan.

## Sales Connect {#sales-connect}

* **Uppdatering för Salesforce API**: I Salesforce Sommar 22 stöds inte längre äldre API-versioner 21-30 av Salesforce. I den här Marketo Engage-versionen har alla Sales Connect-begäranden som använder äldre API-versioner uppdaterats så att de hålls i en version som stöds. Om du vill ha fullständig information om återtagandeplaner för Salesforce API klickar du på [här](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## API-förbättringar {#api-enhancements}

* **Nya filtreringsfunktioner för API:t för Bulk Program Member Extract**: Filtrera efter status för programmedlemskap, updatedAt, cadence eller slut på innehåll för att förfina extraherade datauppsättningar.

* **Förbättring av API för Massprogrammedlemsextrahering**: Ange upp till 10 program när du skapar jobb för att förbättra genomströmningen.

## Meddelanden {#announcements}

* **Forms-borttagning - Forms 1.0, lead Capture/save endpoint och no-script-versioner av formulär**: Stöd för Forms 1.0-material kommer att tas bort helt från Marketo Engage i oktober 2022. Alla befintliga Forms 1.0-resurser kommer inte längre att fungera. För Marketo Engage-formulär krävs att JavaScript läses in på landningssidor och webbplatser.

**_Product Release Webinar_**

Besök oss den 24 augusti 2022 kl. 9.00 PT/12.00 ET för en [live webbinarium](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} som hanteras av vårt produktteam där du kan lära dig att använda alla de senaste produktinnovationerna.
