---
unique-page-id: 7515401
description: Skapa en guidad landningssidmall - Marketo Docs - Produktdokumentation
title: Skapa en mall för guidad landningssida
translation-type: tm+mt
source-git-commit: 975e048271dae6a877ae9ff5d39360b159afcc8a
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---


# Skapa en mall för guidad landningssida {#create-a-guided-landing-page-template}

>[!NOTE]
>
>**Djupdykning:** Trött på att läsa? [Titta på den här videon](https://youtu.be/3O7e4GdZKsM) med steg-för-steg-instruktioner.

Mallar för guidade landningssidor har en speciell syntax. Använd den här syntaxen för att ange vad som kan anpassas och var innehållet ska hamna på varje landningssida som skapats utifrån din mall. Endast de regioner eller variabler som du anger som redigerbara kommer att vara tillgängliga för anpassning i den guidade redigeraren för landningssidor.

>[!TIP]
>
>Använd vedertagna namnkonventioner så kommer marknadsföringsteamet att älska med dig.

Det finns två sätt att deklarera att något på sidan ska kunna redigeras:

* Deklarera ett objekt som ett &quot;element&quot;. Den som skapar landningssidan kan lägga till bilder, text eller Marketo-resurser i de angivna områdena.
* Deklarera en sträng som en&quot;variabel&quot;. Den som skapar landningssidan kan ersätta variabeln med en sträng, färg eller booleskt läge från en true/false-spak.

## Redigerbara element {#editable-elements}

Elementen deklareras genom att ett vanligt DOM-element läggs till i mallen och elementet dekoreras med ett Marketinspecifikt klassnamn.

## Text {#text}

Om du definierar ett område som RTF-text kan användarna redigera innehållet [med hjälp av Marketos RTF-redigerare](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attribut som krävs:\
**klass**: &quot;mktoText&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
Innehållet i ett element med klassen mktoText (om sådan finns) används som standardvärde för det redigerbara området.

Exempel:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Bild {#image}

Det finns två alternativ för att definiera redigerbara bildelement. Du kan antingen använda en `<div>`, som anger en behållare som bilden ska infogas i, eller en `<img>` tagg.

## Alternativ 1 - Använd <div> {#option-use-a-div}

Attribut som krävs:

klass: &quot;mktoImg&quot;\
id: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
mktoName : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
mktoImgClass: Sträng. Värdet här läggs till i klassattributet för `<img>` elementet inuti div-filen.

Exempel:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Alternativ 2 - Använd `<img>` {#option-use-a-img}

Attribut som krävs:\
klass: &quot;mktoImg&quot;\
id: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
mktoName : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
src: Sträng-URL. Detta används som standardvärde för bilden.

Exempel:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>När du använder `<img>` versionen innehåller den återgivna HTML-koden en genererad div-wrapper runt `<img>` -taggen. Den ställs in på klassen .&quot;mktoImg.mktoGen&quot;, och kommer att visas:inline-block.

## Formulär {#form}

Exempel:Attribut som krävs:\
**klass**: &quot;mktoForm&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Fragment {#snippet}

Attribut som krävs:\
**klass**: &quot;mktoSnippet&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Knappen Dela {#share-button}

Attribut som krävs:\
**klass**: &quot;mktoShareButton&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Video {#video}

>[!NOTE]
>
>När du använder videoelementet på en landningssida stöder Marketo endast videor från YouTube. Om du använder en annan tjänst rekommenderar vi att du använder en RTF-ruta och klistrar in videons inbäddningskod.

Attribut som krävs:
**klass**: &quot;mktoVideo&quot;**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Omröstning {#poll}

Attribut som krävs:\
**klass**: &quot;mktoPoll&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Hänvisning {#referral}

Attribut som krävs:\
**klass**: &quot;mktoReferral&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Lotteriet {#sweepstakes}

Attribut som krävs:\
**klass**: &quot;mktoSweepstakes&quot;\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Redigerbara variabler {#editable-variables}

Alla variabeltyper används genom att referera till värdet för deras id-attribut som omsluts av en ${ }-teckensekvens. De kan användas var som helst i dokumentet, utom i andra variabeldeklarationer.

Exempel:

`<pre data-theme="Confluence">${var1}</pre>`

**Deklaration:**

Variabler deklareras som metataggar inuti mallens `<head>` element. Det finns tre typer av variabler som kan användas: Sträng, Färg och Boolean.

## Sträng {#string}

Attribut som krävs:\
**class** : &quot;mktoString&quot;,\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
**standard**: Strängvärde för attributet. Tomt om inget anges.\
**allowHTML**: &quot;true&quot; eller &quot;false&quot;. Kontrollerar om värdet skrivs ut utan att HTML-koden behöver föregås av ett undantag. Standardvärdet är &quot;false&quot; om det tas bort.

Grundläggande exempel:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Exempel med alla attribut:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Färg {#color}

Attribut som krävs:\
**class** : &quot;mktoColor&quot;,\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
**standard**: En 7-siffrig färgkod för HEX-tecken. Exempel: &quot;#336699&quot;

Grundläggande exempel:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Exempel med alla attribut:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Boolean {#boolean}

Attribut som krävs:\
**class** : &quot;mktoBoolean&quot;,\
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.\
**mktoName** : Sträng. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:\
**standard**: Boolesk sträng. &quot;true&quot; eller &quot;false&quot; kontrollerar om värdet börjar i position ON eller OFF. &quot;false&quot; om inget anges.\
**false_value**: Sträng. Det värde som ska infogas för variabeln när den är i AV-positionen. &quot;false&quot; om inget anges.\
**true_value**: Sträng. Värdet som ska infogas för variabeln när den är på-positionen. &quot;true&quot; om inget anges.\
**false_value_name**: Sträng. Det visningsnamn som ska visas i landningssidans redigerare när värdet är i AV-läge. &quot;AV&quot; om ej angivet.\
**true_value_name**: Sträng. Det visningsnamn som ska visas i landningssidans redigerare när värdet är på-positionen. &quot;ON&quot; om inte anges.

Grundläggande exempel:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Exempel med alla attribut:

I det här exemplet visas ett vanligt användningsfall där en boolesk variabel styr synligheten för ett CSS-element genom att ange värdet för CSS-visningsegenskapen till antingen &quot;block&quot; eller &quot;none&quot; för att visa/dölja ett element med id:t med CSS. Landningssidans redigerare använder visningsnamnet Visa/Dölj i stället för AV/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Programtokens (my.token) kan också användas var som helst på landningssidorna Guidad och Frihandsfigur.
