---
unique-page-id: 11371040
description: Syntax för e-postmall - Marketo Docs - Produktdokumentation
title: Syntax för e-postmall
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 0%

---

# Syntax för e-postmall {#email-template-syntax}

I Marketo nya e-postupplevelse 2.0 består e-postmallar av valfri kombination av element, variabler, moduler eller behållare. Var och en definieras genom att lägga till Marketo-specifik syntax i din HTML. Gamla (v1.0) e-postmallar stöds i e-postredigeraren 2.0, men inte alla funktioner i den nya redigeraren.

Marketo e-postsyntax fungerar bara i mallar och enskilda e-postmeddelanden. Det fungerar **inte** om det är inbäddat i utdrag eller RTF-token.

>[!NOTE]
>
>Marketo Support har inte konfigurerats för att hjälpa till med CSS/HTML. Om du inte känner till CSS/HTML kontaktar du utvecklaren.

>[!CAUTION]
>
>Klassvärden som innehåller Marketo-syntax (dvs mktoModule, mktoContainer, mktoText) är skiftlägeskänsliga. Anpassade attributnamn (dvs. mktoimgwidth, mktoname) är inte tillåtna.

## Element {#elements}

Element är innehållsområden som du definierar som redigerbara i din e-postmall. Redigeringsupplevelsen av ett element är unik för sin typ och erbjuder ett enkelt sätt att arbeta med innehåll. De möjliga elementen som kan inkluderas i en e-postmall är:

* RTF
* Bilder
* Fragment
* Videor

## RTF {#rich-text}

Om du definierar ett område som RTF kan användare redigera innehållet [med Marketo RTF-redigerare](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Det finns två sätt att definiera ett RTF-element i en e-postmall: mktEditable och mktoText. Kom ihåg att ett RTF-element alltid kan konverteras till ett fragment i e-postredigeraren.

### Alternativ 1 - mktEditable {#option-mkteditable}

Eftersom e-postredigeraren 2.0 är bakåtkompatibel kan vissa gamla e-postmallar ange RTF-element genom att lägga till class=&quot;mktEditable&quot; i alla HTML-element. Detta stöds fortfarande och elementets ID används som visningsnamn i e-postredigeraren.

Attribut som krävs

* **class**: &quot;mktEditable&quot;.
* **id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.

Valfria attribut

* **mktoName** : String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Standardvärde

Innehållet i HTML-elementet (om det finns) med class=&quot;mktEditable&quot; används som standardvärde för Rich Text-elementet.

Exempel:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Alternativ 2 - mktoText {#option-mktotext}

Vi rekommenderar att du anger RTF-element med syntaxen class=&quot;mktoText&quot;. Detta garanterar att det alltid finns ett korrekt visningsnamn för elementet.

Attribut som krävs

* **klass**: &quot;mktoText&quot;
* **id**: ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
* **mktoName** : String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Standardvärde

Innehållet i HTML-elementet (om det finns) med class=&quot;mktoText&quot; används som standardvärde för Rich Text-elementet.

Exempel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Bilder {#images}

Det finns två alternativ för att definiera redigerbara bildelement. Du kan antingen använda en `<div>`, som anger en behållare som `<img>` ska infogas i, eller en `<img>` -tagg. Om du vill att slutanvändaren ska välja en bild som returnerar bild-URL:en (till skillnad från DOM), se&quot;bildvariabler&quot; i avsnittet nedan. Följande två alternativ infogar ett HTML `<img>`-element.

### Alternativ 1 - Använd en `<div>` {#option-use-a-div}

Attribut som krävs

* **klass:** &quot;mktoImg&quot;.
* **id:** ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
* **mktoName :** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **mktoImgClass:** String. Värdet här läggs till i klassattributet för elementet `<img>` inuti div:n.
* **mktoImgSrc:** Används som standardvärde för bilden som placeras i den här diven. En platshållare används om detta utelämnas.
* **mktoImgLink:** Ange att `<img>` ska omges av en `<a>`-tagg med denna mål-URL. Användaren kan ändra detta i e-postredigeraren.
* **mktoImgLinkTarget:** Ange att taggen `<a>` från attributet mktoImgLink ska använda det här målet. Har ingen effekt om mktoImgLink inte också används.
* **mktoImgWidth:** Används som bredd på innesluten `<img>`.
* **mktoImgHeight:** Används som höjd på innesluten `<img>`.
* **mktoLockImgSize:** Används för att låsa upp `<img>`-elementets height- och width-egenskap så att slutanvändaren kan ändra (standard är true om det utelämnas).
* **mktoLockImgStyle:** Används för att låsa stilegenskapen för elementet `<img>` (standardvärdet är false).

Standardvärde (valfritt)

**`<img>`**: Ska användas som `<img>`-elementet som bilden ska placeras i. Användbart om du vill lägga till en textbunden formatering i bilden. Kom ihåg att ta med omgivande `<a> </a>`-taggar, så om användaren lägger till en länk kommer din formatering inte att tas bort!

Exempel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Alternativ 2 - Använd en \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Det här alternativet tillåter inte slutanvändare att lägga till en länk till sina bilder. Använd alternativ 1 om det är viktigt för mallen.

Attribut som krävs

* **klass:** &quot;mktoImg&quot;.
* **id:** ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
* **mktoName:** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.  Standardvärde (valfritt)
* **src:** Ska användas som standardvärde för bilden. En platshållare används om detta utelämnas.
* **mktoLockImgSize:** Används för att låsa upp `<img>`-elementets height- och width-egenskap så att slutanvändaren kan ändra (standard är true om det utelämnas).
* **mktoLockImgStyle:** Används för att låsa stilegenskapen för elementet `<img>` (standardvärdet är false).

Exempel:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Fragment {#snippets}

Om du definierar ett område som ett kodfragment kan slutanvändarna välja vilket godkänt [kodfragment](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)de vill infoga i det här området. Även om RTF-element kan konverteras till fragment i e-postredigeraren, kan de inte konverteras till RTF när du definierar ett område som ett fragment. Du kan ange ett fragmentområde med hjälp av en `<div>` med class=&quot;mktoSnippet&quot;

Attribut som krävs

* **id:** ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
* **mktoName:** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Standardvärde (valfritt)

**mktoDefaultSnippetId**: Det numeriska ID:t för Marketo Snippet som ska visas som standard (fungerar bara om det finns ett fragment med detta ID och det har godkänts på den arbetsytan).

Exempel:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Om du definierar ett område som en video kan slutanvändarna infoga antingen en YouTube- eller Vimeo-webbadress som visas som en miniatyrbild (med uppspelningsknappen) inuti e-postmeddelandet. Du kan ange ett videoområde med en `<div>` med class=&quot;mktoVideo&quot;

Attribut som krävs

* **id:** ID-sträng. Innehåller endast bokstäver, siffror, bindestreck &quot;-&quot; och understreck &quot;_&quot;. Inga blanksteg tillåts. Måste vara unikt.
* **mktoName:** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **mktoImgClass:** String. Värdet här läggs till i klassattributet för videominiatyrbilden `<img>` i div-filen.

Exempel:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variabel {#variables}

Variabler är som tokens. Du definierar dem först i avsnittet `<head>` i din e-postmall med `<meta>` -taggar och använder dem sedan så många gånger som du vill i hela mallen. Eftersom de är definierade i mallen kan slutanvändaren ändra sina värden enligt sina regler. Observera att du kan definiera en variabel som lokal eller global i omfattningen. Om du använder en variabel i en &quot;modul&quot; (se nedan) och en slutanvändare duplicerar den modulen, kommer lokala variabler att ha oberoende värden, medan globala variabler gäller för båda modulerna.

## Sträng {#string}

Om du anger en variabel som en sträng kan slutanvändaren ange text i en textruta i e-postredigeraren. Du anger en strängvariabel med `<meta>` med class=&quot;mktoString&quot;

Attribut som krävs

* **id:** Så här refererar du till variabeln i din e-postmall.
* **mktoName:** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **allowHTML:** Boolean. Styr om variabelns värde är HTML-escape. Standardvärdet är Falskt om det utelämnas.
* **standard**: Standardvärde för strängen. Tom om utelämnad.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Exempel:

`${textHeader}`

## Lista {#list}

Om du anger en variabel som List kan slutanvändaren välja bland en uppsättning värden som du definierar i e-postredigeraren. Du anger en List-variabel med `<meta>` med class=&quot;mktoList&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName:** String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.
* **värden:** Kommaseparerade värdelista. Måste ha minst en sträng.

Valfria attribut

* **standard:** Standardvärde för listrutan Välj. Om det utelämnas används det första värdet från attributet &quot;values&quot;.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Exempel:

`${textFontFamily}`

## Nummer {#number}

Om du anger en variabel som Number kan slutanvändaren ange en siffra i e-postredigeraren. Du anger en Number-variabel med `<meta>` med class=&quot;mktoNumber&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.
* **standard:** Variabelns numeriska standardvärde.

Valfria attribut

* **min:** Minsta tillåtna värde.
* **max:** Högsta tillåtna värde.
* **units:** Enheter som ska läggas till i talvärdet (t.ex. px, pt, em osv.) när de visas i e-postredigeraren, samt i den resulterande koden.
* **steg:** Hur många enheter talvariabeln ska öka/minska med (0,1, 1, 10 osv.). Om det utelämnas blir standardvärdet 1.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> `

Exempel:

`${textFontSize}`

## Färg {#color}

Om du anger en variabel som en färg kan slutanvändaren ange ett hexadecimalt färgvärde eller välja en färg i färgväljaren i e-postredigeraren. Du anger en Color-variabel med `<meta>` med class=&quot;mktoColor&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **standard:** Standardvärde för färgen. 6-siffrig hexfärgkod. Exempel: #ffffff.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Exempel:

`${textColor}`

## Boolean {#boolean}

Om du anger en variabel som Boolean kan slutanvändaren aktivera/inaktivera alternativet i e-postredigeraren. Du anger en boolesk variabel med hjälp av `<meta>` med class=&quot;mktoBoolean&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **standard:** Ett booleskt värde som fastställer växlingens standardläge. Falskt om det utelämnas.
* **false_value:** Värde som ska infogas när växlingen är i AV-läge. Falskt om det utelämnas.
* **true_value:** Värde som ska infogas när växlingen är på plats. True om det utelämnas.
* **false_value_name:** Gränssnittet visas i växlingsläget när det är inaktiverat. Falskt om det utelämnas.
* **true_value_name:** Gränssnittet visas i växlingsläget när det är på plats. True om det utelämnas.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Exempel:

`${showFooter}`

## HTML Block {#html-block}

Om du anger en variabel som ett HTML-block kan slutanvändaren mata in ordagrant HTML inifrån e-postredigeraren. Du anger en HTML Block-variabel med `<meta>` med class=&quot;mktoHTML&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **standard:** HTML-kodat värde som fungerar som standardinnehåll i blocket.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Exempel:

`${trackingPixel}`

## Bildvariabel {#image-variable}

Om du anger en variabel som en bild kan slutanvändaren välja en bild i bildväljaren i e-postredigeraren. Den valda bild-URL:en är variabelns värde. Du anger en bildvariabel med `<meta>` med class=&quot;mktoImg&quot;

Attribut som krävs

* **id**: Så här refererar du till variabeln i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **standard:** Elementets standardbild-URL.
* **mktoModuleScope**: Boolean. Kontrollerar om variabeln är lokal (true) eller global (false) när den används i en modul. Standardvärdet är Falskt om det utelämnas.

Exempeldeklaration:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Exempel:

`${heroBackgroundImage}`

## Moduler {#modules}

Moduler är mallavsnitt som definieras på mallnivå och som visas för slutanvändare så att de kan infoga dem i sina e-postmeddelanden. Eftersom du har skapat de här modulerna kan du se till att de interagerar med resten av ditt e-postinnehåll på ett smidigt sätt (på ett helt responsivt sätt). Du kan bara placera en modul i en behållare.

>[!IMPORTANT]
>
>När ett e-postmeddelande genereras från en e-postmall som innehåller definierade modulkomponenter skickas **inte** ändringar som gjorts i mallens moduler till det meddelandet.

**För behållare av typen `<table>`, `<tbody>`, `<thead>` eller `<tfoot>`:**

Anges med `<tr>` med class=&quot;mktoModule&quot;

**För behållare av typen `<td>`:**

Anges med `<table>` med class=&quot;mktoModule&quot;

Attribut som krävs

* **id**: Så här refererar du till modulen i din e-postmall.
* **mktoName**: String. Det här är det visningsnamn som visas i e-postredigeraren 2.0. Det bästa sättet är att använda ett beskrivande namn.

Valfria attribut

* **mktoActive:** Avgör om den här modulen visas i listan med moduler i e-postredigeraren. Standardvärdet är true. Om värdet är false kan modulen inte läggas till av en slutanvändare i ett e-postmeddelande.
* **mktoAddByDefault:** Avgör om den här modulen kommer att finnas på arbetsytan i ett nytt e-postmeddelande som använder mallen när den skapas. Standardvärdet är true (om mktoActive är false ignoreras det här värdet).

>[!NOTE]
>
>Klassvärden som innehåller Marketo-syntax (dvs mktoModule, mktoContainer, mktoText) är skiftlägeskänsliga. Anpassade attributnamn (dvs. mktoimgwidth, mktoname) är inte tillåtna.

## Behållare {#containers}

En behållare innehåller moduler och definierar var de kan placeras. När slutanvändarna sorterar om och infogar moduler i sina e-postmeddelanden styr behållaren vart de kan gå.

**Anges med antingen `<table>`, `<tbody>`, `<thead>`, `<tfoot>` eller `<td>` med class=&quot;mktoContainer&quot;**

Attribut som krävs

**id**: Så här refererar du till modulen i din e-postmall.

>[!CAUTION]
>
>Behållare kan bara innehålla moduler - om det finns något annat, anses behållaren vara ogiltig! Endast en behållare tillåts per mall.
