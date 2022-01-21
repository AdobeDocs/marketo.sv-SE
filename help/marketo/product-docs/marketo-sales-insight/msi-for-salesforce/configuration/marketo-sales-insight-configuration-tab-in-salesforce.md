---
unique-page-id: 42762322
description: Marketo Sales Insight Configuration Tab in Salesforce - Marketo Docs - Product Documentation
title: Marketo Sales Insight Configuration tab in Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Marketo Sales Insight Configuration tab in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Driftsinställningar {#operational-settings}

Du måste ha konfigurerat detta för att kunna börja använda Sales Insight i SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI använder både Soap- och Rest-API
* Sidan Sales Insight i ditt Marketo-konto kommer att ha två motsvarande paneler med autentiseringsuppgifterna Soap och Rest API som du kan kopiera och klistra in här
* Programmerings- och återställnings-API har olika tidsgränser som du kan ange utifrån organisationens behov. Den högsta tillåtna tiden är 120 sekunder
* Inaktiverar instrumentpanelen för insikter: Du kan ta bort Rest API-autentiseringsuppgifter och endast använda Soap API. Om du gör det inaktiveras fliken Insights Dashboard på alla MSI-visualforce-paneler

## MSI-konfiguration {#msi-configuration}

Konfigurationer gäller för alla MSI-användare och är inte specifika för profiler.

**Visualforce-sidinställningar**

* Listrutan Aktivera åtgärd:
   * Möjlighet att dölja Skicka Marketo-e-post i listrutan Lead och Contact MSI Layout
   * Möjlighet att dölja Lägg till i Marketo Campaign-alternativen från listrutan i lead- och Kontakta MSI-layout
* Kommande event: Möjlighet att visa inbjudna händelser, alla händelser till användare eller helt dölja den här fliken
* Kommande kampanjer: Möjlighet att visa alla e-postkampanjer eller dölja den här fliken helt
* Läs in kommande kampanjer och evenemang: Möjlighet att minska antalet Rest API-anrop som görs av användare genom att placera händelser och kampanjer på en flik bakom knappen Läs in kommande objekt på begäran
* Flikinställningar: Alla fem flikarna är som standard tillgängliga. Du kan välja tabbordning på panelen Sales Insight. Samma order gäller för alla layouter (Lead, Contact, Account, Opportunity)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Marketo Global Tab**

* RSS-flöde aktiverat: När det här alternativet är aktiverat kan MSI-användare visa sin lead-feed i en RSS-feed (utöver lead-feed i Salesforce). RSS-matningen fungerar bara om funktionen &quot;Token Expiration&quot; är inaktiverad. Den här inställningen styrs på sidan Marketo Sales Insight Admin.
* Felsökningsläge för bästa val
* Dölj som standard: Det alternativ du väljer här är det antal dagar som det bästa valet döljs på fliken Bästa val i Marketo när du klickar på ikonen Dölj
* Kontaktstatusfält: Det alternativ du väljer här är det värde som anges i kolumnen Statusrubrik på fliken Bästa val i Marketo
* Inställningar för Live-feed: Alternativet att endast visa Live-feed (i panelerna Lead, Kontakt, Konto och säljprojekt samt på Marketo-sidan Global), endast Lead-feed (på Marketo Global Page) eller både Live- och Lead-feed
* Flikinställningar: Alla fem flikarna är som standard tillgängliga. Du kan välja tabbordning på Marketo globala sida

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Gränser**

* Aktivitet (Intressant stund, Webbaktivitet, E-post) är som standard inställd på 1 000. E-postkampanjer och händelser är som standard inställda på 200
* Om du får problem med tidsgränsen i din organisation kan du minska den

**Åtgärdsinställningar**

* Skicka e-post från Marketo: Om du aktiverar detta får alla användare av Sales Insight tillgång till e-post från lead-, kontakt-, konto-, säljprojektspanelerna och fliken Bästa val (gruppåtgärder och internt engagemang)
* Lägg till i Marketo Campaign: Om du aktiverar detta får alla användare av Sales Insight tillgång till kampanjer från panelerna Lead, Contact, Account, Opportunity och Best Bets (massåtgärder och internt engagemang).

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Återställ Marketo Sales Insight {#reset-marketo-sales-insight}

Om du väljer att göra det raderas alla konfigurationer i SFDC och de kan inte återställas. Du måste konfigurera om allt igen.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!MORELIKETHIS]
>
>[Konfigurera Sales Insight för ditt team](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
