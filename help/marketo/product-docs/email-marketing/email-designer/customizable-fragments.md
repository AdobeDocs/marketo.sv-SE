---
solution: Marketo Engage
product: marketo
title: Anpassningsbara fragment
description: Lär dig hur du anpassar fragment genom att göra vissa av deras fält redigerbara.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Anpassningsbara fragment {#customizable-fragments}

När fragment används i en e-postmall eller e-postmall låses de som standard på grund av arv. Det innebär att ändringar som görs i ett fragment automatiskt sprids till alla resurser där fragmentet används. Med anpassningsbara fragment kan specifika fält i ett fragment definieras som redigerbara när fragmentet läggs till i en e-post- eller e-postmall. Anta att du har ett fragment med en banderoll, text och en knapp. Du kan ange att vissa fält, t.ex. bild- eller knappens mål-URL, kan redigeras. På så sätt kan användare ändra dessa element när de infogar fragmentet i e-post-/e-postmallen, vilket ger en skräddarsydd upplevelse utan att det ursprungliga fragmentet påverkas.

Genom att utnyttja anpassningsbara fragment kan ni effektivt hantera och personalisera ert innehåll utan att skapa helt nya innehållsblock eller störa arvet från det ursprungliga fragmentet. Detta garanterar att ändringar som görs på fragmentnivån fortfarande sprids, samtidigt som nödvändiga anpassningar kan göras på e-post-/e-postmallnivå.

Både visuella fragment och uttrycksfragment kan markeras som anpassningsbara. Detaljerade instruktioner om hur du fortsätter med varje fragmenttyp finns i avsnitten nedan.

## Lägga till redigerbara fält i visuella fragment {#visual}

Gör så här för att göra delar av ett visuellt fragment redigerbara:

>[!NOTE]
>
>Redigerbara fält kan läggas till i komponenterna **image**, **text** och **button**. För **HTML**-komponenter läggs redigerbara fält till med anpassningsredigeraren, ungefär som uttrycksfragment. [Lär dig hur du lägger till redigerbara fält i HTML-komponenter och uttrycksfragment](#expression)

1. Öppna skärmen för fragmentinnehållsutgåva.

1. Markera den komponent i fragmentet där du vill konfigurera redigerbara fält.

1. Panelen Komponentegenskaper öppnas till höger. Välj fliken **[!UICONTROL Editable fields]** och växla sedan till alternativet **[!UICONTROL Enable edition]**.

1. Alla fält som kan redigeras för den valda komponenten visas i rutan. Vilka fält som är tillgängliga för redigering beror på den valda komponenttypen.

   I exemplet nedan tillåter vi redigering av URL:en för knappen Klicka här.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Klicka på **[!UICONTROL Overview]** om du vill kontrollera alla redigerbara fält och deras standardvärden.

   I det här exemplet visas knappens URL-fält med det standardvärde som definierats i komponenten. Det här värdet kan anpassas av användare efter att de har lagt till fragmentet i innehållet.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Spara ändringarna när du är klar.

När du har lagt till fragmentet i ett e-postmeddelande kan användarna anpassa alla redigerbara fält som är konfigurerade i fragmentet.
<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->
>[!MORELIKETHIS]
>
>[Fragment](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
