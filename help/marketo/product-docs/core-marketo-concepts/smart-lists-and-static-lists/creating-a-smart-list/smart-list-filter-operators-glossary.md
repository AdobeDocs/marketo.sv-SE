---
unique-page-id: 557312
description: Operatorordlista för smarta listfilter - Marketo Docs - produktdokumentation
title: Ordlista för operatorer för smarta listfilter
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 1%

---

# Ordlista för operatorer för smarta listfilter {#smart-list-filter-operators-glossary}

En operator är en del av den smarta listan som hjälper dig att få en specifik bild. Du kan beskriva filtret eller utlösaren på ett enkelt språk. De tillgängliga operatorerna är olika för varje fälttyp.

Här är en ordlista som beskriver varje uppsättning operatorer.

## Datumfält {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

När du väljer en operator ändras den högra sidan dynamiskt.

<table><thead>
  <tr>
    <th>Operator</th>
    <th>Höger sida</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>är</td>
    <td>Enstaka datum</td>
    <td>Exakt datummatchning</td>
  </tr>
  <tr>
    <td>är inte</td>
    <td>Enstaka datum</td>
    <td>Alla datum förutom det angivna</td>
  </tr>
  <tr>
    <td>mellan</td>
    <td>Två datumfält</td>
    <td>Alla datum inklusive och mellan två angivna datum</td>
  </tr>
  <tr>
    <td>tidigare</td>
    <td>Indata för naturligt språk*</td>
    <td>Se diagrammet nedan</td>
  </tr>
  <tr>
    <td>tidigare än</td>
    <td>Indata för naturligt språk*</td>
    <td>Se diagrammet nedan</td>
  </tr>
  <tr>
    <td>i framtiden</td>
    <td>Indata för naturligt språk*</td>
    <td>Se diagrammet nedan</td>
  </tr>
  <tr>
    <td>i framtiden</td>
    <td>Indata för naturligt språk*</td>
    <td>Se diagrammet nedan</td>
  </tr>
  <tr>
    <td>tidsram</td>
    <td>Förinställningar (sista kvartalet, igår osv.)</td>
    <td>Definierad i plocklista</td>
  </tr>
  <tr>
    <td>efter</td>
    <td>Enstaka datum</td>
    <td>Alla poster efter angivet datum</td>
  </tr>
  <tr>
    <td>före</td>
    <td>Enstaka datum</td>
    <td>Alla poster före den angivna</td>
  </tr>
  <tr>
    <td>på eller efter</td>
    <td>Enstaka datum</td>
    <td>Samma som"efter" men inkluderande</td>
  </tr>
  <tr>
    <td>på eller före</td>
    <td>Enstaka datum</td>
    <td>Samma som"före" men inklusive</td>
  </tr>
  <tr>
    <td>är tom</td>
    <td>Ingen</td>
    <td>Alla poster utan datum</td>
  </tr>
  <tr>
    <td>är inte tom</td>
    <td>Ingen</td>
    <td>Alla poster med valfritt datum</td>
  </tr>
</tbody></table>

**&#42;** Naturliga språkindata är coola. Här är några av de mönster du kan ange:

* 1 timme
* 82 dagar
* 3 veckor
* 14 månader
* 1 år

Skriv bara in numret och enheten så fungerar det!

>[!NOTE]
>
>&quot;Tidigare&quot; _omfattar_ den dag (fram till tidpunkten, inte efter) som du skapar din smarta lista.

>[!CAUTION]
>
>När du skapar en smart lista med ett datumfältfilter (t.ex. Födelsedatum, Skapat av SFDC) och använder begränsningarna **[!UICONTROL before]**, **[!UICONTROL on or before]** eller **[!UICONTROL in past before]**, kommer den smarta listan även att innehålla personer som inte har något värde i det datumfältet.

Använd följande diagram för att förstå skillnaden mellan datumoperatorerna.

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**Exempel**
>
>Datumfält kan bli knepiga när du arbetar med tidigare och framtida händelser. Här är några exempel.
>
>**[!UICONTROL In past before]**
>
>Använd den här operatorn för att skicka e-post till personer som inte har prenumererat på eller förnyat tjänsten inom ett år eller som aldrig har varit prenumeranter.
>
>**[!UICONTROL In future after]**
>
>Säg att ni vill se kunder som är redo för förnyelse på 90 dagar. Du använder två separata filter. Använd först&quot;I framtiden efter 90 dagar&quot; och sedan&quot;I framtiden 91 dagar&quot;. Det skulle fånga den som har ett datum 90 dagar från nu.

## Strängfält {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>Operator</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>är</td>
    <td>Exakt matchning (ej skiftlägeskänslig)</td>
  </tr>
  <tr>
    <td>är inte</td>
    <td>Allt utom exakt matchning</td>
  </tr>
  <tr>
    <td>börjar med</td>
    <td>Första bokstäver i strängmatchning</td>
  </tr>
  <tr>
    <td>börjar inte med</td>
    <td>Strängens första bokstäver matchar INTE</td>
  </tr>
  <tr>
    <td>innehåller</td>
    <td>Alla bokstäver i strängen matchar (exempel: california, förmögenhet, däri)</td>
  </tr>
  <tr>
    <td>innehåller inte</td>
    <td>Inga bokstäver i strängmatchningen. (inverterat av "contains")</td>
  </tr>
  <tr>
    <td>är tom</td>
    <td>Poster utan värde (NULL)</td>
  </tr>
  <tr>
    <td>är inte tom</td>
    <td>Poster med ANY-värde</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Använd positiva över negativa operatorer. Filtren &quot;Is not&quot; måste söka igenom hela datauppsättningen i din instans, vilket kan vara extremt tidskrävande. Positiva&quot;is&quot;-filter kan utnyttja effektivare sökalgoritmer.

## Heltalsfält {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Operator</th>
    <th>Beskrivning</th>
  </tr></thead>
<tbody>
  <tr>
    <td>är</td>
    <td>Exakt nummermatchning ( = 0 returnerar båda leads med 0 och NULL)</td>
  </tr>
  <tr>
    <td>är inte</td>
    <td>Allt utom exakt nummermatchning</td>
  </tr>
  <tr>
    <td>mellan</td>
    <td>Definiera två värden för att hitta alla däremellan (inklusive)</td>
  </tr>
  <tr>
    <td>större än</td>
    <td>Ovanför angivet</td>
  </tr>
  <tr>
    <td>mindre än</td>
    <td>Mindre än den angivna</td>
  </tr>
  <tr>
    <td>minst</td>
    <td>Ovanför angivet (inkluderande)</td>
  </tr>
  <tr>
    <td>högst</td>
    <td>Mindre än den angivna (inkluderande)</td>
  </tr>
  <tr>
    <td>är tom</td>
    <td>Poster som saknar värde (NULL) - noll är ett tal, det är inte NULL</td>
  </tr>
  <tr>
    <td>är inte tom</td>
    <td>Poster med ANY-värde (inklusive noll)</td>
  </tr>
</tbody>
</table>

Som du ser gör de här operatorerna det enkelt att tala Marketo-esiska flytande!
