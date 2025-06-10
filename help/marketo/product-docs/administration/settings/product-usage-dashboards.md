---
description: Kontrollpaneler för produktanvändning - Marketo Docs - produktdokumentation
title: Kontrollpaneler för produktanvändning
hide: true
hidefromtoc: true
feature: Administration
exl-id: a0fa5cd0-a61d-4383-88c0-9f2a4b2c717a
source-git-commit: 8a4f0015f99e62127f8b690263fb07de6a0a6e6f
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Kontrollpaneler för produktanvändning {#product-usage-dashboards}

På Marketo Engage kontrollpaneler för produktanvändning kan du visa produkt- och plattformsanvändning mot vissa begränsningar eller eftersläpning av data genom-put, användning mot daglig kvot och nyckeltal i din prenumeration. Infrastruktur tilldelas för att tillhandahålla prestandagränser definierade för produktnivåer för särskilda attribut. Vissa av dessa begränsningar, som API-användning, är avtalsbegränsningar som köpts som en del av ditt paket eller din produktnivå.

## Åtkomst {#how-to-access}

1. Klicka på **Admin** i Marketo Engage.

   ![](assets/product-usage-dashboards-1.png)

1. I trädet till vänster rullar du nedåt och väljer **Kontrollpaneler för produktanvändning**.

   ![](assets/product-usage-dashboards-2.png)

## Kontrollpanel för aktivitetsanvändning {#activity-usage-dashboard}

### Genomsnittlig veckoaktivitet {#average-weekly-activities}

Kontrollpanelen för aktivitetsanvändning varje vecka visar antalet aktivitetstyper under en rullande 52-veckorsperiod. Veckoaktiviteter som producerats är en bra indikator på hur mycket marknadsföring du gör i Marketo Engage. Verksamheterna fungerar som en proxy för de olika systemprocesser och spårbara händelser som äger rum inom Marketo.

Aktivitetstyper omfattar både antal aktiviteter som tagits när personer/leads interagerar med marknadsföringshändelser och systembaserade aktiviteter som utlöses av Flow Actions. Exempel på aktiviteter som initierats av en person är när en mottagare öppnar ett e-postmeddelande som du har skickat till honom eller klickar på en länk i ett e-postmeddelande. Ett exempel på en systembaserad aktivitet som utlöses av en Flow-åtgärd är _Skicka till SFDC_ när utlösaren initieras.

>[!TIP]
>
>Om du vill visa antalet aktivitetstyper för en viss vecka håller du pekaren över önskad vecka så visas antalet.

#### Vanliga frågor och svar {#faq}

**Vilka aktivitetstyper räknas?**

Det beror på vilka aktiviteter som ingår i pipeline.

**Är både känd och anonym person/lead-aktivitet inkluderad?**

Endast kända personer/leads.

**Hur ofta uppdateras data?**

Antalet aktiviteter uppdateras varje morgon.

## Aktivitetsdelning {#activity-breakdown}

Här får vi antalet aktiviteter under de senaste sju dagarna baserat på meningsfulla datasegment. Gruppera aktiviteter efter de vanligaste aktivitetstyperna de senaste sju dagarna. Detta kan omfatta kategorier som _Ändra datavärde_, _Lägg till i lista_ eller _Skicka e-post_. På så sätt kan du se vilka typer av aktiviteter som sker oftast i systemet. Användning av aktivitetstyp är en nyckelindikator för att fastställa tillväxt eller om optimeringar behövs för att minska användningen.

>[!NOTE]
>
>* Alla uppdelningar nedan är en rullande summering på sju dagar och inkluderar **inte** den aktuella dagen. Så tänk på det som&quot;igår + sex dagar före det&quot;.
>
>* På kontrollpanelen visas endast de 20 viktigaste aktivitetstyperna, medan resten sorteras i en kategori med namnet&quot;Annan&quot;.

Aktivitetsanvändningen visar hur mycket marknadsföring som bedrivs och hjälper er att visualisera tillväxten mot den nivå som avtalats för produkten. Kontrollpaneler kan också användas som vägledning för att avgöra hur mycket optimering som kan/bör göras genom att reducera antalet fält som uppdateras.

### Efter typ {#by-type}

Gruppera aktiviteter efter de vanligaste aktivitetstyperna de senaste sju dagarna. Detta kan omfatta kategorier som _Ändra datavärde_, _Lägg till i lista_ eller _Skicka e-post_. På så sätt kan du se vilka typer av aktiviteter som sker oftast på ditt Marketo Engage-konto.

### Efter attributet Ändra datavärde {#by-change-data-value-attribute}

_Ändra datavärde_ är den vanligaste aktivitetstypen. Det anger när en del information om en person/lead-post uppdateras. Här grupperar vi de fält som har ändrats oftast så att du kan avgöra vilken information som är användbar i marknadsföringsåtgärderna, om det finns möjligheter att optimera plattformsanvändningen osv.

### Efter kampanj {#by-campaign}

Grupp för vilka kampanjer producerar mest aktiviteter. På så sätt kan ni se om ni har några särskilt &quot;högljudda&quot; kampanjer som skapar mer aktivitet än nödvändigt. Lär dig snabbt om kampanjer som ska avvecklas, eller kampanjer som gör mer arbete än tänkt.
