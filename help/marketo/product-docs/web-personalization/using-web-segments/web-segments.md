---
unique-page-id: 4719093
description: Webbsegment - Marketo Docs - produktdokumentation
title: Webbsegment
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 0%

---

# Webbsegment {#web-segments}

## Visa segment {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

På fliken Segment visas alla anpassade definierade segment som du ställer in baserat på olika attribut.  **Ett segment är en samling besökare som uppfyller de angivna villkoren som definieras på sidan Ange ett segment.**  Ett segment kan vara besökare från en viss bransch, plats eller baserat på besökarens aktivitet på plats.

Inom webbpersonalisering kan en besökare matcha mer än ett segment. Om det till exempel finns ett segment för besökare i USA och ett segment för finansföretag skulle en webbbesökare från Bank of America matcha **båda** segmentet för besökare i USA och segmentet för finansföretag.

**DIAGRAM:**  På sidan Segment visas ett stapeldiagram över de valda segmenten utifrån antalet besökare från segmentet (y-axeln) och segmentnamnet (x-axeln).

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Namn</th> 
   <th colspan="1" rowspan="1">Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Namn</strong></td> 
   <td colspan="1" rowspan="1">Segmentets titel</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Matchar</strong></p></td> 
   <td colspan="1" rowspan="1">Antalet besökare som uppfyller segmentets anpassade, definierade villkor</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Ange kampanj</strong></td> 
   <td colspan="1" rowspan="1">Gör att du kan ställa in en Campaign CTA som är associerad med den valda söktermen</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Besökare</strong></td> 
   <td colspan="1">En förhandsgranskning av besökstabellen som är associerad med den valda söktermen</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Clickstream</strong></td> 
   <td colspan="1" rowspan="1">Visar en tabell över besökarens aktivitet och URL-sökväg på webbplatsen och hur länge besökaren besökte varje sida </td> 
  </tr> 
 </tbody> 
</table>

Se [hur du skapar och visar segmentetiketter](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segment - högerpanel**

![](assets/image2014-11-12-10-3a46-3a32.png)

Om du markerar ett segment i tabellen visas mer information om segmentet på den högra panelen.

Bland dessa uppgifter finns:

* Segmentets namn
* Segmentets skapandedatum
* De associerade kampanjerna visar vilka kampanjer som används i segmentet. Om du klickar på antalet reaktioner kommer du till kampanjsidan där kampanjkoden (Call to Action) för segmentet visas
* Antalet matchningar (antalet besökare som uppfyller segmentvillkoren) för segmentet och antalet distinkta (unika) besökare som matchade segmentet. När du klickar på den unika besökarlänken visas segmentets resultat på besökarens sida
* Segmentets ägare/användare som skapat det
* Domänwebbplatserna som är kopplade till segmentet
* En kort sammanfattning av de valda villkoren för segmentet

## Aktivera eller inaktivera ett segment {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Om du vill aktivera eller inaktivera ett segment markerar du kryssrutan för det segmentet i tabellen och väljer åtgärden Aktivera eller Inaktivera i listrutan Välj åtgärd längst ned i tabellen. När ett segment är inaktiverat visas ordet&quot;inaktivera&quot; under kolumnen Läge.

## Skapa segment {#create-segments}

Segmentet som du skapar uppfyller de specifika villkor som du anger i **Ange segment** sida. Ni kan anpassa era segment baserat på en kombination av kriterier också, och inrikta er på en viss målgrupp i kampanjen.

Skapa ett nytt segment

Från **Segment** sida, klicka **Skapa nytt** under diagrammet. Följande skärm visas.

![](assets/four.png)

Definiera allmänna parametrar för ditt segment:

* **Namn:**  Ge segmentet ett namn.
* **Beskrivning:**  Ge en mer detaljerad förklaring av segmentvillkoren.
* **Domäner:**  Markera den eller de domäner som du vill inkludera i segmentet.
* **Segmentregellogik:**  Välj en AND/OR-logik för att skapa varje segmenteringsattribut
* **Timing:** Definiera nivån på besökarens engagemang i kampanjen

   * **Vid registrering**: Engagemang från besökaren kommer till webbplatsen
   * **Efter 1:a och 9:e klickningen**: Engagera besökaren efter ett visst antal klick på webbplatsen

>[!TIP]
>
>**Segmentregellogik**
>
>Det finns tre filteralternativ:
>
>1. Använd alla filter (1, 2 och 3...)
>1. Använd filter (1 eller 2 eller 3..)
>1. Avancerade filter (med och/eller uttryck)
>
>    Med avancerade filter kan du styra segmentvillkoren. Ange filternumren avgränsade med &quot;och&quot; och &quot;eller&quot;.
>
>    * 1, 2 och 3
>    * 1 eller 2 eller 3
>
>    Blandning av&quot;och&quot; och&quot;eller&quot; kräver parenteser för att förtydliga logiks avsikt. &quot;1 eller 2 och 3&quot; skall skrivas som något av följande:
>
>    * 1 och (2 eller 3)
>    * (1 och 2) eller 3
>
>    Kapslade parenteser accepteras för mer komplicerad logik, t.ex.
>
>    * (1 och 2) eller (3 och 4)
>    * 1 och (2 eller (3 och 4))
>
>    Kontrollera logiken efter infogning, borttagning eller sortering.

Dra och släpp segmentattribut från den högra kolumnen i segmentredigeraren till vänster:

![](assets/five.png)

### Firmographics {#firmographics}

**Plats**

Dra och släpp **Plats** i segmentredigeraren.

* Välj bland följande parametrar:

   * **Inkludera** - Välj om du vill att kampanjen ska inkludera eller exkludera en plats.
   * **Välj land att lägga till** - I listrutan väljer du det land du vill inkludera i segmentet. Landsnamnet visas till höger. Du kan välja flera länder.

När landet har lagts till kan du även ange segmentets stat, ort och postnummer.

* **Välj delstat eller region som ska läggas till** - I listrutan väljer du delstat eller kanadensisk provins som du vill inkludera. Du kan göra flera val.
* **Postnummer** - Ange det postnummer du vill inkludera i ditt segment.
* **Städer** - Ange den ort eller de städer du vill inkludera. Använd ett semikolon mellan städer.

>[!TIP]
>
>**Vilka segmentvillkor väljer jag? &#39;AND&#39; eller &#39;OR&#39;?** Eller fungerar som ett extra alternativ i varje fält. Prospekt behöver bara uppfylla ett av de kriterier som valts ut i varje fält för att vara kvalificerade för segmentet. (Prospekt kan till exempel antingen komma från USA. *eller* från försvarsindustrin). AND fungerar som en extra obligatorisk parameter som måste uppfyllas för det här segmentet. (Prospekten måste till exempel vara både från USA och försvarsindustrin). Inom varje segmenteringsprofil kan varje separat fält fungera som både och, antingen&quot;AND&quot; eller&quot;OR&quot; beroende på vilket segmentvillkor som valts.

**Branscher** Under **Profilsegmentering** markerar du kryssrutan intill **Bransch**.

* Välj bland följande parametrar:

   * **Inkluderar** - Välj om du vill att segmentet ska inkludera eller exkludera en bransch.
   * **Välj branscher att lägga till** - Välj vilken bransch du vill inkludera i segmentet. Branschen visas under listrutan. Du kan välja flera branscher.

**Organisationsgrupp**

Under **Profilsegmentering** markerar du kryssrutan intill **Organisationsgrupp.**

* Välj bland följande alternativ i listrutan:

   * Fortune 500 - Omfattar endast Fortune 500-företag i detta segment
   * Fortune 1000 - Omfattar endast Fortune 1000-företag i detta segment
   * Global 2000 - Innefattar Global 2000-företagen i detta segment
   * Enterprise - Innehåller organisationer med fler än 1 000 anställda och intäkter över 250 miljoner dollar
   * SMB - Endast små och medelstora företag ingår i detta segment

**-Namngivna konton-**

**Organisationer**

* **Kommer från dessa företag (specifika namn)**

   * Välj företag att rikta in på i listrutan Välj företag att lägga till.
   * Du kan ange det exakta organisationsnamn som du vill ha som mål. *Det är _alltid_ Vi rekommenderar att du använder Namngivna kontolistor i stället för att skriva in namnen manuellt för att få bättre matchningar (se nedan).

**Namngiven kontolista**

Välj från en [Namngiven kontolista](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) för att segmentera viktiga målkonton.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Siffran inom hakparenteser bredvid namnet Namngiven kontolista används som indexreferens för listan för webbanpassning [Läs API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization).

**Exkludera ISP**

Utesluter Internetleverantörer (ISP) från segmentet.

### Kända personer {#known-people}

**Databas**

Webbpersonalisering kan integreras med Marketo Database så att ni kan segmentera och personalisera kampanjer utifrån kända personattribut och data.

Välj Databas och välj ett persondatafält i listrutan. Välj **+** om du vill lägga till fält från listrutan.

![](assets/seven.png)

Du kan lägga till eller ta bort persondatafält från Kontoinställningar > Databas

>[!TIP]
>
>Skapa dina segmentkriterier utifrån alla persondatafält från Marketo-personer som Befattning, Poäng, Roll osv.
>
>T.ex. &quot;Befattning är lika med CMO&quot; och &quot;Poängen är mindre än eller lika med 50&quot;

**Marketo Email Campaign** Segmentera och personalisera kampanjer genom att skicka e-postmeddelanden från en besökare som klickar på ett e-postmeddelande från Marketo och kommer till webbplatsen. Segmentera efter Marketo programnamn eller kampanjnamn och fortsätt konversationen från e-post till webben. Välj + för att lägga till fält från listrutan.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Status**

Definiera ditt segment utifrån den potentiella kundens status: känd eller anonym.

* Känd - Välj det här alternativet i listrutan för kända besökare. En besökare är känd när de skickar in ett formulär på din webbplats och visas på sidan Webbpersonalisering.
* Anonym - Välj det här alternativet i listrutan för anonyma besökare.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Beteende {#behavioral}

**Besök -** Definiera segmentet utifrån besökarens beteende eller identifiering.

* Antal besök - Välj det här alternativet i listrutan för att ange antalet besök för potentiella kunder på webbplatsen.

   * Välj Lika med, Lika med eller Större än, eller Lika med eller Mindre än i listrutan.

* Specifika besök - Välj det här alternativet i listrutan för att ange en specifik besökare.

   * Ange det besökarnummer du vill spåra i textrutan till höger. Det unika besökaridentifieringsnumret för webbpersonalisering visas när du klickar på en besökare (på besökarsidan) och på Ställ in kampanj på den högra panelen. Besökar-ID finns i avsnittet Avancerade inställningar. Besökar-ID:t finns också i URL:en (t.ex. VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Sökvillkor** - Definiera ett segment enligt den potentiella kundens sökvillkor.

* Besökaren sökte efter - I listrutan väljer du de termer som du vill spåra från besökarens sökning eller lägger till egna söktermer. (Det finns inget behov av &#42; jokertecken i söktermer eftersom det är inställt som standard för att inkludera fraser som innehåller söktermen).

**Hänvisningar** - Lägg till URL:er som besökaren refererades till.

* Välj hänvisningar att lägga till - Välj de hänvisningswebbplatser du vill spåra i listrutan eller lägg till din egen hänvisning. När du har valt detta alternativ visas hänvisningarna i rutan nedan. (Använder &#42; som jokertecken tillåts)

**Inkludera sidor** - Spåra specifika sidor som potentiella kunder besökt på din webbplats.

* URL-matchningar - Lägg till URL:en för specifika webbsidor som du vill spåra. Du kan lägga till flera URL-adresser genom att separera dem med ett semikolon. (Använder &#42; som jokertecken).

**Uteslut sidor** - Uteslut specifika sidor som du inte vill matcha i segmentet. (Använder &#42; som jokertecken).

* URL:en matchar inte - Lägg till URL:en för specifika webbsidor som du vill utesluta från spårning. Du kan lägga till flera URL-adresser genom att separera dem med ett semikolon

![](assets/segment-extra.png)

### Enhet/webbläsare {#device-browser}

**Mobiloperativsystem**

Dra och släpp det mobila operativsystemet i segmentredigeraren

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Typ av besökare**<br />
  **Mobiloperativsystem** - I listrutan väljer du ett eller flera mobila operativsystem i listan. Det valda mobiloperativsystemet visas nedan.

   * Besökaren använder en mobil enhet
   * Besökaren använder den specifika enheten/operativsystemet
   * Besökaren använder inte någon mobil enhet

* **Enhet**  - I listrutan väljer du en eller flera enheter (Apple, Samsung, LG, HTC, Nexus, Blackberry osv.). De valda enheterna visas nedan.

**Webbläsare**

Målgrupp som använder specifika webbläsartyper och/eller versioner.

* Typ av webbläsare - Välj en eller flera webbläsare i listrutan. De valda webbläsarna visas nedan.
* Webbläsarversion - Ange den webbläsarversion som du vill lägga till i segmentet. Du kan välja flera versioner genom att separera dem med kommatecken. (Använder &#42; som jokertecken).

### API {#api}

**Datahändelser** - Segmentera besökare som utlöser specifika anpassade datahändelser

Lägg till det händelsevärde som du vill ha som mål. Till exempel från datakällor från tredje part.

**API för användarkontext**

API-anrop för webbanpassning  [läs mer om det här.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Använda jokertecken -** När du vill ta med ett sökord eller en URL som innehåller något i det, t.ex. &quot;[google.com](https://google.com)&quot; eller &quot;söktermsprodukt&quot;, kallar vi det här jokertecken och det ska läggas in med en asterisk - den här lilla killen&#42; - i varje ände. Så allt kommer från [google.com](https://google.com) ska anges som &#42; [google.com](https://google.com)&#42;

## Redigera segment {#edit-segments}

Du kan redigera ett segment som har skapats.

1. Om du vill redigera ett segment går du till **Segment**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. I **Segment** klickar du på redigeringsikonen ( ![](assets/segment-edit.png)) för det segment som du vill redigera. The **Ange segment** sidan öppnas med det valda segmentet.
1. Gör de ändringar du vill i segmentet.
1. Klicka **Spara**.

## Ta bort segment {#delete-segments}

Du kan ta bort segment som du har skapat.

1. Från **Segment** markerar du ett segment ovan.
1. Klicka på ikonen Ta bort ( ![](assets/segment-delete.png) ) för det segment som du vill ta bort.
1. Ett bekräftelsemeddelande visas som bekräftar att du håller på att ta bort **Segment**.

>[!NOTE]
>
Du kan inte ta bort ett segment som är associerat med en kampanj. Först måste ni ta bort kampanjen och sedan segmentet.

Bra! Nu när ni förstår segmentavsnittet kan vi lära oss mer om kampanjer.

>[!MORELIKETHIS]
>
* [Skapa ett enkelt webbsegment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
* [Skapa en ny webbkampanj för dialog](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Skapa en ny webbkampanj i zonen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Skapa en ny webbkampanj för widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
