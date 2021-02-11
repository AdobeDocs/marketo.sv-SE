---
unique-page-id: 14352464
description: Rapportera instrumentpaneler i Salesforce - Marketo Docs - Produktdokumentation
title: Rapportera instrumentpaneler i Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Rapportera instrumentpaneler i Salesforce {#reporting-dashboards-in-salesforce}

Lär dig hur du konfigurerar instrumentpaneler nedan.

## Öppna och klicka på Rapport {#open-and-click-report}

1. Välj posttypen **Aktiviteter och händelser**.
1. Definiera rapportparametrarna baserat på den önskade tidsramen och hierarkistrukturen.
1. Lägg till ett filter för att ta bort interna e-postmeddelanden som loggats i Salesforce (t.ex. Företag/Konto som inte är lika med Marketo).
1. Välj rapportformatet **Sammanfattning**.
1. Lägg till fälten Ämne, Tilldelad och Marketo Försäljning klickad/Marketo Försäljning Visad i rapporten.
1. Dubbelklicka på **Lägg till formel** i fältfönstret.
1. Lägg till ett namn i formeln, välj **Procent** i formatet och välj **Gruppera 1**.
1. Välj **Marketo Sales Click/Marketo Sales Viewed,** och **Sum** i sammanfattningsfälten.
1. Lägg till ett divisionstecken i formeln och välj sedan **Antal poster** i sammanfattningsfälten - _Spara som_.

## Resultatrapport för mall {#template-performance-report}

1. Anpassa rapporten Öppna och klicka för att inkludera följande fält - _Spara som_.

## Mallvolymrapport {#template-volume-report}

1. Ändra mallresultatrapporten och inkludera filtret&quot;Marketo Sales Template not equal to blank&quot;.
1. Ta bort fältet Marketo Sales Click - _Spara som_.

## Trendkontorapport {#trending-accounts-report}

1. Välj aktiviteter med posttypen Konton.
1. Konfigurera rapportparametrar och fält enligt nedan - _Spara som_.
