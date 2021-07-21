---
unique-page-id: 42762514
description: Instrumentpanelsfunktion - översikt - Marketo Docs - produktdokumentation
title: Översikt över funktionen Insikt i instrumentpanelen
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
source-git-commit: 6679e1e0bdb53d3f330c15415a5fbe38f61d28d2
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 0%

---

# Översikt över funktionen Insikt i instrumentpanelen {#insights-dashboard-feature-overview}

Läs mer om de funktioner som finns på kontrollpanelen för försäljningsinsikter.

>[!PREREQUISITES]
>
>Du måste ha det senaste MSI SFDC-paketet och [konfigurationen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/one.png)

## Kontaktlayout {#contact-layout}

**Hastighetsrutnät för engagemang**

* Detta smarta rutnät innehåller intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna
* Användaren kan välja aktiviteten &quot;Visa konto&quot;, vilket lagrar alla intressanta ögonblick på kontonivå, e-post och webbaktivitet i kontaktvyn
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Översikt och detaljgranskning av engagemang**

* Granska aktivitetskort för intressanta ögonblick, e-post och webbaktivitet
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang**

Fliken E-postkampanjer:

* Inkluderar kampanjer som är en del av e-postprogram eller standardprogram som planeras inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett förhandsvisningsalternativ. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filtren innehåller &quot;Sök&quot; och &quot;Datumintervall&quot;

![](assets/three.png)

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller&quot;Sök&quot;,&quot;Visa endast inbjudna händelser&quot; och&quot;Datumintervall&quot;

![](assets/two.png)

## Leadlayout {#lead-layout}

**Hastighetsrutnät för engagemang**

* Detta smarta rutnät innehåller intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts
* Funktionen Visa kontoaktivitet är inte tillgänglig för leads eftersom den inte är en del av något konto i Salesforce förrän den konverteras till en kontakt

**Översikt och detaljgranskning av engagemang**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang:**

Fliken E-postkampanjer:

* Inkluderar kampanjer som är en del av e-postprogram eller standardprogram som planeras inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett förhandsvisningsalternativ. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filtren innehåller &quot;Sök&quot; och &quot;Datumintervall&quot;

![](assets/five.png)

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller&quot;Sök&quot;,&quot;Visa endast inbjudna händelser&quot; och&quot;Datumintervall&quot;

![](assets/four.png)

## Kontolayout {#account-layout}

**Hastighetsrutnät för engagemang**

* Detta smarta rutnät innehåller Intressanta stunder, e-post och webbaktivitet de senaste 90 dagarna för alla kontakter i kontot
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Översikt och detaljgranskning av engagemang**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet, inklusive kontaktnamn
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang**

Fliken E-postkampanjer:

* Inkluderar kampanjer som är en del av e-postprogram eller standardprogram som planeras inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett förhandsvisningsalternativ. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filtren innehåller &quot;Sök&quot; och &quot;Datumintervall&quot;

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller&quot;Sök&quot;,&quot;Visa endast inbjudna händelser&quot; och&quot;Datumintervall&quot;

## Affärsmöjlighet {#opportunity-layout}

**Hastighetsrutnät för engagemang**

* Detta smarta rutnät innehåller Intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna för alla kontakter i affärsmöjligheten
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Översikt och detaljgranskning av engagemang**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet, inklusive kontaktnamn
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande fliken E-postkampanjer och** evenemangE-postkampanjer:

* Inkluderar kampanjer som är en del av e-postprogram eller standardprogram som planeras inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett förhandsvisningsalternativ. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filtren innehåller &quot;Sök&quot; och &quot;Datumintervall&quot;

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller&quot;Sök&quot;,&quot;Visa endast inbjudna händelser&quot; och&quot;Datumintervall&quot;
