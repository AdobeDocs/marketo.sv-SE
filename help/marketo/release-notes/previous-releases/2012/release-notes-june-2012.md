---
unique-page-id: 2951114
description: Versionsinformation -juni 2012 - Marketo Docs - produktdokumentation
title: Versionsinformation -juni 2012
exl-id: c22eda86-da7a-4c76-9cea-1ce23ff0f3e8
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Versionsinformation: juni 2012 {#release-notes-june}

## Förbättringar av Marketo Lead Management {#marketo-lead-management-enhancements}

### Byt namn {#rename}

Du kan byta namn på smarta listor, statiska listor och kampanjer. Om du använder dessa resurser i filter, utlösare eller flöden uppdateras även namnet automatiskt där. Du har alltid kunnat byta namn på e-post, formulär och mappar.

Och som bonus har vi förbättrat möjligheten att ange och visa beskrivningstext för resurser.

![](assets/image2014-9-23-10-3a23-3a10.png)

## Importera fältmappning {#import-field-mapping}

Vi har gjort det mycket enklare att importera en lista till Marketo! Under importprocessen kan du mappa namnet på Marketo-fältet till kolumnrubriknamnet i importfilen. I [!UICONTROL Admin] kan du dessutom konfigurera aliasnamn som mappas till fältnamnet i Marketo, så att användarna alltid väljer rätt fält.

När du fortsätter att importera och mappa fält kommer Marketo att komma ihåg och visa mappningarna under importen för att underlätta användningen. Och för att göra livet ännu enklare kan du klicka på rubriken Exempelvärde för att se de olika värden som skulle fylla i fältet. Detta hjälper dig att mappa rätt fält varje gång!

![](assets/image2014-9-23-10-3a23-3a27.png)

## [!UICONTROL Summary] sida för smarta listor och statiska listor {#summary-page-for-smart-lists-and-static-lists}

Har du någonsin undrat var listorna används? Eller vem skapade listan eller senast ändrade den? Den nya sammanfattningssidan som finns på smarta listor och statiska listor innehåller dessa viktiga detaljer.

![](assets/image2014-9-23-10-3a23-3a40.png)

På de befintliga sammanfattningssidorna för program och kampanj har vi även lagt till informationen Skapad den/Användare och Senast ändrad den/Användare!

![](assets/image2014-9-23-10-3a23-3a54.png)

## [!UICONTROL Used By] för Assets {#used-by-for-assets}

En ny flik har lagts till på resursens [!UICONTROL Summary] sidor, som kallas [!UICONTROL Used By]!

![](assets/image2014-9-23-10-3a24-3a5.png)

Exempel: [!UICONTROL Used By] för statiska listor

## Stödlinjer för landningssida {#landing-page-gridlines}

Med stödlinjerna för landningssidor blir det mycket enklare att justera text, grafik och formulär på landningssidan. Slå på och av den för en viss landningssida och justera även bredden mellan linjerna!

![](assets/image2014-9-23-10-3a24-3a19.png)

![](assets/image2014-9-23-10-3a24-3a33.png)

## Leads blockerade från utskick {#leads-blocked-from-mailings}

När du schemalägger en kampanj kan du klicka på länken för att se en lista över leads som har blockerats från ditt utskick.

![](assets/image2014-9-23-10-3a24-3a51.png)

## [!UICONTROL Wait] steg - Leadtoken och Min token {#wait-step-lead-token-and-my-token}

I maj-versionen har vi lagt till avancerade alternativ i flödessteget [!UICONTROL Wait]. Med dessa ändringar kan du ange en arbetsdag, ett datum och en tid. I den här versionen har vi lagt till möjligheten att använda en token i väntesteget. Du kan till exempel använda `{{lead.Birthday}}` för att skicka ett e-postmeddelande på sin födelsedag eller använda `{{my.Event Date}}` för att skicka en slutgiltig påminnelse för webbinariet.

![](assets/image2014-9-23-10-3a25-3a57.png)

## [!UICONTROL View] som [!UICONTROL Thumbnails] i Design Studio {#view-as-thumbnails-in-design-studio}

Byt vy från en lista med bilder till en miniatyrbildsvy!

![](assets/image2014-9-23-10-3a26-3a13.png)

Obs! Från och med den här versionen gäller inte den tidigare sorteringen i stödraster för smarta listor för nästa smarta lista som du visar. Om du t.ex. sorterar en smart lista efter företagsnamn sorteras inte nästa smarta lista som visas i det här fältet automatiskt.

Påminnelse: Uppgradering av e-postprestandarapport pågår!

## Förbättringar i Marketo Revenue Cycle Analytics {#marketo-revenue-cycle-analytics-enhancements}

### Nya mått i analys av affärsmöjligheter i programmet  {#new-metrics-in-program-opportunity-analysis}

Ni kan nu få insikter om det genomsnittliga antalet marknadsföringsåtgärder innan ni skapar eller stänger nya möjligheter, samt om det genomsnittliga värdet av en marknadsföringskontakt.

![](assets/image2014-9-23-10-3a26-3a30.png)

![](assets/image2014-9-23-10-3a26-3a41.png)

## Visa flera diagram {#displaying-multi-charts}

Med funktionen för flera diagram kan du visa flera diagram i en enda rapport om intäktscykler i Explorer. Du kan till exempel använda den här funktionen när du vill visa samma data för olika månader. Den här funktionen förhindrar också att du behöver skapa separata filter och rapporter.

![](assets/image2014-9-23-10-3a27-3a41.png)

## Typ av värmestödrasterdiagram  {#heat-grid-chart-type}

Värmestödraster gör det möjligt att visualisera data så att ni kan identifiera mönster för marknadsföringens resultat. Den här visualiseringstypen färgkodar dina resultat så att du kan visa komplexa affärsanalyser i en lättbegriplig visualisering.

![](assets/image2014-9-23-10-3a28-3a21.png)

## Typ av punktdiagram  {#scatter-chart-type}

Punktdiagram hjälper dig att visualisera data i flera dimensioner i ett diagram. Den här visualiseringstypen ritar en bubbla i ett diagram baserat på de attribut som används. Du kan sedan använda ett mått för att färgkoda bubblan och/eller använda ett mått för att ange bubblans storlek.

![](assets/image2014-9-23-10-3a29-3a7.png)
