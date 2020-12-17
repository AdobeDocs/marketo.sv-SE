---
unique-page-id: 15695924
description: Rankning och justering av kontoprofilering - Marketo Docs - Produktdokumentation
title: Rankning och justering av kontoprofilering
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Rankning och justering för kontoprofilering {#account-profiling-ranking-and-tuning}

Kontoprofilering identifierar din Ideal Customer Profile (ICP), rangordnar företag i din databas baserat på ICP och lägger till ICP Indicator-data till konton som befordrats som namngivna konton.

## Modellresultat {#model-results}

Resultaten visar alla dina kända konton uppdelade efter grad. A är av högsta klass, D är den lägsta.

![](assets/results.png)

Även om det är valfritt rekommenderar vi att du markerar kryssrutan Automatiskt befordra eftersom du då sparar mycket tid. Men om du vill gå igenom varje konto och [lägga till dem manuellt](http://docs.marketo.com/display/DOCS/Discover+Accounts#DiscoverAccounts-DiscoverCRMAccounts) lämnar du bara rutan avmarkerad.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Rankning</strong></td> 
   <td> 
    <div>
      Kontorangordningen baseras på kundprofilen Ideal. A är bäst, D är minst lämpligt. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensitet</strong></td> 
   <td> 
    <div>
      Uppskattad ökning av konverteringsgraden jämfört med ett icke-ICP-baserat urval av konton. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Konton (%)</strong></td> 
   <td> 
    <div>
      Procentandel konton i modellindata som har den här rangordningen. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% av modellbasen</strong></td> 
   <td> 
    <div>
      Procent av konton i modellbasen som har den här rangordningen. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Modelljustering {#model-tuning}

Klicka på knappen Justera modell på fliken Modell.

![](assets/two.png)

Det finns flera flikar att välja mellan, vilket möjliggör en djupgående anpassning.

![](assets/tuning-page.png)

Indikatorkategorier

| **Regelefterlevnad** | Certifieringar, regelefterlevnadsrelaterade positioner/anställning. |
|---|---|
| **Operationer** | Driftsrelaterade positioner/anställning. |
| **HR** | HR- eller löneprogramvara, HR-relaterade befattningar/anställning. |
| **Teknik** | Teknik, ramverk, ingenjörsrelaterade positioner/anställning. |
| **Försäljning** | Lösningar och programvara för försäljning, försäljningsrelaterade positioner/anställning. |
| **Återgivning** | Avfallsindikatorer. |
| **IT** | Maskinvaru- och programvarulösningar, tekniker, IT-relaterade befattningar/anställning. |
| **Ekonomi** | Ekonomisk programvara, finansiella tjänster/anställning. |
| **Marknadsföring** | Marknadsföringsteknologier och programvara, marknadsrelaterade befattningar/anställning. |
| **Företag** | Forbes eller Inc listings eller Business Partnership. |
| **Kundupplevelser och relationer** | Kundframgångar och kundrelationer befattningar/anställning. |

Håll pekaren över verktygstipsen om du vill se en beskrivning av varje kolumn.

![](assets/tool-tip.png)

Klicka på listrutan Lägg till ICP-indikator för att infoga ytterligare indikatorer i modellen.

![](assets/add-icp.png)

Om du markerar rutan Exportera kan du se ICP-indikatorn på sidan med namngivna kontouppgifter, och du kan använda den valda ICP-indikatorn som begränsningar i [filter för namngivna konton](http://docs.marketo.com/display/DOCS/Account+Filters).

![](assets/export.png)

>[!NOTE]
>
>ICP-indikatorer inkluderas som begränsningar i **Medlem i namngivet konto** Filter och utlösare.

Indikatorns viktning styr den prioritetsnivå som varje indikator får i din modell.

![](assets/weightage.png)

Klicka på Uppdatera modell för att ändringarna ska börja gälla.

![](assets/refresh-button.png)

När du är klar med att justera modellen (efter att du har uppdaterat den) går du tillbaka till fliken Modellresultat och klickar på **Spara och använd rangordning**.

![](assets/ranks.png)

