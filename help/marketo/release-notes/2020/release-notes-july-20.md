---
unique-page-id: 45416698
description: Versionsinformation -juli 20 - Marketo Docs - produktdokumentation
title: Versionsinformation -juli 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Versionsinformation: 20 juli {#release-notes-july}

Följande funktioner finns i versionen från 20 juli. Se om det finns funktioner i din Marketo-utgåva.

>[!AVAILABILITY]
>
>Observera att objekt med en stjärna ( ![(stjärna)](assets/yellow-star.png)) kan behöva köpa ett värdetillägg beroende på vilket paket du använder. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa_** utgåvorFöljande funktioner kommer att släppas den 31  **juli 2020**.

## Administration {#administration}

* **[&quot;Används av&quot;-export i fälthantering](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Administratörer kan nu exportera alla resurslänkar som används av för ett markerat fält till en CSV-fil. Den här förbättringen kan hjälpa både administratörer och icke-administratörer att rensa bort oanvända fält. Dessutom kan resurser nu öppnas på en ny webbläsarflik eller i ett nytt fönster.

## Kontobaserad marknadsföring {#account-based-marketing}

![(stjärna)](assets/yellow-star.png)

* **Uppdaterat användargränssnitt för kontoprofilering**: Förenkla framtagningen av din kontolista i kontoprofilering med smidiga steg på en enda skärm.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

* **Forms-tjänst**: Vi introducerar starkare syntaxvalidering av formulärfält och möjlighet att blockera vanliga robotmönster med nya funktioner för säkra domäner för landningssidor. Genom att blockera robotmönster kan du minska antalet inskickade skräppostformulär och förbättra databaskvaliteten.

>[!NOTE]
>
>Fullständig utrullning av förbättrad syntaxvalidering av formulärfält har skjutits upp till efter vår Jan 2021-utgåva.

* **URI-storleksgräns** för utökat tillgångs-API: Storleksgränsen för URI ökas från 8 kB till 65 kB innan parametern &quot;_method&quot; tas bort. När du utför långa frågesträngar kommer den här storleksökningen att göra det enklare att skicka data. Borttagningen av parametern&quot;_method&quot; ingår i en kommande säkerhetsuppgradering.

## Sales Insight {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Säljannonsering aktiverad för kunder med icke-inbyggd Salesforce CRM Integration](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  (beta)**: Marketo Engage-kunder med icke-ursprungliga Salesforce CRM-integreringar kan nu använda Sales Insight för att hjälpa sina säljteam att förstå, prioritera och interagera med de mest engagerade leads och möjligheter som möjliggör smart försäljning och snabbare avtal.

## Säljanslutning {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **[Förbättrat tvåpartsmedgivande för försäljningssamtal:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Administratörer har nu större kontroll över konfigurationen för samtalsinspelning. [Aktivera ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) inspelning av samtal utan att äventyra efterlevnaden av tvåpartslagen. Automatisera meddelandet om det samtal som spelas in och aktivera ljudklipp som ska spelas upp före samtalet.

<br> 

## Meddelanden och borttagningar {#announcements-deprecations}

* **Ta bort parameter för resurs-API &quot;_method&quot;**: Efter september 2020 kommer Resurs-API-slutpunkter inte längre att acceptera &quot;_method&quot; för att skicka Query Parameters i en POST för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränserna för tillgångs-API:er från 8 kB till 65 kB.
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: I den här versionen av Munchkin JavaScript Client, version 159, kommer vi att börja ta bort Munchkin Associate Lead-metoden. Om den anropas får du ett varningsmeddelande om att metoden kommer att tas bort i en framtida version. När metoden tagits bort kommer den inte längre att fungera och försök att använda den kommer att misslyckas. Marketo Engage-kunder som nyligen har använt den här metoden får ett separat meddelande om hur de använder den.
* **Stöd för Internet Explorer**: Som tidigare meddelats upphör Marketo Engage-stödet för Internet Explorer 11 den 31  **juli 2020**. Vi kommer att fortsätta att stödja Google Chrome, Mozilla Firefox, Apple Safari och Microsoft Edge.
* **Standardupplevelse** för Sky: Alternativet för administratörer och användare att ange Marketo Sky som standardupplevelse kommer att tas bort i den här versionen som förberedelse för en uppdatering av den primära användarupplevelsen. Mer information om uppdateringen av den primära upplevelsen, som planeras senare i år, kommer i juli. Användare som har angett Marketo Sky som standardupplevelse, eller som har beviljats åtkomst till Marketo Sky, kan fortsätta få åtkomst till Marketo Sky från en panel på startsidan för My Marketo.
* **Stöd** för Microsoft EdgeHTML (ej Chromium): Marketo Engage kommer inte längre att ha stöd för EdgeHTML-versioner av Microsoft Edge i slutet av 2020. Från och med 1 januari 2021 har vi bara stöd för den senaste Chromium-versionen av Microsoft Edge.
