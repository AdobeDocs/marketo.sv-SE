---
unique-page-id: 37356893
description: MSI Feature Overview - Marketo Docs - Produktdokumentation
title: Översikt över MSI-funktioner
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---


# MSI-funktionsöversikt {#msi-feature-overview}

MSI har följande funktioner i Salesforce Lightning och Classic.

## Visualforce-panelen {#visualforce-panel}

MSI Visualforce-panelen innehåller följande funktioner:

* Tabbar

   * [Instrumentpanel för insikter](http://docs.marketo.com/x/EoGMAg)
   * Intressant stund
   * Webbaktivitet
   * E-post
   * Poäng

* Åtgärder

   * Lägg till i Marketo Campaign
   * Skicka Marketo-e-post
   * Lägg till/ta bort från bevakad lista

* Stjärnor och flamman

## Leadlayout {#lead-layout}

Visualforce-sidor:

* Lead - Inkluderar alternativet att klicka på&quot;Gå till fullständig lista&quot;, du kommer att få en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig lista för lead - Innehåller inte alternativet Gå till fullständig lista
* Lead Mobile - synlig i Salesforce-mobilprogram
* Lead Contact Bridge - Visar MSI-panelen för den kontakt du har lagt till i fältet för MSI-kontakt-ID

Fält:

* Senaste intressanta stund
* Senaste intressanta datum
* Senaste intressanta tillfälle
* Källa för senaste intressanta stund
* Typ av senaste intressanta stund
* Senaste marknadsföringsaktivitet efter försäljning
* Senaste marknadsföringsåtagande av försäljning
* Relativa poäng
* Relativt poängvärde
* Akut
* Värde för nödsituationer
* Visa i Marketo - Klicka på det här fältet för att öppna en icke-redigerbar vy av leadet i Marketo. Innehåller: Leadinformation, företagsinformation, SFDC-huvudinformation, SFDC-anpassade fält, aktivitetslogg
* MSI-kontakt-ID - Lägg till en Salesforce-kontakt i det här fältet och ta med panelen &quot;Lead Contact Bridge&quot; i leadlayouten för att se kontaktens MSI-panel

## Kontaktlayout {#contact-layout}

Visualforce-sidor:

* Kontakt - innehåller alternativ för att klicka på&quot;Gå till fullständig lista&quot;, du kommer att få en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig kontaktlista - innehåller inte alternativet Gå till fullständig lista
* Kontakt Mobile - synlig i Salesforce-mobilprogram
* Lägg till i Marketo Campaign ContactPage - funktionen Lägg till i Marketo Campaign är tillgänglig i den här panelen

Fält:

* Senaste intressanta stund
* Senaste intressanta datum
* Senaste intressanta tillfälle
* Källa för senaste intressanta stund
* Typ av senaste intressanta stund
* Senaste marknadsföringsaktivitet efter försäljning
* Relativa poäng
* Relativt poängvärde
* Akut
* Värde för nödsituationer
* Visa i Marketo - Klicka på det här fältet för att öppna en icke-redigerbar vy av leadet i Marketo. Innehåller: Leadinformation, företagsinformation, SFDC-huvudinformation, SFDC-anpassade fält, aktivitetslogg
* MKto Lead Score
* Sales Insight - Öppnar hela kontaktlistsidan

## Kontolayout {#account-layout}

Visualforce-sidor:

* Konto - Innehåller alternativ för att klicka på &quot;Gå till fullständig lista&quot;. Du kommer att få en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig kontolista - innehåller inte alternativet Gå till fullständig lista
* Kontomobilt - synligt i Salesforce-mobilprogrammet

Fält:

* Sales Insight - Öppnar hela kontaktlistsidan

Följande funktioner är **inte tillgängliga** på sidan Kontolayout:

* Funktionsmakron: Lägg till i Marketo Campaign, Skicka Marketo-e-post, Lägg till/ta bort från bevakad lista
* Stjärnor och flamman

## Affärsmöjlighetslayout {#opportunity-layout}

Visualforce-sidor:

* Möjlighet - innehåller ett alternativ för att klicka på &quot;Gå till fullständig lista&quot;, du kommer att skickas till en ny flik i Salesforce där MSI-panelen visas i en helsideslayout
* Fullständig lista för affärsmöjlighet - innehåller inte alternativet Gå till fullständig lista
* Mobil möjlighet - synlig i Salesforce-mobilprogram

Fält:

* Sales Insight - Öppnar hela kontaktlistsidan
* Marketo Opportunity Analysis - Öppnar analys av affärsmöjlighet i Marketo

Följande funktioner är **inte tillgängliga** på sidan för säljprojektslayout:

* Funktionsmakron: Lägg till i Marketo Campaign, Skicka Marketo-e-post, Lägg till/ta bort från bevakad lista
* Stjärnor och flamman

## Vyn Lead- och kontaktlista (gruppåtgärder) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning: Lägg till åtgärdsknapparna Lägg till i Marketo Campaign och Skicka till e-postmarknadsföring i grupplistan i Lead- och Kontaktlistvyn.

Salesforce Classic: Lägg till åtgärdsknapparna Lägg till i Marketo Campaign och Skicka till e-post i Bulklistan i Lead- och Kontaktlistvyn.

## Marketo Tab {#marketo-tab}

* Bästa val

   * Innehåller möjlighet att skapa och redigera vyer. Möjlighet att dölja bästa val beroende på konfigurationen av alternativet &quot;Default Hide&quot; på sidan Marketo Configuration
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

## Marketo Sales Insight Configuration Tab {#marketo-sales-insight-configuration-tab}

* Driftsinställningar: Inkluderar de Soap &amp; Rest API-autentiseringsuppgifter som krävs för att konfigurera MSI i SFDC
* MSI-konfiguration: Inkluderar konfiguration av Marketo-fliken och MSI visualforce-panelen
* Återställ Marketo Sales Insight: Innehåller möjlighet att rensa bort alla konfigurationer

>[!MORELIKETHIS]
>
>[Marketo Sales Insight Configuration tab in Salesforce](http://docs.marketo.com/x/UoCMAg)

## Prestandarapporter för Sales Insight {#sales-insight-performance-reports}

Visa prestanda för e-postmeddelanden som skickas via Salesforce, Microsoft Dynamics eller ett Gmail- eller Outlook-plugin-program

## MSI för mobilen {#msi-for-mobile}

MSI-funktioner stöds i Salesforce-mobilprogram

## Språkstöd {#language-support}

Marketo Sales Insight lagras på språk. Om du vill att det ska fungera för mer än ett språk måste du ange inloggningsuppgifterna separat för varje språk.
