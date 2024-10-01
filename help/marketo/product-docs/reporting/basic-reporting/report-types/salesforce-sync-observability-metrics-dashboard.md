---
description: Salesforce Sync Observability Metrics Dashboard - Marketo Docs - Produktdokumentation
title: Salesforce Sync Observability Metrics Dashboard
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 2457f0f51c6365c29a040e908678e81517327de5
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Salesforce Sync Backlog Metrics  {#salesforce-sync-backlog-metrics}

Granska dina synkroniseringsprestandaströmmar och synkronisera eftersläpningar med den här instrumentpanelen.

## Synkronisera dataflöde och eftersläpning {#sync-throughput-and-backlog}

1. Gå till Admin i Marketo Engage.

   SCREENSHOT

1. Välj Salesforce.

   SCREENSHOT

Statistiken visar genomströmning och eftersläpningsstatus för varje objekttyp som är synkroniserad under de senaste 24 timmarna. Objekttyperna omfattar alla objekt som är synkroniserade, inklusive Lead, Kontakt, Konto, Möjlighet, Kampanj, Användare och Anpassade objekt. Dataflödesstatistiken uppdateras automatiskt var 15:e minut, men du kan uppdatera manuellt med hjälp av uppdateringsikonen. Eftersläpningen hämtas varje timme.

>[!NOTE]
>
>Statistiken uppdateras på rullande basis, inte efter kalenderdag.

SCREENSHOT

<table><thead>
  <tr>
    <th>Fält</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Maximalt antal synkroniserade poster / hr</td>
    <td>Det högsta antalet poster som synkroniseras per timme (maximalt dataflöde) som observerats under de senaste 24 timmarna för objekttypen. 24-timmarsperioden är full av tid, inte kalenderdagen.</td>
  </tr>
  <tr>
    <td>Minsta antal synkroniserade poster / hr</td>
    <td>Det minsta antalet poster som synkroniseras per timme (lägsta dataflöde) som observerats under de senaste 24 timmarna för objekttypen. 24-timmarsperioden är full av tid, inte kalenderdagen.</td>
  </tr>
  <tr>
    <td>Genomsnittligt antal synkroniserade poster/timme</td>
    <td>Det genomsnittliga antalet poster som synkroniserats per timme (lägsta dataflöde) som observerats under de senaste 24 timmarna för objekttypen. 24-timmarsperioden är full av tid, inte kalenderdagen. Detta beräknas som det totala antalet poster som synkroniserats under de senaste 24 timmarna.</td>
  </tr>
  <tr>
    <td>Synkronisera eftersläpning</td>
    <td>Eftersläpningen med poster som väntar på synkronisering för objekttypen. Det är den totala summan för eftersläpande synkronisering i båda riktningarna (från Salesforce till Marketo Engage och vice versa). Eftersläpningen från Salesforce hämtas med ett API-anrop till Salesforce, och eftersläpningen från Marketo Engage beräknas med hjälp av statistik från ändringsdataloggen. Detta beräknas varje timme. De två följande fälten i den här tabellen anger när eftersläpningen senast beräknades och nästa schema för beräkning.</td>
  </tr>
  <tr>
    <td>Uppskattad eftersläpning (tid)</td>
    <td>Uppskattning av den tid som krävs för att synkronisera eftersläpningen per objekttyp. Beräknas som synkroniserade poster för Synkronisera eftersläpning/genomsnitt per timme.</td>
  </tr>
  <tr>
    <td>Senast hämtad eftersläpning</td>
    <td>Tidpunkten för den senaste eftersläpningsberäkningen.</td>
  </tr>
  <tr>
    <td>Eftersläpning vid nästa hämtning</td>
    <td>Tidpunkten för nästa eftersläpningsberäkning.</td>
  </tr>
  <tr>
    <td>Status för eftersläpning</td>
    <td>Detta visar om eftersläpningen har växt de senaste sex timmarna. Den betraktas som "Växande" om den nuvarande eftersläpningen är större än den som registrerats för 6 timmar sedan. I annat fall visas det som"Normal". Detta är avsett att visa om synkroniseringens genomströmning håller på att ta igen eftersläpningen.</td>
  </tr>
</tbody></table>

## Trend för eftersläpning {#backlog-trend}

Trenden för eftersläpning återspeglar förändringar i eftersläpningar som registrerats under de senaste fem dagarna. Eftersläpningen visas i ett 4-timmars tidsintervall som sträcker sig över 5 dagar. Därför kommer diagrammet att visa 6 intervall per dag gånger 5 dagar, vilket motsvarar 30 intervall.

Eftersläpning observeras vid ett visst 4-timmars tidsintervall på x-axeln. Det här värdet gäller för alla objekt som är synkroniserade. Detta är det totala antalet eftersläpningar i Salesforce och Marketo Engage som väntar på att synkroniseras.

SCREENSHOT
