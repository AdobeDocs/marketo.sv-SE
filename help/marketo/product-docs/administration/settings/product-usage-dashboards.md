---
description: Kontrollpaneler för produktanvändning - Marketo Docs - produktdokumentation
title: Kontrollpaneler för produktanvändning
hide: true
hidefromtoc: true
feature: Administration
source-git-commit: f3bc58c0d65e8110c5366269fdb4abf817370aee
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Kontrollpaneler för produktanvändning {#product-usage-dashboards}

På Marketo Engage produktkontrollpaneler kan du visa produkt- och plattformsanvändning mot vissa begränsningar eller eftersläpning av data via indata, användning mot daglig kvot och nyckelvärden för en prenumeration. Infrastruktur tilldelas för att tillhandahålla prestandagränser definierade för produktnivåer för särskilda attribut. Vissa av dessa begränsningar, som API-användning, är avtalsbegränsningar som köpts som en del av ditt paket eller din produktnivå.

## Åtkomst {#how-to-access}

1. Klicka på **Admin** i Marketo Engage.

   ![](assets/product-usage-dashboards-1.png)

1. I trädet till vänster rullar du nedåt och väljer **Kontrollpaneler för produktanvändning**.

   ![](assets/product-usage-dashboards-2.png)

## Kontrollpanel för aktivitetsanvändning {#activity-usage-dashboard}

### Genomsnittlig veckoaktivitet {#average-weekly-activities}

Kontrollpanelen för aktivitetsanvändning varje vecka visar antalet aktivitetstyper under en rullande 52-veckorsperiod. Veckoaktiviteter som producerats är en bra indikator på hur mycket marknadsföring du gör i Marketo Engage. Verksamheterna fungerar som en proxy för de olika systemprocesser och spårbara händelser som äger rum inom Marketo.

Aktivitetstyper omfattar både antal aktiviteter som tagits när personer interagerar med marknadsföringshändelser och systembaserade aktiviteter som utlöses av Flow Actions. Exempel på aktiviteter som initierats av en person är när en person öppnar ett e-postmeddelande eller klickar på en länk i ett e-postmeddelande. Ett exempel på systembaserade aktiviteter som utlöses av en Flow-åtgärd är&quot;Skicka till SFDC&quot; när utlösaren initieras. Om du vill visa antalet aktivitetstyper för en viss vecka håller du pekaren över en vecka och visar antalet.

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### Vanliga frågor och svar {#faq}

**Vilka aktivitetstyper räknas?**

Det beror på vilka aktiviteter som ingår i pipeline.

**Ingår både känd och anonym lead-/personaktivitet?**

Endast kända personer/leads.

**Hur ofta uppdateras data?**

Antalet aktiviteter uppdateras varje morgon.

## Aktivitetsdelning {#activity-breakdown}

Här får vi antalet aktiviteter under de senaste sju dagarna baserat på meningsfulla datasegment. Gruppera aktiviteter efter de vanligaste aktivitetstyperna de senaste sju dagarna. Detta kan omfatta kategorier som&quot;Ändra datavärde&quot;,&quot;Lägg till i lista&quot; eller&quot;Skicka e-post&quot;. På så sätt kan du se vilka typer av aktiviteter som sker oftast i systemet. Användning av aktivitetstyp är en nyckelindikator för att fastställa tillväxt eller om optimeringar behövs för att minska användningen.

>[!NOTE]
>
>* Alla uppdelningar nedan är en rullande sjudagarssumma och **inkluderar inte** den aktuella dagen. Så tänk på det som&quot;igår + sex dagar före det&quot;.
>
>* På kontrollpanelen visas endast de 20 viktigaste aktivitetstyperna, medan resten sorteras i en kategori med namnet&quot;Annan&quot;.

![](assets/product-usage-dashboards-4.png){width="800" zoomable="yes"}

Aktivitetsanvändning är en nyckelindikator på hur mycket marknadsföring som bedrivs och hjälper till att visualisera tillväxten mot den nivå som avtalats för produkten. Kontrollpaneler kan också användas som vägledning för att avgöra hur mycket optimering som kan/bör göras genom att reducera antalet fält som uppdateras.

### Efter typ {#by-type}

Gruppera aktiviteter efter de vanligaste aktivitetstyperna de senaste sju dagarna. Detta kan omfatta kategorier som _Ändra datavärde_, _Lägg till i lista_ eller _Skicka e-post_. På så sätt kan du se vilka typer av aktiviteter som sker oftast i Marketo Engage.

### Efter attributet Ändra datavärde {#by-change-data-value-attribute}

_Ändra datavärde_ är den vanligaste aktivitetstypen. Det anger när en del information om en person/lead-post uppdateras. Här grupperar vi de fält som har ändrats oftast så att du kan avgöra vilken information som är användbar för marknadsföringsåtgärderna, om det finns möjligheter att optimera plattformsanvändningen osv.

### Efter kampanj {#by-campaign}

Grupp för vilka kampanjer producerar mest aktiviteter. Detta ger insikter för att se om ni har några särskilt &quot;högljudda&quot; kampanjer som skapar mer aktivitet än nödvändigt. Lär dig snabbt om kampanjer som ska avvecklas, eller kampanjer som gör mer arbete än tänkt.

### Av Source (KOMMER SNART) {#by-source}

Gruppera efter aktiviteternas källa (_CRM-synkronisering_, _Kampanjflödesåtgärd_, _API-överföring_, _Landing Page Form Fill_ osv.). Detta hjälper er att förstå om de flesta av era aktiviteter produceras av marknadsföringsåtgärder, CRM-synkroniseringar eller av personerna/ledarna själva.
