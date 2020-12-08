---
unique-page-id: 557312
description: Operatorordlista för smarta listfilter - Marketo Docs - Produktdokumentation
title: Ordlista för operatorer för smarta listfilter
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# Ordlista för operatorer för smarta listfilter {#smart-list-filter-operators-glossary}

En operator är en del av den [smarta listan](http://docs.marketo.com/display/docs/smart+lists+and+static+lists) som hjälper dig att få reda på mer. Du kan beskriva filtret eller utlösaren på ett enkelt språk. De tillgängliga operatorerna är olika för varje fälttyp.\
Här är en ordlista som beskriver varje uppsättning operatorer.

## Datumfält {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

När du väljer en operator ändras den högra sidan dynamiskt.

| Operator | Höger sida | Beskrivning |
|---|---|---|
| är | Enstaka datum | Exakt datummatchning |
| är inte | Enstaka datum | Alla datum förutom det angivna |
| mellan | Två datumfält | Alla datum inklusive och mellan två angivna datum |
| tidigare | Indata för naturligt språk* | Se diagrammet nedan |
| tidigare än | Indata för naturligt språk* | Se diagrammet nedan |
| i framtiden | Indata för naturligt språk* | Se diagrammet nedan |
| i framtiden efter | Indata för naturligt språk* | Se diagrammet nedan |
| tidsram | Förinställningar (sista kvartalet, igår osv.) | Definierad i plocklista |
| efter | Enstaka datum | Alla poster efter angivet datum |
| före | Enstaka datum | Alla poster före den angivna |
| på eller efter | Enstaka datum | Samma som&quot;efter&quot; men inkluderande |
| på eller före | Enstaka datum | Samma som&quot;före&quot; men inklusive |
| är tom | Ingen | Alla poster utan datum |
| är inte tom | Ingen | Alla poster med valfritt datum |

* Inmatningen i naturens språk är häftig. Här är några av de mönster du kan ange:

* 1 timme
* 82 dagar
* 3 veckor
* 14 månader
* 1 år

Skriv bara in numret och enheten så fungerar det!

>[!NOTE]
>
>Tidigare **omfattar** det datum (fram till tidpunkten, inte efter) som du skapar den smarta listan.

>[!CAUTION]
>
>När du skapar en smart lista med ett datumfältsfilter (t.ex. Födelsedatum, Skapat den SFDC) och använder begränsningarna **före** eller **före** eller före, kommer den smarta listan även att omfatta personer som inte har något värde i det datumfältet.

Använd följande diagram för att förstå skillnaden mellan datumoperatorerna.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Exempel**
>
>Datumfält kan bli knepiga när du arbetar med tidigare och framtida händelser. Här är några exempel.
>
>**Tidigare**
>
>Använd den här operatorn för att skicka e-post till personer som inte har prenumererat på eller förnyat tjänsten inom ett år eller som aldrig har varit prenumeranter.
>
>**I framtiden efter**
>
>Säg att ni vill se kunder som är redo för förnyelse på 90 dagar. Du använder två separata filter. Använd först&quot;I framtiden efter 90 dagar&quot; och sedan&quot;I framtiden 91 dagar&quot;. Det skulle fånga den som har ett datum 90 dagar från nu.

## Strängfält {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operator | Beskrivning |
|---|---|
| är | Exakt matchning (ej skiftlägeskänslig) |
| är inte | Allt utom exakt matchning |
| börjar med | Första bokstäver i strängmatchning |
| börjar inte med | Strängens första bokstäver matchar INTE |
| innehåller | Alla bokstäver i strängen matchar (exempel: california, förmögenhet, därav) |
| innehåller inte | Inga bokstäver i strängmatchningen. (omvänt för &quot;contains&quot;) |
| är tom | Poster som inte har något värde (NULL) |
| är inte tom | Poster med ANY-värde |

>[!TIP]
>
>Använd positiva över negativa operatorer. Filtren &quot;Is not&quot; måste söka igenom hela datauppsättningen i din instans, vilket kan vara extremt tidskrävande. Positiva&quot;is&quot;-filter kan utnyttja effektivare sökalgoritmer.

## Heltalsfält {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operator</th> 
   <th colspan="1" rowspan="1"><p>Beskrivning</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">är</td> 
   <td colspan="1" rowspan="1">Exakt nummermatchning ( = 0 returnerar båda leads med 0 <em>och</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">är inte</td> 
   <td colspan="1" rowspan="1">Allt utom exakt nummermatchning</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">mellan</td> 
   <td colspan="1" rowspan="1">Definiera två värden för att hitta alla däremellan (inklusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">större än</td> 
   <td colspan="1" rowspan="1">Ovanför angivet</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">mindre än</td> 
   <td colspan="1" rowspan="1">Mindre än den angivna</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">minst</td> 
   <td colspan="1" rowspan="1">Ovanför angivet (inkluderande)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">högst</td> 
   <td colspan="1" rowspan="1">Mindre än den angivna (inklusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">är tom</td> 
   <td colspan="1" rowspan="1">Poster som inte har något värde (NULL) - noll är ett tal, det är <em>inte</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">är inte tom</td> 
   <td colspan="1" rowspan="1">Poster med ANY-värde (inklusive noll)</td> 
  </tr> 
 </tbody> 
</table>

Som du ser gör de här operatorerna det enkelt att tala Marketo-ese flytande!
