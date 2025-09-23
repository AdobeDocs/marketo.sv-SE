---
unique-page-id: 15695924
description: Rankning och justering av kontoprofilering - Marketo Docs - produktdokumentation
title: Rankning och justering av kontoprofilering
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Rankning och justering av kontoprofilering {#account-profiling-ranking-and-tuning}

Kontoprofilering identifierar din Ideal Customer Profile (ICP), rangordnar företag i din databas baserat på ICP och lägger till ICP-indikatordata till konton som marknadsförs som [!UICONTROL Named Accounts].

>[!IMPORTANT]
>
>Från och med 2025 är kontoprofilering inte längre tillgängligt för nya användare. Det fortsätter att fungera för befintliga användare.

## Modellresultat {#model-results}

Resultaten visar alla dina kända konton uppdelade efter grad. A är av högsta klass, D är den lägsta.

![](assets/results.png)

Även om det är valfritt rekommenderar vi att du markerar kryssrutan Automatiskt befordra eftersom du då sparar mycket tid. Men om du vill gå igenom varje konto och [lägga till dem manuellt](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts) lämnar du bara rutan avmarkerad.

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Rankning</span></strong></td>
   <td>
    <div>
      Kontorangordningen baseras på kundprofilen Ideal. A är bäst, D är minst passad.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Propensitet</span></strong></td>
   <td>
    <div>
      Uppskattad ökning av konverteringsgraden jämfört med ett icke-ICP-baserat urval av konton.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Konton (%)</span></strong></td>
   <td>
    <div>
      Procentandel konton i modellindata som har den här rangordningen.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">% av modellbasen</span></strong></td>
   <td>
    <div>
      Procent av konton i modellbasen som har den här rangordningen.
    </div></td>
  </tr>
 </tbody>
</table>

## Modelljustering {#model-tuning}

Klicka på knappen **[!UICONTROL Tune Model]** på fliken Modell.

![](assets/two.png)

Det finns flera flikar att välja mellan, vilket möjliggör en djupgående anpassning.

![](assets/tuning-page.png)

**Indikatorkategorier**

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Regelefterlevnad</span></strong></td>
   <td>
    <div>
      Certifieringar, regelefterlevnadsrelaterade positioner/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Användning</span></strong></td>
   <td>
    <div>
      Driftsrelaterade positioner/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">HR</span></strong></td>
   <td>
    <div>
      HR- eller löneprogramvara, HR-relaterade befattningar/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Teknik</span></strong></td>
   <td>
    <div>
      Teknik, ramverk, ingenjörsrelaterade positioner/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Försäljning</span></strong></td>
   <td>
    <div>
      Lösningar och programvara för försäljning, försäljningsrelaterade positioner/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Återgivning</span></strong></td>
   <td>
    <div>
      Avfallsindikatorer.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">IT</span></strong></td>
   <td>
    <div>
      Maskinvaru- och programvarulösningar, tekniker, IT-relaterade befattningar/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Ekonomi</span></strong></td>
   <td>
    <div>
      Ekonomisk programvara, finansiella tjänster/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Marknadsföring</span></strong></td>
   <td>
    <div>
      Marknadsföringsteknologier och programvara, marknadsrelaterade befattningar/anställning.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Business</span></strong></td>
   <td>
    <div>
      Forbes eller Inc listings eller Business Partnership.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Kundupplevelser och relationer</span></strong></td>
   <td>
    <div>
      Kundframgångar och kundrelationer befattningar/anställning.
    </div></td>
  </tr>
 </tbody>
</table>

Håll pekaren över verktygstipsen om du vill se en beskrivning av varje kolumn.

![](assets/tool-tip.png)

Klicka på listrutan [!UICONTROL Add ICP Indicator] för att infoga ytterligare indikatorer i modellen.

![](assets/add-icp.png)

Om du markerar rutan [!UICONTROL Export] kan du se ICP-indikatorn på informationssidan för [!UICONTROL Named Account] och använda den valda ICP-indikatorn som begränsningar i [namngivna kontofilter](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>ICP-indikatorer inkluderas som begränsningar i **[!UICONTROL Member of Named Account]**-filter och utlösare.

[!UICONTROL Indicator Weightage] är den prioritetsnivå som varje indikator får i din modell.

![](assets/weightage.png)

Klicka på **[!UICONTROL Refresh Model]** för att ändringarna ska börja gälla.

![](assets/refresh-button.png)

När du är klar med att justera modellen (efter att du har uppdaterat den) går du tillbaka till fliken Modellresultat och klickar på **[!UICONTROL Save & Apply Ranks]**.

![](assets/ranks.png)
