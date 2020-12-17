---
unique-page-id: 45416698
description: Versionsinformation -juli 20 - Marketo Docs - Produktdokumentation
title: Versionsinformation -juli 20
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Versionsinformation: 20 juli {#release-notes-july}

Följande funktioner finns i versionen från 20 juli. Se om din Marketo-utgåva har funktioner tillgängliga.

>[!NOTE]
>
>**Tillgänglighet**
>
>Observera att objekt med en stjärna ( ![(stjärna)](assets/star-yellow.svg)) kan behöva köpa ett värdetillägg beroende på vilket paket du använder. Kontakta din Marketo Engage-representant om du vill veta mer.

***Kvartalsvisa*** utgåvorFöljande funktioner kommer att släppas den 31  **juli 2020**.

## Administration {#administration}

* ** [&quot;Används av&quot;-export i fälthantering](https://docs.marketo.com/x/hAK1Ag)**: Administratörer kan nu exportera alla resurslänkar som används av för ett markerat fält till en CSV-fil. Den här förbättringen kan hjälpa både administratörer och icke-administratörer att rensa bort oanvända fält. Dessutom kan resurser nu öppnas på en ny webbläsarflik eller i ett nytt fönster.

**Kontobaserad marknadsföring ![(stjärna)](assets/star-yellow.svg)

**

* **Uppdaterat användargränssnitt för kontoprofilering: **Förenkla framtagningen av målkontolistor i kontoprofilering med smidiga steg - allt på en enda skärm.

<br> 

**

***Frigör under hela kvartalet***

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

* **Forms-tjänst: **Vi introducerar starkare syntaxvalidering av formulärfält och möjlighet att blockera vanliga robotmönster med nya funktioner för säkra domäner för landningssidor. Genom att blockera robotmönster kan du minska antalet inskickade skräppostformulär och förbättra databaskvaliteten.
* **URI-storleksgräns** för utökat tillgångs-API: Storleksgränsen för URI ökas från 8 kB till 65 kB innan parametern &quot;_method&quot; tas bort. När du utför långa frågesträngar kommer den här storleksökningen att göra det enklare att skicka data. Borttagningen av parametern&quot;_method&quot; ingår i en kommande säkerhetsuppgradering.

**Sales Insight ![(star)](assets/star-yellow.svg)

**

* ** [Sales Insight Enabled for Customers with Non-Native Salesforce CRM Integration](https://docs.marketo.com/x/pQK1Ag)(Beta)**: Marketo Engage-kunder med icke-ursprungliga Salesforce CRM-integreringar kan nu använda Sales Insight för att hjälpa sina säljteam att förstå, prioritera och interagera med de mest engagerade leads och möjligheter som möjliggör smart försäljning och snabbare avtal.

**Sales Connect ![(star)](assets/star-yellow.svg)

**

* ** [Förbättrat tvåpartsmedgivande för försäljningssamtal:](https://docs.marketo.com/x/dgC1Ag)** Administratörer har nu större kontroll över konfigurationen för samtalsinspelning. [Aktivera ](https://docs.marketo.com/x/dAC1Ag) inspelning av samtal utan att äventyra efterlevnaden av tvåpartslagen. Automatisera meddelandet om det samtal som spelas in och aktivera ljudklipp som ska spelas upp före samtalet.

<br> 

## Meddelanden och borttagningar {#announcements-deprecations}

* **Ta bort parameter för resurs-API &quot;_method&quot;**: Efter september 2020 kommer Resurs-API-slutpunkter inte längre att acceptera &quot;_method&quot; för att skicka Query Parameters i en POST för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränserna för tillgångs-API:er från 8 kB till 65 kB.
* ** [Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: I den här versionen av Munchkin JavaScript Client, version 159, kommer vi att börja ta bort Munchkin Associate Lead-metoden. Om den anropas får du ett varningsmeddelande om att metoden kommer att tas bort i en framtida version. När metoden tagits bort kommer den inte längre att fungera och försök att använda den kommer att misslyckas. Marketo Engage-kunder som nyligen har använt den här metoden får ett separat meddelande om hur de använder den.
* **Stöd för Internet Explorer**: Som tidigare meddelats upphör Marketo Engage-stödet för Internet Explorer 11 den 31  **juli 2020**. Vi kommer att fortsätta att stödja Google Chrome, Mozilla Firefox, Apple Safari och Microsoft Edge.

* **Standardupplevelse** för Sky: Alternativet för administratörer och användare att ange Marketo Sky som standardupplevelse kommer att tas bort i den här versionen som förberedelse för en uppdatering av den primära användarupplevelsen. Mer information om uppdateringen av den primära upplevelsen, som planeras senare i år, kommer i juli. Användare som har angett Marketo Sky som standardupplevelse, eller som har beviljats åtkomst till Marketo Sky, kan fortsätta få åtkomst till Marketo Sky från en panel på startsidan för My Marketo.
* **Stöd** för Microsoft EdgeHTML (ej Chromium): Marketo Engage kommer inte längre att ha stöd för EdgeHTML-versioner av Microsoft Edge i slutet av 2020. Från och med 1 januari 2021 har vi bara stöd för den senaste Chromium-versionen av Microsoft Edge.

