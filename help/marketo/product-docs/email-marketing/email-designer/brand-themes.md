---
solution: Marketo Engage
product: marketo
title: Varumärkesteman
description: Lär dig hur du skapar och hanterar riktlinjer för varumärken.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: e6b576e5-3456-4bee-9383-b63cd6728620
source-git-commit: 2f0ac66406a0e9d077ce784f8b2492cdbe21fe30
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 0%

---

# Varumärkesteman {#brand-themes}

Med varumärkesteman kan du enkelt skapa återanvändbart innehåll som passar ett visst varumärke och designspråk genom att lägga in egen formatering i e-postmallarna.

Den här funktionen gör att marknadsförarna kan använda visuellt tilltalande, varumärkesenhetliga e-postmeddelanden snabbare och enklare, samtidigt som de erbjuder avancerade anpassningsalternativ för unika designbehov.

## Saker att notera {#things-to-note}

* När du skapar ett e-postmeddelande från grunden kan du välja att börja bygga ditt innehåll med ett tema för att snabbt tillämpa en specifik formatering som passar ert varumärke och er design. Om du väljer läget Klassisk kan du inte använda några teman om du inte återställer e-postmeddelandet.

* Fragment är inte korskompatibla mellan teman och klassiska lägen. Om du vill kunna använda ett fragment i ett innehåll där ett tema används måste det skapas i temaläget.

* Uppdatering av ett tema kommer inte automatiskt att överlappa alla resurser som använder dem. Du måste redigera enskilda objekt för att kunna uppdatera temat.

* När du tar bort teman påverkas inte resurserna som använder dem.

## Skapa ett varumärkestema {#create-a-brand-theme}

1. Följ stegen för att [skapa en e-postmall](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template).

1. Välj _Skapa eller redigera teman_ på skärmen **Utforma mallen**.

   ![](assets/brand-themes-1.png)

1. Välj standardtemat som bas att skapa från grunden och klicka på **Skapa**.

   ![](assets/brand-themes-2.png)

1. Arbetsytan öppnas så att du kan redigera olika delar av temat.

   ![](assets/brand-themes-3.png)

## Inställningar

Alla inställningsalternativ är tillgängliga via ikonerna till höger. Låt oss granska var och en av dem.

![](assets/brand-themes-4.png)

### Allmänna inställningar {#general-settings}

Ge temat ett namn och justera visningsrutans storlek.

![](assets/brand-themes-5.png)

### Färger {#colors}

När du gör färgjusteringar bör du observera de ändringar som görs på huvudpanelen.

![](assets/brand-themes-6.png)

>[!NOTE]
>
>En uppsättning färgrutor har redan konfigurerats för dig baserat på standardtemat.

Klicka på **Redigera**.

![](assets/brand-themes-7.png)

Du kan välja mellan en förinställning eller konfigurera varje färg i uppsättningen separat. Om du väljer paletten blir dessa färger tillgängliga under de olika färginställningarna senare.

![](assets/brand-themes-8.png)

När du är klar med redigeringen klickar du på bakåtpilen (![bakåtpilen ](assets/icon-back-arrow.png)) för att gå tillbaka.

Om du vill redigera en variant klickar du på pennikonen.

![](assets/brand-themes-9.png)

>[!NOTE]
>
>Du kan skapa upp till sex varianter.

Det finns flera tillgängliga element som du kan anpassa. Variantinställningar grupperas i följande kategorier:

* Allmänt
* Rubriker
* Stycken
* Knappar

**Allmänt**

Med de här inställningarna kan du ange färger för brödtext, strukturer, bakgrunder, behållare, bilder med mera.

![](assets/brand-themes-10.png)

**Rubrik**

Ange text- och kantfärger för varje rubriktyp, från Rubrik 1 till Rubrik 6.

![](assets/brand-themes-11.png)

**Stycke**

Ange text- och kantfärger för upp till tre stycketyper.

![](assets/brand-themes-12.png)

**Knappar**

Ange fyllnings-, kant- och textfärg för tre olika knapptyper: Primär, Sekundär och Högre.

![](assets/brand-themes-13.png)

### Textinställningar {#text-settings}

Ange teckensnittstyper och storlekar för globala rubriker och stycken.

![](assets/brand-themes-14.png)

**Global**

Välj mellan Standard- eller Google-teckensnittsbibliotek och deras respektive teckensnittsfamiljer.

![](assets/brand-themes-15.png)

**Rubriker**

Ange teckensnittsbibliotek, familj, storlek, textformat och textjusteringar för olika rubriktyper.

![](assets/brand-themes-16.png)

**Stycken**

Ange teckensnittsbibliotek, familj, storlek, textformat och textjusteringar för olika styckeförinställningar.

![](assets/brand-themes-17.png)

### Mellanrum och kantlinje {#spacing-and-border}

Under det här alternativet kan du ange utfyllnad och marginal för olika typer av struktur eller knapp.  Välj typ i den första listrutan och fortsätt sedan att ange utfyllnad och/eller marginal för det elementet. Upprepa den här i ett steg om det behövs.

SCREENSHOT

Typer av strukturer är följande:

SCREENSHOT

Inställningar för ett exempelelement, till exempel Behållare.

Marginaler

SCREENSHOT

Utfyllnad

SCREENSHOT

Hörn

SCREENSHOT

Kantlinjer

Visa alternativ för storlek, format och position genom att växla ramen till PÅ.

SCREENSHOT

Alternativ för format

SCREENSHOT

Exempel på effekter för format i rutan

```
TABLE

Type

Size and Style setting

Effect

Dashed

Dotted

Solid
```

Justera om ramen visas eller döljs med hjälp av kantlinjeposition

Exempel: Överkanten är dold i exemplet nedan.

```
TABLE

Position setting

Effect
```

Upprepa inställningarna för inställning av marginal, utfyllnad, hörn och kantlinjer för olika typer av strukturer.

### Knappinställningar {#button-settings}

Under det här alternativet kan du ange olika element för knappar (andra än färg), som knappform, knappradie, knapptext och knappstorlekar. Du kan ange dessa för tre förinställningar - primär, sekundär och tertiär.

SCREENSHOT

```
TABLE

Primary/Secondary/Tertiary    Allows settings for 3 presets of button configurations
Text > Font Library    Font library choice for button text
Text > Font family    Font family choice for button text
Text > Font size    Font size for button text
Text > Text styles    Text style (bold, italicized, underlined, strikethrough) for button text
Text > Text alignment    Alignment for button text
Border> Border size     Button border thickness
Border> Border style    Button border style (dashed, solid, dotted, etc.)
Border> Border radius    Button border corner curvature
SIZE > Height    Height setting for the button
SIZE > Width    Width setting for the button
```

### Delningsinställningar {#divider-settings}

I det här exemplet kan du ange inställningar för linjetyp och behållarinställningar för avgränsare.

SCREENSHOT

### Stödrasterinställningar {#grid-settings}

Använd kolumnmellanrum för att styra mellanrummet i rutnätet.

```
TABLE
```

Klicka på Spara när du är klar.

SCREENSHOT

## Redigera varumärkesteman {#editing-brand-themes}

Det går att skapa märkesteman på mallpanelen i redigeraren. Du kan nå den här panelen när du skapar en ny mall eller i Ändra design inifrån redigeraren.

SCREENSHOT

Klicka på Ändra din design.

SCREENSHOT

Klicka på Skapa eller redigera teman

SCREENSHOT

Välj Egna teman om du vill visa en lista med anpassade teman som skapats i din organisation. Välj ett tema och klicka på Redigera.

SCREENSHOT

Arbetsytan är nu öppen för redigering.

SCREENSHOT

Ändra inställningarna under avsnitten till höger.

SCREENSHOT

Klicka på Spara när du är klar.

SCREENSHOT

## Använda varumärkesteman {#using-brand-themes}

De varumärkesteman som skapas/redigeras är klara att användas för e-post, e-postmallar och fragment.

Adobe Marketo Engage: De varumärkesteman som skapas/redigeras är klara att användas för e-post, e-postmallar och fragment som skapas med den nya e-postredigeraren.

Du kan skapa strukturer och komponenter i redigeraren och tillämpa vilket varumärke som helst och någon av deras varianter.

### I dina e-postmeddelanden {#in-your-emails}

Skapa e-postmallar från grunden

* Börja med&quot;Skapa e-post&quot;/&quot;Skapa e-postmall&quot; och välj alternativet&quot;Designa från grunden&quot;

* Välj Använd teman i modalen som visas

SCREENSHOT

Obs! Det är bara den e-postadress som skapas med det här alternativet som kan utnyttja de varumärkesteman som definierats i föregående avsnitt

* Det här nya alternativet visas till höger, vilket gör att du kan använda varumärkesteman i ditt e-postmeddelande

SCREENSHOT

* Du kan välja bland teman från Adobe eller egna teman som skapats för dina varumärken

SCREENSHOT

* Designa e-postinnehåll på arbetsytan och välj ett tema som ska användas på innehållet

* Ett e-postmeddelande får endast innehålla ett varumärkestema

* För alla komponenter som skapas i den här resursen kan du använda något av de formatalternativ som är tillgängliga i temat från fliken Stilar i den högra rutan

* t.ex. kan en CTA konfigureras som primär/sekundär/tertiär

SCREENSHOT

* Du kan t.ex. markera en textkomponent om du vill använda någon av rubrikerna/styckeformaten enligt temat

SCREENSHOT

* Observera att nu ser det annorlunda ut på fliken Stil jämfört med ett vanligt e-postmeddelande med manuell formatering där det finns mer kreativ frihet att formatera en komponent

### Skapa e-post-/e-postmallar från en mall

* Du kan använda teman när du skapar en e-postmall eller e-postmall från en befintlig e-postmall som också skapades med teman

* Börja med Skapa e-post/Skapa e-postmall och välj en av e-postmallarna som skapats med teman i avsnittet Sparade mallar

* Nu används temat som används i den sparade e-postmallen automatiskt

SCREENSHOT

* Du kan också ändra temat i den här e-postmallen via alternativet Teman i det högra fältet

SCREENSHOT

* Du kan också använda valfri variant av ett tema för innehållet

SCREENSHOT

SCREENSHOT

### I dina fragment {#in-your-fragments}

Börja med Skapa nytt fragment

Välj önskat tema och använd samma tema från alternativet &quot;Teman&quot; i den högra sidlisten

SCREENSHOT

Allt fragmentinnehåll som skapas på arbetsytan därefter kommer att anta det valda temat

Du kan också använda valfri variant av ett tema för innehållet

När det här fragmentet har publicerats kan det användas i alla e-postmallar som skapas med teman
