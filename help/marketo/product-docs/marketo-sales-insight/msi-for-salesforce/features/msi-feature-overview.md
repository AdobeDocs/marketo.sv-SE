---
unique-page-id: 37356893
description: MSI Feature Overview - Marketo Docs - produktdokumentation
title: Översikt över MSI-funktioner
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 0%

---

# Översikt över MSI-funktioner {#msi-feature-overview}

MSI har följande funktioner tillgängliga i [!DNL Salesforce] Lightning och Classic.

>[!NOTE]
>
>Kontrollera att webbläsarens zoom är inställd på högst 125 % när du använder Windows och 150 % på Mac för att se alla tillgängliga data.

## Visualforce-panel {#visualforce-panel}

MSI Visualforce-panelen innehåller följande funktioner:

* Tabbar

   * [Instrumentpanel för insikter](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Intressanta ögonblick
   * Webbaktivitet
   * E-post
   * Poäng

* Åtgärder

   * Lägg till i Marketo Campaign
   * Skicka e-post till Marketo
   * Lägg till/ta bort från bevakad lista

* Stjärnor och flamman

## Leadlayout {#lead-layout}

Visualforce-sidor:

* Lead - Med det här alternativet kan du klicka på&quot;Gå till fullständig lista&quot;. Då skickas du till en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig lista för lead - Innehåller inte alternativet Gå till fullständig lista
* Lead Mobile - synlig i Salesforce mobilprogram
* Leadkontakt Bridge - Visar MSI-panelen för den kontakt du har lagt till i fältet för MSI-kontakt-ID

Fält:

* Senaste intressanta stund
* Senaste intressanta datum
* Senaste intressanta tillfälle
* Senaste intressanta stund Source
* Typ av senaste intressanta stund
* Senaste Marketo-aktivitet per försäljning
* Senaste Marketo-engagemang från försäljning
* Relativa poäng
* Relativt poängvärde
* Akut
* Värde för nödsituationer
* Visa i Marketo - Klicka på det här fältet för att öppna en icke-redigerbar vy av leadet i Marketo. Innehåller: Leadinformation, Företagsinformation, SFDC Lead Info, SFDC anpassade fält, Aktivitetslogg
* MSI-kontakt-ID - Lägg till en Salesforce-kontakt i det här fältet och ta med panelen &quot;Lead Contact Bridge&quot; i leadlayouten för att se kontaktens MSI-panel

## Kontaktlayout {#contact-layout}

Visualforce-sidor:

* Kontakt - innehåller alternativ för att klicka på&quot;Gå till fullständig lista&quot;, du kommer att få en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig kontaktlista - innehåller inte alternativet Gå till fullständig lista
* Kontakt Mobile - synlig i Salesforce mobilprogram
* Lägg till på kontaktsidan för Marketo Campaign - Funktionen Lägg till i Marketo Campaign är tillgänglig på den här panelen

Fält:

* Senaste intressanta stund
* Senaste intressanta datum
* Senaste intressanta tillfälle
* Senaste intressanta stund Source
* Typ av senaste intressanta stund
* Senaste Marketo-aktivitet per försäljning
* Relativa poäng
* Relativt poängvärde
* Akut
* Värde för nödsituationer
* Visa i Marketo - Klicka på det här fältet för att öppna en icke-redigerbar vy av leadet i Marketo. Innehåller: Leadinformation, Företagsinformation, SFDC Lead Info, SFDC anpassade fält, Aktivitetslogg
* MKto Lead Score
* [!DNL Sales Insight] - Öppnar sidan med fullständig kontaktlista

## Kontolayout {#account-layout}

Visualforce-sidor:

* Konto - innehåller alternativ för att klicka på&quot;Gå till fullständig lista&quot;. Du kommer att få en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig kontolista - innehåller inte alternativet Gå till fullständig lista
* Kontomobilt - synligt i Salesforce mobilprogram

Fält:

* [!DNL Sales Insight] - Öppnar sidan med fullständig kontaktlista

Funktionsmakron:

* Lägg till i Marketo Campaign
* Skicka e-post till Marketo
* Lägg till/ta bort från bevakad lista

Följande funktioner är **inte tillgängliga** på sidan Kontolayout:

* Stjärnor och flamman

## Affärsmöjlighet {#opportunity-layout}

Visualforce-sidor:

* Möjlighet - innehåller ett alternativ för att klicka på&quot;Gå till fullständig lista&quot;, du kommer att skickas till en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig lista för affärsmöjlighet - innehåller inte alternativet Gå till fullständig lista
* Mobil möjlighet - synlig i Salesforce mobilapplikation

Fält:

* [!DNL Sales Insight] - Öppnar sidan med fullständig kontaktlista
* Marketo säljprojektsanalys - Öppnar analys av säljprojektspåverkan i Marketo

Funktionsmakron:

* Lägg till i Marketo Campaign
* Skicka e-post till Marketo
* Lägg till/ta bort från bevakad lista

Följande funktioner är **inte tillgängliga** på sidan för säljprojektslayout:

* Stjärnor och flamman

## Lead- och kontaktlistevy (massåtgärder) {#lead-and-contact-list-view-bulk-actions}

[!DNL Salesforce Lightning]: Lägg till i bevakningslistan, Lägg till i Marketo Campaign och Skicka Marketo e-postgruppknappar i vyn Lead- och kontaktlista.

[!DNL Salesforce Classic]: Lägg till i bevakningslistan, Lägg till i Marketo Campaign och Skicka Marketo e-postgruppknappar i vyn Lead- och kontaktlista.

## Marketo Tab {#marketo-tab}

* [!DNL Best Bets]

   * Innehåller möjlighet att skapa och redigera vyer. Möjlighet att dölja bästa val beroende på konfigurationen av alternativet &quot;Dölj som standard&quot; på Marketo konfigurationssida
   * Kolumner - Namn, Konto, Senaste intressanta stund, Statusrubrik, Engagement (Stars &amp; Flames), Dölj

* Min bevakningslista

   * Innehåller funktioner för att skapa och redigera vyer
   * Kolumner - Namn, Konto, Senaste intressanta stund, Statusrubrik, Engagement (Stars &amp; Flames), Ta bort

* Webbaktivitet

   * Innehåller funktioner för att skapa och redigera vyer, tidsramfilter
   * Kolumn - sidvy, namn, konto, senaste besök

* Anonym webbaktivitet

   * Innehåller funktioner för att skapa och redigera vyer, tidsramfilter
   * Kolumner - sidvy, företag, senaste besök, forskning (öppnar företagets LinkedIn-sida)

* Min e-postadress

   * Innehåller funktioner för att skapa och redigera vyer
   * Kolumner - Namn, Konto, Ämne, Datum, Öppna, Klicka

* Leadfeed - Innehåller möjlighet att prenumerera på intressanta ögonblick, RSS-flöde på konfigurationssidan måste vara aktiverat för att den här funktionen ska kunna användas

   * Lead/kontakt som hade denna intressanta stund
   * Typ av intressant stund (webb, e-post eller milstolpe) och beskrivning
   * Kontonamn
   * Tid då det här intressanta ögonblicket inträffade
   * Prenumerationsalternativ för att få e-postmeddelanden för den här typen av händelse
   * Ikonen med hög prioritet för att visa den här personen är ett Bästa val

## Fliken Konfiguration för [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

* Driftsinställningar: Inkluderar de Soap &amp; Rest API-autentiseringsuppgifter som krävs för att konfigurera MSI i SFDC
* MSI-konfiguration: Innehåller konfiguration av Marketo-fliken och MSI visualforce-panelen
* Återställ [!DNL Marketo Sales Insight]: Innehåller möjlighet att ta bort alla konfigurationer

>[!MORELIKETHIS]
>
>[[!DNL Marketo Sales Insight] Fliken Konfiguration i [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## [!DNL Sales Insight] prestandarapporter {#sales-insight-performance-reports}

Visa prestanda för e-postmeddelanden som skickas via [!DNL Salesforce], [!DNL Microsoft Dynamics] eller en Gmail- eller [!DNL Outlook]-plugin

## MSI för mobiler {#msi-for-mobile}

MSI-funktioner stöds i [!DNL Salesforce]-mobilprogram

## Språkstöd {#language-support}

[!DNL Marketo Sales Insight] lagras efter språk. Om du vill att det ska fungera för mer än ett språk måste du ange inloggningsuppgifterna separat för varje språk.

>[!NOTE]
>
>* En kontakt/lead måste finnas i standardpartitionen för att kunna läggas till i bevakningslistan.
>
>* MSI-paketet [!DNL Salesforce] stöder inte anpassad vy med beroende fält.
