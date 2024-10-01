---
description: Salesforce Sync Backlog Metrics - Marketo Docs - produktdokumentation
title: Salesforce Sync Backlog Metrics
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: a9ed4a7e2247a26b376bde64bb1cfd6db2833822
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Salesforce Sync Backlog Metrics  {#salesforce-sync-backlog-metrics}

Synkroniseringens eftersläpning representerar poster som väntar på synkronisering från Salesforce till Marketo Engage, och vice versa. Om du ser till att eftersläpningen är under kontroll kommer synkroniseringen att gå smidigt och i rätt tid.

>[!NOTE]
>
>Eftersläpningen täcker antalet väntande synkroniseringsuppdateringar på båda sidor och inte de som utförs av synkroniseringsflödessteg som [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} eller [Synkronisera person till Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}.

## Åtkomst {#how-to-access}

1. Gå till området **Admin** i Marketo Engage.

   SCREENSHOT

1. Välj **Salesforce**.

   SCREENSHOT

## Synkronisera eftersläpning {#sync-backlog-trend}

Trenden för eftersläpning återspeglar förändringar i eftersläpningar som registrerats under de senaste fem dagarna. Eftersläpningen visas i ett 4-timmars tidsintervall som sträcker sig över 5 dagar. Därför kommer diagrammet att visa 6 intervall per dag gånger 5 dagar, vilket motsvarar 30 intervall.

Eftersläpning observeras vid ett visst 4-timmars tidsintervall på x-axeln. Det här värdet gäller för alla objekt som är synkroniserade. Detta är det totala antalet eftersläpningar i Salesforce och Marketo Engage som väntar på att synkroniseras.

SCREENSHOT

## Synkronisera dataflöde och eftersläpning {#sync-throughput-and-backlog}

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
    <td>Uppskattning av den tid som krävs för att synkronisera eftersläpningen per objekttyp. Beräknas som "Synkronisera eftersläpning/medel-poster synkroniserade per timme".</td>
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

## Vad orsakar synkronisering av eftersläpningar {#what-causes-sync-backlogs}

Oavsett om uppdateringen görs på Marketo Engage eller CRM-sidan kommer den att utlösa att posten synkroniseras igen för att uppdatera informationen på andra sidan genom den vanliga synkroniseringscykeln mellan Marketo Engage och CRM. När en uppdatering görs av en post i Salesforce genereras en tidsstämpel för systemändring, som kallas SysModStamp. Detta medför att en ändring som ska synkroniseras köas.

När en stor mängd uppdateringar görs (till exempel när ett fältvärde ändras) ändras många poster, vilket ger nya SysModStamps. Ett stort antal personregisteruppdateringar måste sedan synkroniseras igen mellan Marketo Engage och CRM, vilket ibland skapar en tillfällig eftersläpning.

## Bästa tillvägagångssätt för hantering av eftersläpningar i synkronisering {#best-practices-for-managing-sync-backlogs}

**Fält under synkronisering**: Kontrollera att endast de fält som är under synkronisering är de som behöver synkroniseras. Ändringar av fält ökar synkroniseringens eftersläpning och fält med lägre prioritet kan stoppa eller göra att viktigare fält under synkronisering blir långsammare. Gå till [Marketo Engage Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} om du vill ta bort fält som är synkroniserade.

**Känsliga fält**: Vissa fält kan uppdateras ofta (t.ex. valutafält som kan ändras). Granska om dessa behöver synkroniseras eller om fälten måste utformas på ett annat sätt.

**Anpassade objekt**: Granska regelbundet anpassade objekt under synkronisering och ta bort objekt som inte längre behöver synkroniseras.

**Aktiviteter**: Kontrollera om det finns några aktiviteter under synkroniseringen som kan tas bort från synkroniseringen.

**Schemalägg massuppdateringar under icke-kritiska timmar**: Granska dina datasynkroniseringsmönster för att identifiera icke-kritiska perioder. Se om det går att schemalägga större uppdateringar under dessa icke-kritiska perioder.

Om du följer alla de bästa metoderna ovan och fortfarande har betydande eftersläpningar kontaktar du [Marketo Engage Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
