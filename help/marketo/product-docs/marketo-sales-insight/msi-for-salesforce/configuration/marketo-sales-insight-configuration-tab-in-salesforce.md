---
unique-page-id: 42762322
description: Marketo Sales Insight Configuration tab in Salesforce - Marketo Docs - Product Documentation
title: Marketo Sales Insight Configuration tab in Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Marketo Sales Insight Configuration tab in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Driftsinställningar {#operational-settings}

Du måste ha konfigurerat detta för att kunna börja använda Sales Insight i SFDC.

![](assets/one.png)

* MSI använder både Soap- och Rest-API
* Sidan Sales Insight i ditt Marketo-konto kommer att ha två motsvarande paneler med autentiseringsuppgifterna Soap och Rest API som du kan kopiera och klistra in här
* Programmerings- och återställnings-API har olika tidsgränser som du kan ange utifrån organisationens behov. Den högsta tillåtna tiden är 120 sekunder
* Inaktiverar instrumentpanelen för insikter: Du kan ta bort Rest API-autentiseringsuppgifter och endast använda Soap API. Om du gör det inaktiveras fliken Insights Dashboard på alla MSI-visualforce-paneler

## MSI-konfiguration {#msi-configuration}

Konfigurationer gäller för alla MSI-användare och är inte specifika för profiler.

**Inställningar för Marketo-flik**

* Felsökningsläge för bästa val
* Dölj som standard - Det alternativ du väljer här är det antal dagar ett bästa val döljs på fliken Bästa val i Marketo när du klickar på Dölj-ikonen
* Kontaktstatusfält - Det alternativ du väljer här är det värde som fylls i i kolumnen Statusrubrik på fliken Bästa val i Marketo
* Flikinställningar - Alla fem flikarna är tillgängliga som standard. Du kan välja tabbordning på den globala sidan Markto

**Visualforce-sidinställningar**

* Listrutan Aktivera åtgärd:

   * Möjlighet att dölja Send Marketo-e-post från listrutan i lead- och kontakt-MSI-layout
   * Möjlighet att dölja Lägg till i Marketo Campaign-alternativen från listrutan i lead- och kontaktelayout för MSI

* Kommande event: Möjlighet att visa inbjudna händelser, alla händelser till användare eller helt dölja den här fliken
* Kommande kampanjer: Möjlighet att visa alla e-postkampanjer eller dölja den här fliken helt
* Flikinställningar - Alla fem flikarna är tillgängliga som standard. Alla fem flikarna är som standard tillgängliga. Du kan välja tabbordning på panelen Försäljningsinsikter. Samma order gäller för all layout (Lead, Contact, Account, Opportunity)

![](assets/two.png)

**Gränser**

* Aktivitet (Intressant stund, Webbaktivitet, E-post) är som standard inställd på 1 000. E-postkampanjer och händelser är som standard inställda på 200
* Om du får problem med tidsgränsen i din organisation kan du minska den

## Återställ Marketo Sales Insight {#reset-marketo-sales-insight}

Om du väljer att göra det raderas alla konfigurationer i SFDC och de kan inte återställas. Du måste konfigurera om allt igen.

![](assets/three.png)

