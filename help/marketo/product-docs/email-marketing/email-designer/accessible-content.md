---
title: Utforma tillgängligt innehåll
description: Lär dig hur du utformar tillgängligt innehåll för e-postmeddelanden i Marketo Engage.
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: e-post, design, tillgänglighet
source-git-commit: 753455b40ead039a56c595fa61ab9a95b7936382
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# Utforma tillgängligt innehåll {#accessible-content}

Den [europeiska tillgänglighetslagen](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"} är ett direktiv som är utformat för att förbättra den inre marknaden för tillgängliga produkter och tjänster genom att eliminera hinder som orsakas av olika nationella regler i medlemsstaterna.

I den här förordningen står det att all digital kommunikation, inklusive e-post, nyhetsbrev, PDF-filer och nedladdningsbart innehåll, bör vara tillgänglig. När du skapar innehåll för dina mottagare måste du därför följa särskilda riktlinjer, t.ex. använda hjälpmedelsanpassade teckensnitt och läsbara format, samt tillhandahålla alternativ text för bilder.

Med Marketo Engage Email Designer kan du enkelt följa det här direktivet, baserat på Web Content Accessibility Guidelines (WCAG) 2.1, nivå AA. De bästa sätten att utforma hjälpmedelsanpassat innehåll med Marketo Engage listas nedan.

>[!NOTE]
>
>Den här sidan handlar om att göra ditt innehåll tillgängligt för alla mottagare, så att personer med funktionshinder kan läsa, förstå och interagera med e-postmeddelanden som skapats i Marketo Engage.

## Säkra textläsbarhet {#text-readability}

Utnyttja fliken **[!UICONTROL Styles]** i komponenten **[!UICONTROL Text]** för att säkerställa att texten är läsbar, till exempel genom att använda rätt färgkontrast och enkla teckensnitt.

<!--![](assets/accessible-text-styles.png){width="80%"}-->

För teckensnitt och text måste du följa dessa riktlinjer:

**Val av teckensnitt**

* Använd sans-serif-teckensnitt som Arial, Verdana, Tahoma, Helvetica eller Open Sans.
* Undvik serif-, cursive- och dekorativa teckensnitt i brödtextinnehållet.
* Behåll en begränsad teckensnittsuppsättning för konsekvens och reservteckensnitt (till exempel: `font-family: Arial, Helvetica, sans-serif;`).

**Teckensnittsstorlek**

* Se till att teckensnittsstorleken är minst 16px för brödtext.
* Använd rätt hierarki för rubriker.

**Färgkontrast**

* Behåll ett kontrastförhållande på minst 4,5:1 mellan text och bakgrund.
* För stor text (≥24px eller fet 18px) måste du se till att kontrasten är minst 3:1.
* Undvik ljusgrå eller pastelltext på vita bakgrunder.
* Förlita dig inte på enbart färg för att förmedla innebörden. Använd understrykning, ikoner osv.

**Texttillgänglighet**

* Undvik text i bilder.
* Använd inte versaler i brödtexten.
* Se till att texten kan zoomas upp till 200 % utan att layouten bryts.

## Säkerställ visuell tillgänglighet {#visual-accessibility}

* Undvik att använda färgbara indikatorer för viktig information.
* Använd textetiketter eller ikoner för att få tydlighet.
* Optimera designen för mobil och responsiv layout och se till att knapparna är stora och har rätt avstånd.
* Testa regelbundet olika enheter och skärmstorlekar för att bevara tillgängligheten.

I Marketo Engage kan storleken och mellanrummet för de olika elementen i ditt innehåll förfinas ytterligare med formatparametrar och attribut från e-postfönstret i Designer **[!UICONTROL Styles]**.

Du kan till exempel uppdatera bakgrunden eller ändra marginalerna, utfyllnaden och justeringen för att förbättra den visuella tillgängligheten.

<!--![](assets/accessible-styles.png){width="80%"}-->

Med Marketo Engage Email Designer kan du förhandsgranska och optimera designen för olika enheter och skärmstorlekar. Du kan när som helst **[!UICONTROL Switch to live view]** kontrollera hur ditt innehåll kan återges på olika enhetsstorlekar.

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>Live-vyn är en allmän förhandsvisning som är utformad för att jämföra hur innehållet kan återges på olika enhetsstorlekar. Den slutliga återgivningen kan variera beroende på mottagarens e-postklient.

## Använd alternativ text för bilder {#alt-text}

Använd komponenten **[!UICONTROL Image]** för att ange alternativ text för bilder.

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* Beskriv syftet med bilden kortfattat och i sitt sammanhang.
* Undvik överflödiga fraser som &quot;Bild av ...&quot; och använd tom alt-text för dekorativa bilder.
* För ikoner med betydelse, ange meningsfulla etiketter och för komplexa bilder använder du en kort alternativ text plus en längre beskrivning någon annanstans.

## Använd läsbart format {#readable-format}

Använd e-postens relevanta struktur- och innehållskomponenter för Designer, samt alternativen i **[!UICONTROL Styles]**-rutan, för att ordna ditt innehåll på ett tydligt, logiskt och koncist sätt som är tillgängligt för alla.

<!--![](assets/accessible-components.png){width="100%"}-->

* Använd strukturerad, semantisk HTML med rätt rubriker, stycken, listor och tabeller.
* Kontrollera att innehållet följer ett logiskt flöde från vänster till höger, uppifrån och ned.
* Använd klart och koncist språk.
* Ange alternativa format för PDF:er och infografik.
* Tillåt storleksändring och omformning av text och se till att typografin är läsbar med tillräcklig färgkontrast i alla format.

## Säkerställ läsbarhet {#readability}

För att innehållet ska vara läsbart måste det vara klart, välstrukturerat och användbart för alla, även personer med visuella, kognitiva eller läsrelaterade problem, och personer som använder hjälpmedelstekniker. Några saker du bör tänka på när du skapar hjälpmedelsanpassat innehåll är:

* Behåll meningar till 20 ord eller mindre.
* Redigera texten så att den blir direkt och koncis.
* Använd aktiv röst för att förenkla meningsbyggnaden.
* Undvik slang, jargon och regionala ord som vissa kanske inte känner till.

Om du vill utvärdera läsbarheten för e-post kan du använda det populära [Flesch Reading Ease-testet](https://support.microsoft.com/en-us/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"} som finns i Microsoft Word och som beräknar hur enkelt innehållet är att läsa på en skala från 0 till 100.

## Testa innehållet {#test}

Om du vill verifiera innehållets tillgänglighet kan du använda testfunktionerna i Marketo Engage. De är inte särskilt utformade för att kontrollera om ditt innehåll är fullt tillgängligt, men de kan tillhandahålla en första verifieringsnivå.

* Förhandsgranska innehållet med testprofiler.

* Använd alternativet [Återgivning via e-post](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"} som använder Litmus för att simulera dina designer för de vanligaste e-postklienterna (Apple Mail, Gmail, Outlook) och se om text, färger och bilder gör ditt innehåll tillgängligt. <!--Litmus includes accessibility testing-->

* Skicka korrektur för att testa återgivningen av materialet innan det skickas till den verkliga målgruppen.

<!--![](assets/accessible-simulate.png){width="90%"}-->

Om du vill kontrollera på ett mer konsekvent sätt om innehållet är tillgängligt kan du gå till särskilda externa verktyg som:

* Kontrastkontrollen [WebAim](https://webaim.org/resources/contrastchecker/){target="_blank"} och verktyget [WAVE för utvärdering av webbtillgänglighet](https://wave.webaim.org/){target="_blank"} för utvärdering av kontrast och efterlevnad.

* Hjälpmedelstekniker som skärmläsare (till exempel: [NVDA](https://www.nvaccess.org/download/){target="_blank"} eller [VoiceOver](https://support.apple.com/en-ie/guide/iphone/iph3e2e415f/ios){target="_blank"} på iPhone) för att få e-post från synskadade användare.

## Använd mörkt läge {#dark-mode}

[Mörkt läge](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"} förbättrar den visuella tillgängligheten för användare med ljuskänslighet eller synnedsättning, vilket ger en förbättrad visningsupplevelse.

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

Några av de bästa sätten att utforma innehåll i mörkt läge är:

* Använda genomskinliga PNG- eller SVG-filer
* Ange lämpliga metataggar och CSS
* Erbjuder hjälpmedelsanpassad grundformatering om mörkt läge inte stöds.

Se till att dina e-postmeddelanden återges korrekt i mörkt läge genom att testa allt e-postinnehåll och gränssnittselement i både ljust och mörkt läge.

## Använd specifika attribut för tillgänglighet {#attributes}

### Språkattribut {#language}

När du skapar designer inkluderar du attributen `lang` (språk) och `dir` (textorientering) i innehållets brödtext. Dessa attribut hjälper hjälpmedelstekniker (t.ex. skärmläsare) att tolka och presentera ditt innehåll på rätt sätt.

* Attributet `lang` anger språket i e-postmeddelandet som ska användas till hjälpmedelstekniker, vilket säkerställer att orden uttalas korrekt.

  +++Exempel

  Exempel på engelska:

  ```
  <body lang="en">
  ```

  Exempel för franska:

  ```
  <body lang="fr">
  ```

  +++

* Attributet `dir` anger textriktningen. De flesta språk, inklusive engelska och franska, läses från vänster till höger (ltr), medan språk som arabiska och hebreiska läses från höger till vänster (rtl).

  +++Exempel

  Exempel för engelska (vänster till höger):

  ```html
  <body lang="en" dir="ltr">
  ```

  Exempel för arabiska (höger till vänster):

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

Skärmläsare förlitar sig på attributet `lang` för att använda rätt uttydningsregler, medan textriktning garanterar att innehållet flödar naturligt för språk som läses från vänster till höger eller från höger till vänster. Utan dessa attribut kan användare uppleva förvirrande läsordning eller feluttal. Radbryt alltid din e-postbrödtext med rätt `lang`- och `dir`-attribut.

>[!TIP]
>
>Om e-postmeddelandet innehåller flera språk tilldelar du lämpliga språkattribut till specifika avsnitt (t.ex. `<table>` eller `<td>` block) för att säkerställa att varje del läses korrekt.

### Tabeller {#tables}

I HTML-innehåll används ofta tabeller för layout. Som standard behandlar skärmläsare varje `<table>` som en datatabell, där rader, kolumner och struktur presenteras. Detta kan vara förvirrande om tabellen bara används för formatering.

Lägg till `role="presentation"` (eller `role="none"`) i layouttabeller för att säkerställa att hjälpmedelstekniker hoppar över sin struktur och bara fokuserar på det faktiska innehållet.

+++Exempel - Layouttabell (med `role="presentation"`)

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

Skärmläsarna läser:
&quot;Hello World. Välkommen till vårt nyhetsbrev.&quot; _(Ingen uppgift om rader, kolumner eller tabell)_

+++

+++Exempel - Datatabell (utan `role="presentation"`)

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

Skärmläsarna läser:
&quot;Tabell med 2 kolumner och 3 rader.&quot;

&quot;Namn, Peter. Poäng, 19.&quot;

&quot;Namn, parker. Poäng, 62.&quot;

+++

>[!TIP]
>
>Använd `role="presentation"` exklusivt för layouttabeller. Behåll den semantiska `<table>`-strukturen för datatabeller så att skärmläsare kan meddela rubriker och relationer korrekt.

### Text för länkar {#links}

Skärmläsare läser upp länkar med sin text. Om en länk endast heter&quot;Klicka här&quot; eller&quot;Läs mer&quot; kommer användare av hjälpmedelstekniker inte att känna till målet. För att säkerställa tillgänglighet behöver de beskrivande text som tydligt anger målet eller åtgärden.

Använd e-post-Designer för att lägga till en länk till ditt innehåll och redigera etiketten så att den blir urskiljbar (synlig) och beskrivande (tydlig om syftet). Undvik otydliga etiketter som &quot;here&quot; eller &quot;more&quot;.

<!--![](assets/accessible-link.png){width="70%"}-->

+++Exempel - Bra länk (beskrivande): 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

Skärmläsarna läser:
&quot;Link, August release notes.&quot;

+++

+++Exempel - felaktig länk (inte beskrivande)

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

Skärmläsarna läser:
&quot;Länk, klicka här.&quot; *(Ingen kontext ligger utanför läsordningen)*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
