---
unique-page-id: 42762514
description: Instrumentpanelsfunktion - översikt - Marketo Docs - produktdokumentation
title: Översikt över funktionen Insikt i instrumentpanelen
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# Översikt över funktionen Insikt i instrumentpanelen {#insights-dashboard-feature-overview}

Läs mer om de funktioner som är tillgängliga på din [!DNL Sales Insights]-instrumentpanel.

>[!PREREQUISITES]
>
>Du måste ha det senaste MSI SFDC-paketet och [konfigurationen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Kontaktlayout {#contact-layout}

**Hastighetsstödraster för engagemang**

* Detta smarta rutnät innehåller intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna
* Användaren kan välja aktiviteten [!UICONTROL Show Account]. Detta lagrar alla intressanta ögonblick på kontonivå, e-post och webbaktivitet på kontonivån i kontaktvyn
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Fördjupning av engagemang och sammanfattning**

* Granska aktivitetskort för intressanta ögonblick, e-post och webbaktivitet
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang**

fliken E-postkampanjer:

* Inkluderar kampanjer som ingår i e-postprogram eller standardprogram som är schemalagda inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett alternativ för förhandsgranskning. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filter innehåller [!UICONTROL Search] och [!UICONTROL Date Range]

![](assets/insights-dashboard-feature-overview-2.png)

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller [!UICONTROL Search], [!UICONTROL Show only invited events] och [!UICONTROL Date Range]

![](assets/insights-dashboard-feature-overview-3.png)

## Leadlayout {#lead-layout}

**Hastighetsstödraster för engagemang**

* Detta smarta rutnät innehåller intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts
* Funktionen [!UICONTROL Show Account Activity] är inte tillgänglig för leads eftersom den inte är en del av något konto i [!DNL Salesforce] förrän den konverteras till en kontakt

**Fördjupning av engagemang och sammanfattning**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang:**

fliken E-postkampanjer:

* Inkluderar kampanjer som ingår i e-postprogram eller standardprogram som är schemalagda inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett alternativ för förhandsgranskning. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filter innehåller [!UICONTROL Search] och [!UICONTROL Date Range]

![](assets/insights-dashboard-feature-overview-4.png)

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller [!UICONTROL Search], [!UICONTROL Show only invited events] och [!UICONTROL Date Range]

![](assets/insights-dashboard-feature-overview-5.png)

## Kontolayout {#account-layout}

**Hastighetsstödraster för engagemang**

* Detta smarta rutnät innehåller Intressanta stunder, e-post och webbaktivitet de senaste 90 dagarna för alla kontakter i kontot
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Fördjupning av engagemang och sammanfattning**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet, inklusive kontaktnamn
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang**

fliken E-postkampanjer:

* Inkluderar kampanjer som ingår i e-postprogram eller standardprogram som är schemalagda inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett alternativ för förhandsgranskning. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filter innehåller [!UICONTROL Search] och [!UICONTROL Date Range]

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller [!UICONTROL Search], [!UICONTROL Show only invited events] och [!UICONTROL Date Range]

## Affärsmöjlighet {#opportunity-layout}

**Hastighetsstödraster för engagemang**

* Detta smarta rutnät innehåller Intressanta ögonblick, e-post och webbaktivitet de senaste 90 dagarna för alla kontakter i affärsmöjligheten
* Användaren kan markera en viss vecka för att se aktiviteter inom den veckan
* Standardvy: Aktuell vecka har valts

**Fördjupning av engagemang och sammanfattning**

* Detaljerade aktivitetskort för intressanta ögonblick, e-post och webbaktivitet, inklusive kontaktnamn
* Intressanta ögonblick Aktivitetskort - inkluderar prenumerationsalternativ
* E-postaktivitetskort - innehåller alternativ för förhandsgranskning
* Webbaktivitetskort - innehåller möjlighet att klicka på länken
* Veckosammanfattningsfältet visar Intressanta tider, e-post och webbaktivitet för den veckan. Varje ikon går att klicka på och kan användas som filter för att visa specifik aktivitet
* Standardvy: Det här är en lista över aktiviteter i den aktuella vyn

**Kommande e-postkampanjer och evenemang** Fliken E-postkampanjer:

* Inkluderar kampanjer som ingår i e-postprogram eller standardprogram som är schemalagda inom de kommande 90 dagarna
* Inte specifikt för kontakten/leadet (dvs. listan över kampanjer är en allmän lista över alla e-postkampanjer som är schemalagda i Marketo-instansen). Listan över kampanjer för alla lead-, kontakt-, konto- och affärsmöjlighetspaneler blir densamma
* Om kampanjen upprepas mer än tre gånger under de kommande 90 dagarna visas bara de tre efterföljande omgångarna vid en given tidpunkt (liknande beteendet i Marketo)
* Aktivitetsinformationskortet i det här avsnittet har ett alternativ för förhandsgranskning. Om flödet innehåller flera skicka-e-poststeg är alla e-postmeddelanden tillgängliga för förhandsgranskning. Om det finns flera&quot;e-postalternativ&quot; i skicka-e-postflödessteget är standardalternativet tillgängligt för förhandsgranskning
* Filter innehåller [!UICONTROL Search] och [!UICONTROL Date Range]

Fliken Händelse:

* Innehåller schemalagda händelseprogram inom de närmaste 90 dagarna
* Använd filteralternativet för att se alla händelser/inbjudna händelser (baserat på administratörsinställningarna)
* Om du väljer inbjudna händelser visas händelser som en viss kontakt har bjudits in till, tillsammans med medlemskapsstatus
* Om du väljer alla händelser visas en lista över händelser som schemalagts inom de kommande 90 dagarna
* Kortet för aktivitetsinformation i det här avsnittet har förhandsvisningsalternativ
* Filtret innehåller [!UICONTROL Search], [!UICONTROL Show only invited events] och [!UICONTROL Date Range]

>[!NOTE]
>
>Om kontot eller säljprojektet har fler än 800 kontakter visas inga data på instrumentpanelen. Men ni kan gå till enskilda kontakter för att se deras insikter och engagemang. Om ditt konto har fler än 800 kontakter inaktiveras [!UICONTROL Show Account Level Activity].
