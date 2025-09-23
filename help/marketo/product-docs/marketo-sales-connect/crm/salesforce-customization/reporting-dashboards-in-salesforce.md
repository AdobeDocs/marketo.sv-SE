---
unique-page-id: 14352464
description: Rapportera instrumentpaneler i Salesforce - Marketo Docs - produktdokumentation
title: Rapportera instrumentpaneler i Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Rapportera instrumentpaneler i Salesforce {#reporting-dashboards-in-salesforce}

Lär dig hur du konfigurerar instrumentpaneler nedan.

## Öppna och klicka på Rapport {#open-and-click-report}

1. Välj posttypen **[!UICONTROL Tasks and Events]**.
1. Definiera rapportparametrarna baserat på den önskade tidsramen och hierarkistrukturen.
1. Lägg till ett filter för att ta bort interna e-postmeddelanden som loggats på [!DNL Salesforce] (t.ex. företag/konto är inte lika med Marketo).
1. Välj rapportformatet **[!UICONTROL Summary]**.
1. Lägg till fälten Ämne, Tilldelad och Marketo Sales Click/Marketo Sales Viewed i rapporten.
1. Dubbelklicka på **[!UICONTROL Add Formula]** i fältfönstret.
1. Lägg till ett namn i formeln, välj **[!UICONTROL Percent]** i formatet och välj **[!UICONTROL Grouping 1]**.
1. Välj **[!UICONTROL Marketo Sales Clicked/Marketo Sales Viewed]** och sedan **[!UICONTROL Sum]** i sammanfattningsfälten.
1. Lägg till ett divisionstecken i formeln och välj sedan **[!UICONTROL Record Count]** i sammanfattningsfälten - _Spara som_.

## Resultatrapport för mall {#template-performance-report}

1. Anpassa rapporten Öppna och klicka för att inkludera följande fält - _Spara som_.

## Mallvolymrapport {#template-volume-report}

1. Ändra mallprestandarapporten och inkludera filtret&quot;Marketo-försäljningsmall är inte lika med tom&quot;.
1. Ta bort fältet Marketo Sales Click - _Save As_.

## Rapport över trendkonton {#trending-accounts-report}

1. Välj aktiviteter med posttypen Konton.
1. Konfigurera rapportparametrar och fält enligt nedan - _Spara som_.
