---
unique-page-id: 2951103
description: Versionsinformation -februari 2013 - Marketo Docs - produktdokumentation
title: Versionsinformation - februari 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Versionsinformation: Februari 2013 {#release-notes-february}

Februariversionen innehåller en efterfrågad funktion, stöd för Apple Safari och andra små förbättringar.

## Officiellt stöd för Apple Safari {#official-support-for-apple-safari}

De senaste versionerna av Apple Safari för Mac och Windows stöds fullt ut för användning med Marketo Lead Management. Obs! Safari på iOS är inte helt kompatibelt.

## Förbättringar av webbhooks {#webhooks-enhancements}

Webhooks har förbättrats så att tokens i URL/nyttolast kan undvikas och Marketo lead-fält kan också uppdateras genom att XML/JSON-svar från tredjepartssystem analyseras (ej tillgängligt i Spark SMB Edition).

## SOAP API-slutpunkt har uppdaterats {#updated-soap-api-endpoint}

Den önskade SOAP API-slutpunkten har uppdaterats, vilket visas i Admin -> SOAP API. Uppdatera dina samtal för att använda den nya slutpunkten. API-anrop till den gamla slutpunkten är inaktuella, men kommer att fortsätta att fungera. (SOAP API är inte tillgängligt i Spark SMB Edition)

## Mobilstöd för Facebook Tabs {#mobile-support-for-facebook-tabs}

Facebook-flikar som publiceras från Marketo upptäcker mobila enheter och dirigerar dem till en landningssida. Detta säkerställer att användaren får rätt innehåll på mobila enheter där Facebook-flikar inte stöds (finns i Spark, Standard, Select SMB Editions och Marketo Social Marketing).

## Kommer snart: Stöd för flera modeller {#coming-soon-support-for-multiple-models}

Vi lägger grunden för att stödja flera olika intäktscykelmodeller, som vi röstade på bästis för RCA i gemenskapen, i en framtida release. I den här versionen kommer du att märka några ändringar, bland annat [Smarta listfilter och Lägg till alternativ i Flödessteg](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) för att stödja valet av modell och scen. Vi flyttar även fälten Leadintäktsstadium och Leadintäktscykelmodell från fliken Smart List Lead grid.
