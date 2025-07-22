---
unique-page-id: 11385579
description: Skapa innehållsmönster - Marketo Docs - produktdokumentation
title: Skapa innehållsmönster
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Skapa innehållsmönster {#create-content-patterns}

När du anger innehållsmönster identifieras innehållet automatiskt när en webbbesökare klickar på HTML webbsida som är relevant för innehållsmönstret. Det används för att lägga till HTML-sidor (blogginlägg, pressmeddelanden, nyhetsartiklar) som innehållsdelar på sidan Allt innehåll. När automatisk identifiering baseras på innehållsmönster upptäcks och spåras HTML-sidor som är relaterade till det definierade URL-mönstret när en webbbesökare visar eller klickar på en länk till sidan. Innehållsdelen (URL:en, sidnamnet och metadata, inklusive bild-URL:en och beskrivningen) läggs till på sidan Allt innehåll för att färdigställa förutsägbart innehåll. För automatisk identifiering av annat innehåll, som PDF-filer och inbäddad video, måste du [aktivera innehållsidentifiering](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Gå till **[!UICONTROL Content Settings]**.

   ![](assets/settings-dropdown-hand-2.png)

1. Klicka på **[!UICONTROL URL Patterns]**.

   ![](assets/click-url-patterns-hand.png)

1. Klicka på **+** för att öppna en rad där du kan ange dina uppgifter.

   ![](assets/content-settings-create-patterns-hand.png)

1. Lägg till URL-tillägget för domänen där webbsidan finns. Välj kategorin (till exempel [!UICONTROL Blog], [!UICONTROL Article], [!UICONTROL Data Sheet], [!UICONTROL Press Release]).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Objekten i den nedrullningsbara listan till höger återspeglar de kategorier som du angav när du [skapade kategorier](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Klicka på **+** om du vill lägga till en annan sökväg.

   ![](assets/url-patterns-add2.png)

1. Lägg till tillägget och kategorin för den ytterligare sökvägen och klicka på **[!UICONTROL Save]**.

   ![](assets/url-patterns-save.png)

## Innehållsmönsterregler {#content-pattern-rules}

* Du kan använda jokertecken var som helst i ett uttryck (Exempel: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Vi rekommenderar att du använder /&#42; i slutet av ett uttryck för att fortsätta med mönsteridentifieringen (Exempel: _domain.com/blog/&#42;_ upptäcker alla inlägg i bloggmappen)
* Innehållsmönstren är inte skiftlägeskänsliga (Exempel: _domain.com/Blog/&#42;_ identifierar alla HTML-sidor på _domain.com/Blog_ och _domain.com/blog_)

* URL-parametrar identifieras inte (detta undviker att identifiera flera objekt med samma innehålls-URL men olika parametrar)

## Exempel {#examples}

För _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL-mönster</th> 
   <th>Resultat</th> 
  </tr> 
  <tr> 
   <td>blogg/*</td> 
   <td><p>Identifierar allt innehåll som matchar mönstret domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>artikel/2017/*</td> 
   <td><p>Identifierar allt innehåll som matchar mönstret domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
   <td><p>Identifierar alla URL-adresser som innehåller ordet "datablad:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>pressmeddelande</td> 
   <td><p>Endast en exakt matchande HTML-sida hittas:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Om URL-uttrycket är tomt upptäcker URL-mönstret bara hemsidan:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
