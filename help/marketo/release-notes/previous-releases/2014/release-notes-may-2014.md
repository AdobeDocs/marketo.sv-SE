---
unique-page-id: 2951044
description: Versionsinformation -maj 2014 - Marketo Docs - produktdokumentation
title: Versionsinformation -maj 2014
exl-id: c7b5b2c1-ea3d-483b-8a65-c4d6313bfe31
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Versionsinformation: maj 2014 {#release-notes-may}

Följande funktioner ingår i majversionen 2014. Kontrollera om det finns funktioner i Marketo Edition. Kom tillbaka efter releasen och hitta länkar till detaljerade kunskapsbasartiklar för varje funktion!

## Ta bort Workspace {#delete-workspace}

Nu kan du [ta bort en oanvänd arbetsyta](/help/marketo/product-docs/administration/workspaces-and-person-partitions/delete-a-workspace.md). Flytta alla resurser till en annan arbetsyta innan du försöker ta bort arbetsytan.

## Schemalägg första omgången {#schedule-first-cast}

I engagemangsprogram kan du schemalägga datumet för den [första omgången som ska köras](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md). Ange till exempel att cadence ska vara varannan vecka och välj datumet för den första sändningen.

![](assets/image2014-9-22-11-3a57-3a36.png)

![](assets/image2014-9-22-11-3a57-3a54.png)

## Förbättrade engagemangsprogram {#enhanced-engagement-programs}

Nu får alla flera program, strömmar och kommunikationsbegränsningar.

## Länkspårning i textmeddelanden {#link-tracking-in-text-emails}

[Lägg till dubbla hakparenteser](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-tracked-links-to-a-text-email.md) runt URL:er i textversionen av dina e-postmeddelanden för att ange när länkar ska konverteras till omdirigerade Marketo-spårningslänkar

>[!NOTE]
>
>**Exempel**
>
>`[[https://www.marketo.com]]`

Som standard spåras inga länkar i textversionen av e-postmeddelanden. Lägg till den här nya syntaxen för att ange när en länk ska konverteras till en spårningslänk. Beteendet för HTML-länkar ändras inte.  Så här lägger du till spårade länkar i e-postmeddelanden:

* **HTML-version:** Infoga bara länken. Den spåras som standard.
* **Textversion:** Ange URL:en omgiven av dubbla hakparenteser.

Så här lägger du till ej spårade länkar i e-postmeddelanden:

* **HTML-version:** Infoga länken och lägg till klassen&quot;mktNoTrack&quot; i länken.
* **Textversion:** Ange bara webbadressen. Den spåras inte som standard.

![](assets/image2014-9-22-12-3a1-3a34.png)

## Länka markering i exempelmeddelanden {#link-markup-in-sample-emails}

Se hur länkarna fungerar i e-postmeddelanden i förväg. Exempelmejl visar nu länkar exakt som de skulle se ut för era leads. Förhandsgranska vilka länkar som har konverterats till spårningslänkar, så får du en bättre uppfattning om hur meddelandet faktiskt kommer att visas för mottagarna.

## [!UICONTROL Abort Campaign] {#abort-campaign}

Bli inte panikslagen! Om du upptäcker ett misstag kan du använda den nya knappen [Avbryt kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md) för att omedelbart stoppa kampanjer i deras spår. Du får ett meddelande som visar hur många leads som var under behandling i varje flödessteg när kampanjen stoppades.

## [!UICONTROL Sales Insight] på japanska, portugisiska och spanska {#sales-insight-in-japanese-portuguese-and-spanish}

Hämta den senaste versionen av [!UICONTROL Sales Insight] från AppExchange så att dina japanska, portugisiska och spanska säljare kan visa [!UICONTROL Sales Insight]-innehåll på sitt språk.

![](assets/image2014-9-22-12-3a2-3a12.png)

## Programstatus och lyckad tidsram i programmedlemskapsanalys {#program-status-and-success-timeframe-in-program-membership-analysis}

Visa hur många [medlemmar som finns i varje programstatus](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/build-a-program-membership-analysis-report-that-lists-leads.md) och när de har ändrats till respektive status, inklusive datumet när de uppnådde Programstatus.

## A/B-testa e-postmeddelanden i [!UICONTROL Email Analysis] {#a-b-test-emails-in-email-analysis}

Rapportera om var och en av dina [A/B-testvarianter](/help/marketo/product-docs/reporting/revenue-cycle-analytics/email-analysis/build-an-email-analysis-report-that-shows-program-information.md) i [!UICONTROL Email Analysis].

## Ändringar i Analytics-paketering {#analytics-packaging-changes}

Inkomstcykeln Modeler och Success Path Analyzer ingår nu i MA Standard Edition.

## Information om mobilplattform {#mobile-platform-info}

[Segmentera och utlösa](/help/marketo/product-docs/reporting/basic-reporting/report-activity/build-a-people-performance-report-with-mobile-platform-columns.md) av leads som öppnas och klickar på e-postmeddelanden från deras mobila enheter.
