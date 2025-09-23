---
description: Versionsinformation - juni 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - juni 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Versionsinformation: juni 2022 {#release-notes-june-22}

Här nedan hittar du alla funktioner som ingår i versionen från 22 juni. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

Följande funktioner kommer att börja släppas den **24 juni 2022**, med en fasad utrullning av återstående funktioner under de följande veckorna (om inget annat anges).

## Marknadsföringsdatamiljö {#marketing-data-environment}

* **Visa CreatedAt/UpdatedAt-fält för anpassade objekt**: Ger dig möjlighet att inspektera dessa fält i personinformationsfönstret för att få ytterligare insikter.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

* **Förbättrad strömning av Designer-användning för[!DNL Dynamic Chat]**: Lägg till kort direkt från strömmens Designer-arbetsyta utan att behöva dra och släppa. Gränssnittet [!DNL Dynamic Chat] har också förbättrats så att innehåll i enskilda kort visas bättre.

* **Avancerade routningsregler för avtalad tid för[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] innehåller fler alternativ för riktad routning av avtalad tid. Ange vilka agentavtalade tider som ska dirigeras baserat på Marketo Engage-attribut och se till att leads dirigeras till lämpliga agenter.

* **Avancerad dialograpportering för[!DNL Dynamic Chat]**: Visa resultatet för dina [!DNL Dynamic Chat]-kampanjer mer detaljerat med helt nya datavisualiseringar för engagemangs- och konverteringsmått.

* **Osynkroniserade oanvända Marketo Engage-attribut för[!DNL Dynamic Chat]**: Osynkroniserade Marketo Engage-attribut från din [!DNL Dynamic Chat]-prenumeration som inte används, vilket underlättar datarenhet och gör det möjligt att synkronisera alternativa attribut efter behov.

## Nästa generations upplevelser

**Nya Växla vy**: Vyerna nedan är nu tillgängliga i nästa generation av Experience:

* [Vyn E-postinformation](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Visa e-postlista](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Experience Automation {#experience-automation}

* **Undantag för regel för validering av globalt formulärfält**: Uteslut specifika formulär från reglerna för global formulärvalidering så att prenumerationscentraler och andra affärskritiska arbetsflöden kan acceptera alla värden.

* **Självbetjäningsflödessteg**: Utöka anslutningen mellan Marketo Engage och resten av stacken med möjligheten att skapa anpassade flödessteg för användning i smarta kampanjer. Både Marketo Engage-användare och -partners kan utnyttja den här funktionen för att tillåta användning av externa webbtjänster i utlösar-, batch- och körbara kampanjer, i motsats till Webhooks, som bara kan användas i utlösarkampanjer.

* **Munchkin Protocol Agnostic Link Tracking**: Utöka stödet för spårning av `tel`- och `mailto`-länkar med Munchkin för att spåra utökade webbbeteenden.

* **Ytterligare HTTP-metoder för webhooks**: Ange PUT, PATCH och DELETE som begärandetyper för interaktion med webbtjänster.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[!DNL Sales Insight]Behörighetsuppsättning i[!DNL Salesforce]**: Administratörer kan ge [!DNL Sales Insight] åtkomst till en begränsad uppsättning personer på användarnivå i stället för på profilnivå via behörighetsgruppen Marketo App, som ingår i [!DNL Sales Insight] [!DNL Salesforce] -paketet.

* **Min uppdatering av Marketo sida vid sida - [!DNL Sales Insight] Åtgärder**: Marketo-administratörer (och de användare de utser) kan nu snabbt navigera till sin [!DNL Sales Insight] Actions-instans via en ny [!DNL Sales Insight] Actions tile som finns på My Marketo-sidan.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **[!DNL Salesforce]API-uppdatering**: I version [!DNL Salesforce] sommar 22 stöds inte längre API-versioner 21-30 av [!DNL Salesforce]. I den här Marketo Engage-versionen har alla [!DNL Sales Connect]-begäranden som använder äldre API-versioner uppdaterats så att de hålls i en version som stöds. Klicka [!DNL Salesforce]här[ om du vill ha fullständig information om ](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"} API-pensionsplaner.

## API-förbättringar {#api-enhancements}

* **Nya filtreringsfunktioner för API:t för programmedlemsextraheringen**: Filtrera efter programmedlemskapsstatus, updatedAt, cadence eller slut på innehåll för att förfina den extraherade datauppsättningen.

* **Förbättring av API:t för extrahering av gruppprogrammedlem**: Ange upp till 10 program när jobb skapas för att förbättra genomströmningen.

## Meddelanden {#announcements}

* **Borttagning av Forms - Forms 1.0, lead Capture/save endpoint och no-script-versioner av formulär**: Stödet för Forms 1.0-resurser kommer att tas bort helt från Marketo Engage i oktober 2022. Alla befintliga Forms 1.0-resurser kommer inte längre att fungera. Marketo Engage-formulär kräver att JavaScript laddas på landningssidor och webbplatser.

**_Webbseminarium om produktreleaser_**

[Juni och augusti 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
