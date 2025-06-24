---
unique-page-id: 45416698
description: Versionsinformation -juli 20 - Marketo Docs - produktdokumentation
title: Versionsinformation -juli 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Versionsinformation: 20 juli {#release-notes-july}

Följande funktioner finns i versionen från 20 juli. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Observera att objekt med en stjärna ( ![(stjärna)](assets/yellow-star.png)) kan behöva köpa ett värdetillägg, beroende på vilket paket du använder. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa utgåvor_** Följande funktioner kommer att släppas den **31 juli 2020**.

## Administrering {#administration}

* **[&quot;Används av&quot;-export i fälthantering](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Administratörer kan nu exportera alla resurslänkar som används av för ett markerat fält till en CSV-fil. Den här förbättringen kan hjälpa både administratörer och icke-administratörer att rensa bort oanvända fält. Dessutom kan resurser nu öppnas på en ny webbläsarflik eller i ett nytt fönster.

## Account-Based Marketing {#account-based-marketing}

![(stjärna)](assets/yellow-star.png)

* **Uppdaterat användargränssnitt för kontoprofilering**: Förenkla skapandet av målkontolistan i kontoprofileringen med smidiga steg på en enda skärm.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

* **Forms-tjänst**: Vi introducerar starkare syntaxvalidering av formulärfält och möjlighet att blockera vanliga robotmönster med nya säkra domäner för Landing Pages-funktioner. Genom att blockera robotmönster kan du minska antalet inskickade skräppostformulär och förbättra databaskvaliteten.

>[!NOTE]
>
>Fullständig utrullning av förbättrad syntaxvalidering av formulärfält har skjutits upp till efter vår Jan 2021-utgåva.

* **Större URI-storleksgräns för resurs-API**: Storleksgränsen för URI (Universal Resource Identifier) ökas från 8 kB till 65 kB innan parametern &quot;_method&quot; tas bort. När du utför långa frågesträngar kommer den här storleksökningen att göra det enklare att skicka data. Borttagningen av parametern&quot;_method&quot; ingår i en kommande säkerhetsuppgradering.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Aktiverad för kunder med icke-inbyggd [!DNL Salesforce] CRM-integrering](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: Marketo Engage-kunder med icke-ursprungliga [!DNL Salesforce] CRM-integreringar kan nu använda [!DNL Sales Insight] för att hjälpa sina säljteam att förstå, prioritera och interagera med de mest engagerade leads och möjligheter som möjliggör smart försäljning och snabbare erbjudanden.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **[Förbättrat tvåpartsmedgivande för försäljningssamtal:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Administratörer har nu större kontroll över konfigurationen för samtalsinspelning. [Aktivera samtalsinspelningar](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) med vetskap om att du följer tvåpartslagen. Automatisera meddelandet om det samtal som spelas in och aktivera ljudklipp som ska spelas upp före samtalet.

<br> 

## Meddelanden och borttagningar {#announcements-deprecations}

* **Resurs-API:t &quot;_method&quot; - parameterborttagning**: Efter september 2020 kommer Resurs-API-slutpunkter inte längre acceptera &quot;_method&quot; för att skicka frågeparametrar i ett POST-brödtext för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränserna för tillgångs-API:er från 8 kB till 65 kB.
* **[[!DNL Munchkin] Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: I den här versionen av Munchkin JavaScript Client, version 159, börjar borttagningen av metoden [!DNL Munchkin] Associate Lead. Om den anropas får du ett varningsmeddelande om att metoden kommer att tas bort i en framtida version. När metoden tagits bort kommer den inte längre att fungera och försök att använda den kommer att misslyckas. Marketo Engage-kunder som nyligen har använt den här metoden får ett separat meddelande om hur de använder den.
* **Stöd för Internet Explorer**: Som tidigare meddelats upphör Marketo Engage support för Internet Explorer 11 den **31 juli 2020**. Vi fortsätter att stödja [!DNL Google Chrome], [!DNL Mozilla Firefox],[!DNL  Apple Safari] och [!DNL Microsoft Edge].
* **Sky Default Experience**: Alternativet för administratörer eller användare att ange [!DNL Marketo Sky] som standardupplevelse kommer att tas bort i den här versionen som förberedelse för en uppdatering av den primära användarupplevelsen. Mer information om uppdateringen av den primära upplevelsen, som planeras senare i år, kommer att finnas tillgänglig i juli. Användare som har angett [!DNL Marketo Sky] som standardupplevelse, eller som har beviljats åtkomst till [!DNL Marketo Sky], kan fortsätta få åtkomst till [!DNL Marketo Sky] från en panel på startsidan för My Marketo.
* **Stöd för EdgeHTML (ej Chromium) [!DNL Microsoft Edge]**: Marketo Engage stöder inte längre EdgeHTML-versioner av Microsoft Edge i slutet av 2020. Från och med 1 januari 2021 stöder vi endast den senaste Chromium-versionen av Microsoft Edge.
