---
unique-page-id: 15695924
description: Rankning och justering av kontoprofilering - Marketo Docs - Produktdokumentation
title: Rankning och justering av kontoprofilering
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Rankning och justering för kontoprofilering {#account-profiling-ranking-and-tuning}

Kontoprofilering identifierar din Ideal Customer Profile (ICP), rangordnar företag i din databas baserat på ICP och lägger till ICP Indicator-data till konton som befordrats som namngivna konton.

## Modellresultat {#model-results}

Resultaten visar alla dina kända konton uppdelade efter grad. A är av högsta klass, D är den lägsta.

![](assets/results.png)

Även om det är valfritt rekommenderar vi att du markerar kryssrutan Automatiskt befordra eftersom du då sparar mycket tid. Men om du vill gå igenom varje konto och [lägga till dem manuellt](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md#discover-crm-accounts) lämnar du bara rutan avmarkerad.

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

**Indikatorkategorier**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Regelefterlevnad</strong></td> 
   <td> 
    <div>
      Certifieringar, regelefterlevnadsrelaterade positioner/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Operationer</strong></td> 
   <td> 
    <div>
      Driftsrelaterade positioner/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      HR- eller löneprogramvara, HR-relaterade befattningar/anställning.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Teknik</strong></td> 
   <td> 
    <div>
      Teknik, ramverk, ingenjörsrelaterade positioner/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Försäljning</strong></td> 
   <td> 
    <div>
      Lösningar och programvara för försäljning, försäljningsrelaterade positioner/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Återgivning</strong></td> 
   <td> 
    <div>
      Avfallsindikatorer. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Maskinvaru- och programvarulösningar, tekniker, IT-relaterade befattningar/anställning.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ekonomi</strong></td> 
   <td> 
    <div>
      Ekonomisk programvara, finansiella tjänster/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marknadsföring</strong></td> 
   <td> 
    <div>
      Marknadsföringsteknologier och programvara, marknadsrelaterade befattningar/anställning. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Företag</strong></td> 
   <td> 
    <div>
      Forbes eller Inc listings eller Business Partnership. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Kundupplevelser och relationer</strong></td> 
   <td> 
    <div>
      Kundframgångar och kundrelationer befattningar/anställning.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Håll pekaren över verktygstipsen om du vill se en beskrivning av varje kolumn.

![](assets/tool-tip.png)

Klicka på listrutan Lägg till ICP-indikator för att infoga ytterligare indikatorer i modellen.

![](assets/add-icp.png)

Om du markerar rutan Exportera kan du se ICP-indikatorn på sidan med namngivna kontouppgifter, och du kan använda den valda ICP-indikatorn som begränsningar i [filter för namngivna konton](/help/marketo/product-docs/account-based-marketing/engage/account-filters.md).

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
