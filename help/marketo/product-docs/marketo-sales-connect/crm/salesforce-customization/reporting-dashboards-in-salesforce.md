---
unique-page-id: 14352464
description: Rapportera instrumentpaneler i Salesforce - Marketo Docs - produktdokumentation
title: Rapportera instrumentpaneler i Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Rapportera instrumentpaneler i Salesforce {#reporting-dashboards-in-salesforce}

Lär dig hur du konfigurerar instrumentpaneler nedan.

## Öppna och klicka på Rapport {#open-and-click-report}

1. Välj **Uppgifter och händelser** posttyp.
1. Definiera rapportparametrarna baserat på den önskade tidsramen och hierarkistrukturen.
1. Lägg till ett filter för att ta bort interna e-postmeddelanden som loggats i Salesforce (t.ex. Företag/Konto som inte är lika med Marketo).
1. Välj **Sammanfattning** rapportformat.
1. Lägg till fälten Ämne, Tilldelad och Marketo Sales Click/Marketo Sales Viewed i rapporten.
1. Dubbelklicka på **Lägg till formel** i rutan Fält.
1. Lägg till ett namn i formeln, välj **Procent** i formatet och väljer **Gruppering 1**.
1. Välj **Marketo Sales Click/Marketo Sales Viewed,** sedan **Summa** i sammanfattningsfälten.
1. Lägg till ett divisionstecken i formeln och välj sedan **Antal poster** i sammanfattningsfälten - _Spara som_.

## Resultatrapport för mall {#template-performance-report}

1. Anpassa rapporten Öppna och klicka för att inkludera följande fält - _Spara som_.

## Mallvolymrapport {#template-volume-report}

1. Ändra mallprestandarapporten och inkludera filtret&quot;Marketo-försäljningsmall är inte lika med tom&quot;.
1. Ta bort fältet Marketo Sales Click - _Spara som_.

## Rapport över trendkonton {#trending-accounts-report}

1. Välj aktiviteter med posttypen Konton.
1. Ställ in rapportparametrar och fält enligt nedan - _Spara som_.
