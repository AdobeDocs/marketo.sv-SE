---
unique-page-id: 2951877
description: Understanding the Program Opportunity Analysis Area - Marketo Docs - Product Documentation
title: Understanding the Program Opportunity Analysis Area
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 0%

---

# Understanding the Program Opportunity Analysis Area {#understanding-the-program-opportunity-analysis-area}

## Översikt {#overview}

Under Analys av affärsmöjlighet kan du analysera enskilda programs effektivitet eller se summerade resultat per programkanal.

**Exempel på affärsfrågor som du kan besvara med det här analysområdet är**:

Hur många möjligheter har kopplats till ett visst program och hur många av dem har vi vunnit?

![](assets/one-1.png)

Hur stor intäkt har ett visst program eller en viss kanal gett?

![](assets/two-1.png)

Vad är mina intäkter för investeringar för ett visst program eller en viss kanal?

![](assets/three-1.png)

Vilka möjligheter påverkade programmet?

![](assets/four-1.png)

## Attributionsåtgärder för analys av affärsmöjligheter (blå punkter) {#program-opportunity-analysis-attribution-measures-blue-dots}

De mått som är tillgängliga för dig att använda vid analys är vanligtvis siffror och representeras av blå punkter. Dimensioner är attribut som ger olika vyer av måtten och representeras av gula punkter.

Alla åtgärder (blå punkter) avser attribuering -&quot;kredit&quot; för inköp av leads eller för säljframgångar som är kopplade till ett lead.

![](assets/six.five.png) ![](assets/seven-1.png)

Det finns tre typer av åtgärder:

* Förvärvsrelaterade mått, som får förstahandsattribuering (FT).
* Framgångsrelaterade mått, som får multitouch-attribuering (MT).
* Diverse programrelaterade åtgärder, inklusive det genomsnittliga antalet marknadsföringsåtgärder innan affärsmöjligheter skapas eller stängs.

## Förvärva och framgångsrika åtgärder {#acquisition-and-success-related-measures}

Förvärvningsrelaterade åtgärder tillskriver programmet genom vilket en leads kontaktinformation först hämtas. En lead behöver inte bli framgångsrik i ett program för att bli godkänd.

Värdet för att köpa en viss lead ändras över tiden. Det är noll tills ett köp görs av leadet. Den kan sedan öka med ytterligare inköp.

Framgångsrelaterade åtgärder tillskriver alla program som bidrar till att ett lead går mot ett inköp.

Precis som med förvärvet ändras värdet av att bidra till försäljningen av en lead över tiden, och är noll tills något inköp görs av leadet.

<table>
 <tbody>
  <tr>
   <th>Attributionsmått - säljprojektsrelaterade (FT eller MT)*</th>
   <th>Beskrivning</th>
  </tr>
  <tr>
   <td>Affärsmöjlighet</td>
   <td>Den del av kostnaden för programmet som påverkade affärsmöjligheten. Kostnaden kan delas upp om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Skapade affärsmöjligheter</td>
   <td>Den del av krediten som programmet fick för att påverka skapandet av affärsmöjligheten. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Vunna affärsmöjligheter</td>
   <td>Den del av krediten som programmet fick för att påverka den vunna affärsmöjligheten. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Pipeline skapad</td>
   <td>Den del av krediten (i penningvärde) som programmet fick för att påverka skapandet av affärsmöjligheten. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Pipeline skapad - fortfarande öppen</td>
   <td>Andelen kredit (i penningvärde) som programmet tog emot för att påverka skapandet av den öppna affärsmöjligheten. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Förväntade intäkter</td>
   <td>Den del av krediten (i penningvärde) som programmet fick för att påverka skapandet av affärsmöjligheten. Förväntad intäkt är sannolikheten för affärsmöjligheten multiplicerad med affärsmöjlighetsvärdet. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
  <tr>
   <td>Intäkter från investeringar</td>
   <td>Detta är andelen kredit (i penningvärde) som programmet fått för att påverka vunna möjligheter och kostnaden för programmet.</td>
  </tr>
  <tr>
   <td>Vinst på intäkt</td>
   <td>Andelen kredit (i penningvärde) som programmet fick för att påverka vunna möjligheter. Det kan vara en bråkdel om flera leads är inblandade.</td>
  </tr>
 </tbody>
</table>

_&#42;(FT) = First-Touch Attribution, används för mått på lead-förvärv; (MT) = Multi-Touch Attribution, används för mått på lead-lyckade_

Nedan visas ett scenario som beskriver hur säljprojektsenheter beräknas när det finns två program som genererade leads, men dessa leder till ett säljprojekt från samma konto.

**Program 1**

* Genererar en lead: Lead 1
* Lead 1 är från konto 1

**Program 2**

* Skapar en annan lead: Lead 2
* Lead 2 kommer också från konto 1

**Konto 1**

* Skapar en affärsmöjlighet: affärsmöjlighet 1

Marketo ger krediter utan att man behöver göra dubbelräkning i alla program. I det här fallet får varje program 0,5 enheter för säljprojekt. Det innebär att varje program får hälften av krediterna för den skapade möjligheten. Hälften av de intäkter som är kopplade till säljprojektet tilldelas respektive program.

## Diverse programrelaterade åtgärder {#miscellaneous-program-related-measures}

De andra tillgängliga åtgärderna återspeglar programmets övergripande resultat.

<table>
 <tbody>
  <tr>
   <th>Attributionsmått - programrelaterat</th>
   <th>Beskrivning</th>
  </tr>
  <tr>
   <td>Antal affärsmöjligheter som är associerade med programmet</td>
   <td><p>Det totala antalet affärsmöjligheter som har gett ett program någon form av attribueringskrediter. Möjligheterna kan påverkas av ett eller flera leads och av ett eller flera program.</p></td>
  </tr>
  <tr>
   <td>Genomsnittligt antal lyckade försök per avslutad affärsmöjlighet</td>
   <td>Genomsnittligt antal lyckade program innan affärsmöjligheten stängdes. <br></td>
  </tr>
  <tr>
   <td>Genomsnittligt antal lyckade försök per projekt som skapats</td>
   <td>Genomsnittligt antal lyckade program innan affärsmöjligheten skapades.</td>
  </tr>
  <tr>
   <td>Nya namn</td>
   <td>Det totala antalet nya namn, det vill säga nya leads, som förvärvats av programmet.</td>
  </tr>
  <tr>
   <td>Programkostnad</td>
   <td>Total kostnad för programmet.</td>
  </tr>
  <tr>
   <td>Slutfört (totalt)</td>
   <td>Det totala antalet programmedlemmar som lyckades.</td>
  </tr>
 </tbody>
</table>

## Analysdimensioner för programsäljprojekt (gula prickar) {#program-opportunity-analysis-dimensions-yellow-dots}

Måtten (blå punkter) beräknas, och det krävs en viss tanke och förklaring för att kunna använda dem, medan dimensioner (gula punkter) är beskrivande. Här är de tillgängliga dimensionerna.

<table>
 <tbody>
  <tr>
   <th>Kategori</th>
   <th>Visningsetikett</th>
  </tr>
  <tr>
   <td>Attribut för affärsmöjlighet</td>
   <td>Affärsmöjligheten har stängts<br>Affärsmöjlighetens namn*<br>Affärsmöjlighetens ägarnamn<br>Affärsmöjlighetens stadium<br>Affärsmöjlighetstyp</td>
  </tr>
  <tr>
   <td>Tidsram för affärsmöjlighet</td>
   <td>Affärsmöjligheten stängd år/kvartal/månad<br>Skapad affärsmöjlighet år/kvartal/månad</td>
  </tr>
  <tr>
   <td>Programattribut</td>
   <td>Programkanal<br>Programnamn</td>
  </tr>
  <tr>
   <td>Tidsram för programkostnad</td>
   <td>Kostnadsår/kvartal/månad</td>
  </tr>
 </tbody>
</table>

*&#42;Alla affärsmöjligheter som gav någon typ av attribueringskrediter till ett program. Möjligheter kan påverkas av ett eller flera leads och av ett eller flera program.*

>[!MORELIKETHIS]
>
>[Skapa en Intresseutforskarrapport](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
