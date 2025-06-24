---
unique-page-id: 2951103
description: Versionsinformation -februari 2013 - Marketo Docs - produktdokumentation
title: Versionsinformation - februari 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Versionsinformation: februari 2013 {#release-notes-february}

Februariversionen innehåller en mycket begärd funktion, stöd för [!DNL Apple Safari] och andra små förbättringar.

## Officiell support för [!DNL Apple Safari] {#official-support-for-apple-safari}

De senaste versionerna av [!DNL Apple Safari] för Mac och [!DNL Windows] stöds fullt ut för användning med Marketo Lead Management. Obs! [!DNL Safari] på iOS är inte helt kompatibelt.

## Förbättringar av webbhooks {#webhooks-enhancements}

Webhooks har förbättrats till escape-tokens i URL/nyttolast och kan även uppdatera Marketo lead-fält genom att tolka XML/JSON-svar från tredjepartssystem (inte tillgängligt i [!DNL Spark SMB Edition]).

## Uppdaterad API-slutpunkt för SOAP {#updated-soap-api-endpoint}

Den rekommenderade SOAP API-slutpunkten har uppdaterats, vilket visas i [!UICONTROL Admin] -> SOAP API. Uppdatera dina samtal för att använda den nya slutpunkten. API-anrop till den gamla slutpunkten är inaktuella, men kommer att fortsätta att fungera. (SOAP API är inte tillgängligt i [!DNL Spark SMB Edition])

## Mobilstöd för [!DNL Facebook] flikar {#mobile-support-for-facebook-tabs}

[!DNL Facebook] flikar som publiceras från Marketo identifierar mobila enheter och dirigerar dem till en landningssida. Detta säkerställer att användaren får rätt innehåll på mobila enheter där [!DNL Facebook] flikar inte stöds (tillgängliga i [!DNL Spark], [!DNL Standard], [!DNL Select SMB Editions] och [!DNL Marketo Social Marketing]).

## Kommer snart: Stöd för flera modeller {#coming-soon-support-for-multiple-models}

Vi lägger grunden för att stödja flera olika intäktscykelmodeller, som vi röstade på bästis för RCA i gemenskapen, i en framtida release. I den här versionen kommer du att märka några ändringar, bland annat [Smart List-filter och Lägg till alternativ i Flödessteg](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md), som stöder valet av modell och scen. Vi flyttar även fälten Leadintäktsstadium och Leadintäktscykelmodell från fliken Smart List Lead grid.
