---
unique-page-id: 7515401
description: Skapa en guidad landningssidmall - Marketo Docs - produktdokumentation
title: Skapa en mall för guidad landningssida
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1263'
ht-degree: 1%

---

# Skapa en mall för guidad landningssida {#create-a-guided-landing-page-template}

Mallar för guidade landningssidor har en speciell syntax. Använd den här syntaxen för att ange vad som kan anpassas och var innehållet ska hamna på varje landningssida som skapats utifrån din mall. Endast de regioner eller variabler som du anger som redigerbara kommer att vara tillgängliga för anpassning i den guidade redigeraren för landningssidor.

>[!TIP]
>
>Använd vedertagna namnkonventioner så kommer marknadsföringsteamet att älska med dig.

Det finns två sätt att deklarera att något på sidan ska vara redigerbart:

* Deklarera ett objekt som ett &quot;element&quot;. Den som skapar landningssidan kan lägga till bilder, text eller Marketo-resurser i dessa angivna områden.
* Deklarera en sträng som en&quot;variabel&quot;. Den som skapar landningssidan kan ersätta variabeln med en sträng, färg eller booleskt läge från en true/false-spak.

## Redigerbara element {#editable-elements}

Elementen deklareras genom att ett vanligt DOM-element läggs till i mallen och elementet dekoreras med ett Marketo-specifikt klassnamn.

## Text {#text}

Om du definierar ett område som RTF kan användare redigera innehållet [med Marketo RTF-redigerare](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attribut som krävs:
**klass**: &quot;mktoText&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
Innehållet i ett element med klassen mktoText (om sådan finns) används som standardvärde för det redigerbara området.

Exempel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Bild {#image}

Det finns två alternativ för att definiera redigerbara bildelement. Du kan antingen använda en `<div>`, som anger en behållare som bilden ska infogas i, eller en `<img>` -tagg.

## Alternativ 1 - Använd en `<div>` {#option-use-a-div}

Attribut som krävs:

class: &quot;mktoImg&quot;
id: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
mktoName : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
mktoImgClass: String. Värdet här läggs till i klassattributet för elementet `<img>` inuti div:n.

Exempel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Alternativ 2 - Använd en `<img>` {#option-use-a-img}

Attribut som krävs:
class: &quot;mktoImg&quot;
id: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
mktoName : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
src: Sträng-URL. Detta används som standardvärde för bilden.

Exempel:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>När du använder versionen `<img>` innehåller den återgivna HTML en genererad div-wrapper runt taggen `<img>`. Den ställs in på klassen .&quot;mktoImg.mktoGen,&quot; och kommer att visas :inline-block.

## Formulär {#form}

Exempel på :Required-attribut:
**class**: &quot;mktoForm&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Fragment {#snippet}

Attribut som krävs:
**klass**: &quot;mktoSnippet&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Knappen Dela {#share-button}

Attribut som krävs:
**klass**: &quot;mktoShareButton&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Video {#video}

>[!NOTE]
>
>När du använder videoelementet på en landningssida stöder Marketo endast videor från YouTube. Om du använder en annan tjänst rekommenderar vi att du använder en RTF-ruta och klistrar in videons inbäddningskod.

Attribut som krävs:
**klass**: &quot;mktoVideo&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Röstning {#poll}

Attribut som krävs:
**klass**: &quot;mktoPoll&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Hänvisning {#referral}

Attribut som krävs:
**klass**: &quot;mktoReferral&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Dragningar {#sweepstakes}

Attribut som krävs:
**klass**: &quot;mktoSweepstakes&quot;
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Exempel:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Redigerbara variabler {#editable-variables}

Alla variabeltyper används genom att referera till värdet för deras id-attribut som omsluts av en ${ }-teckensekvens. De kan användas var som helst i dokumentet, utom i andra variabeldeklarationer.

Exempel:

`${var1}`

**Deklaration:**

Variabler deklareras som metataggar inuti elementet `<head>` i mallen. Det finns tre typer av variabler som kan användas: String, Color och Boolean.

## Sträng {#string}

Attribut som krävs:
**class** : &quot;mktoString&quot;,
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
**standard**: Strängvärde för attributet. Tomt om inget anges.
**allowHTML**: &quot;true&quot; eller &quot;false&quot;. Styr om värdet skrivs ut utan att HTML escape-konverteras. Standardvärdet är &quot;false&quot; om det tas bort.

Exempel:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Exempel med alla attribut:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Färg {#color}

Attribut som krävs:
**class** : &quot;mktoColor&quot;,
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
**standard**: En 7-siffrig HEX-teckenfärgkod. Exempel: &quot;#336699&quot;

Exempel:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Exempel med alla attribut:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Boolean {#boolean}

Attribut som krävs:
**class** : &quot;mktoBoolean&quot;,
**id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
**mktoName** : String. Det här är det visningsnamn som visas i landningssidans redigerare. Det bästa sättet är att använda ett beskrivande namn.

Valfritt:
**standard**: Boolean-sträng. &quot;true&quot; eller &quot;false&quot; kontrollerar om värdet börjar i position ON eller OFF. &quot;false&quot; om inget anges.
**false_value**: Sträng. Det värde som ska infogas för variabeln när den är i AV-positionen. &quot;false&quot; om inget anges.
**true_value**: Sträng. Det värde som ska infogas för variabeln när den är på-positionen. &quot;true&quot; om inget anges.
**false_value_name**: Sträng. Det visningsnamn som ska visas i landningssidans redigerare när värdet är i AV-läge. &quot;AV&quot; om ej angivet.
**true_value_name**: Sträng. Det visningsnamn som ska visas i landningssidans redigerare när värdet är på-positionen. &quot;ON&quot; om inte anges.

Exempel:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Exempel med alla attribut:

I det här exemplet visas ett vanligt användningsfall där en boolesk variabel styr synligheten för ett CSS-element genom att ange värdet för CSS-visningsegenskapen till antingen &quot;block&quot; eller &quot;none&quot; för att visa/dölja ett element med id:t med CSS. Landningssidans redigerare använder visningsnamnet Visa/Dölj i stället för AV/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Programtokens (my.token) kan också användas var som helst på landningssidorna Guidad och Frihandsfigur.
