---
description: Mörkt läge - Marketo Docs - produktdokumentation
title: Mörkt läge
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 77008ff8d8f7c577f48b508737e1b8eb2ac1e5ce
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 0%

---

# Mörkt läge {#dark-mode}

När du utformar dina e-postmeddelanden kan du växla till vyn **[!UICONTROL Dark mode]** med e-post-Designer.

I **[!UICONTROL Dark mode]** kan du definiera specifika anpassade inställningar som ska visas med stöd för e-postklienter när deras mörka läge är aktiverat.

## Vad är mörkt läge? {#what-is-dark-mode}

I mörkt läge kan e-postklienter och appar som stöder e-post visa e-postmeddelanden med mörkare bakgrund och ljusare färger för text, knappar och andra gränssnittselement. Den minskar ögonbelastningen, sparar batteritid och förbättrar läsbarheten i miljöer med svag belysning för en mer bekväm visning.

## Guardrails {#guardrails}

Återgivning i mörkt läge kan variera avsevärt i olika e-postklienter.

Innan du använder mörkt läge är det viktigt att du förstår hur huvudklienterna för e-post hanterar det. Det finns tre olika fall att skilja mellan:

### Klienter som inte stöder mörkt läge {#not-supporting}

Vissa e-postklienter stöder inte den här funktionen alls, till exempel:

* Yahoo!Mail
* AOL

Vare sig du definierar anpassade inställningar för mörkt läge eller inte visas ingen återgivning i mörkt läge av dessa e-postklienter.

### Klienter som använder sitt eget mörka läge {#default-support}

Vissa e-postklienter tillämpar systematiskt sitt eget mörka standardläge för alla e-postmeddelanden som tas emot. Färger, bakgrunder, bilder osv. justeras automatiskt med inställningar för mörkt läge som är specifika för den e-postklienten. Det går inte att ändra externt.

Några exempel är:

* Gmail (Desktop Webmail, iOS, Android, Mobile Webmail)
* Outlook Windows
* Outlook Windows Mail

I det här fallet, om du definierar anpassade mörkt läge-inställningar i e-post-Designer, åsidosätts dessa inställningar av e-postklientens inställningar.

Så även om dessa e-postklienter hanterar mörkt läge renderas inte din specifika design för mörkt läge.

### Klienter som stöder anpassat mörkt läge {#custom-dark-mode}

Vissa e-postklienter har möjlighet att återge anpassat mörkt läge med frågan `@media (prefers-color-scheme: dark)`, som är den metod som används av Designer-e-postprogrammet i [!DNL Marketo Engage] .

De huvudklienter som hanterar det här alternativet är:

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

De inställningar du anger i e-post-Designer ska visas.

>[!NOTE]
>
>Lär dig hur du definierar [anpassade inställningar för mörkt läge](#define-custom-dark-mode) i e-post-Designer.

Vissa begränsningar kan gälla för varje e-postklient. Vissa klienter (t.ex. Apple Mail 16) kommer inte att generera ett mörkt läge om det finns bilder.

Testa innehållet i de e-postklienter du riktar in dig på för att få optimala resultat. Om du vill se en simulering i varje klient använder du funktionen [E-poståtergivning](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) i Designer för e-post.

## Mörkt läge i e-post-Designer {#dark-mode-email-designer}

När det gäller det mörka läget i e-post-Designer finns det två aspekter att tänka på:

* Du kan få en förhandsvisning av hur det mörka standardläget kommer att återges i de flesta e-postklienter som stöds. [Läs mer](#preview-dark-mode)

* Om du vill åsidosätta standardinställningarna för stöd av e-postklienter kan du definiera anpassade inställningar för mörkt läge i det e-postmeddelande som du redigerar. [Läs mer](#define-custom-dark-mode)

### Förhandsvisa standardläget för mörk {#preview-dark-mode}

Lär dig hur du kommer åt mörkt läge i e-post-Designer och får en förhandsvisning av standardinställningarna för mörkt läge.

1. Välj alternativet **[!UICONTROL Design from scratch]** på hemsidan för e-post till Designer.

1. Lägg till [strukturer och innehåll](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content) i e-postmeddelandet.

1. Aktivera alternativet **[!UICONTROL Dark mode]** längst upp till höger.

   ![](assets/dark-mode-1.png)

1. Standardförhandsvisningen i mörkt läge visas.

   ![](assets/dark-mode-2.png)

Som standard används färgschemat&quot;Fullfärgsinvertering&quot; för alla element utom bilder och ikoner i förhandsvisningen av Designer i mörkt läge.

Det innebär att områden med ljusa och mörka element identifieras och inverteras så att ljusa bakgrunder blir mörka och mörk text blir ljusa, medan mörka bakgrunder blir ljusa och ljusa text blir mörka.

>[!CAUTION]
>
>Den slutliga återgivningen kan variera beroende på mottagarens e-postklient. Om du vill se en simulering för varje e-postklient använder du funktionen [E-poståtergivning](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) .

### Definiera anpassat mörkt läge {#define-custom-dark-mode}

När du har växlat till **[!UICONTROL Dark mode]** kan du välja att redigera specifika formatelement för ditt innehåll som bara visas när mörkt läge är aktiverat i mottagarens e-postklient (förutsatt att det har stöd för den funktionen).

>[!IMPORTANT]
>
>Den slutliga återgivningen i mörkt läge beror på varje e-postklient, så resultatet kan variera från en klient till en annan. [Läs mer](#guardrails)

Marketo Engage använder CSS-frågan `@media (prefers-color-scheme: dark)` som identifierar om användarens e-postklient är inställd på mörkt läge och använder den design med mörka teman som definierats i ditt e-postmeddelande för att utnyttja den anpassade stilen för mörkt läge i Designer.

Följ stegen nedan för att definiera egna inställningar för mörkt läge.

1. Växla till [Förhandsvisning i mörkt läge](#preview-dark-mode) i e-post-Designer.

1. Redigera formatfärgattribut som text, bakgrunder, knappar etc.

1. Du kan inte ändra färgerna på bilder och ikoner, men du kan definiera specifika resurser enbart för mörkt läge. Markera en bild om du vill göra det. Växla till **[!UICONTROL Dark mode]** med den dedikerade växlingsknappen i rutan **[!UICONTROL Settings]** och välj en annan resurs.

   ![](assets/dark-mode-3.png)

1. Du kan när som helst **[!UICONTROL Switch to live view]** för att se hur ditt innehåll kan återges på olika enhetsstorlekar. I den här vyn väljer du alternativet Mörkt läge om du vill förhandsvisa den mörka lägesversionen av ditt innehåll på olika enheter.

   ![](assets/dark-mode-4.png)

   >[!NOTE]
   >
   >Live-vyn är en allmän förhandsvisning som är utformad för att jämföra hur återgivningen kan se ut på olika enhetsstorlekar. Den slutliga återgivningen kan variera beroende på mottagarens e-postklient.

1. När du är nöjd med ändringarna för mörkt läge klickar du på **[!UICONTROL Simulate Content]**.

   ![](assets/dark-mode-5.png)

1. Välj **[!UICONTROL Render email]** och anslut till ditt Litmus-konto. Du kan se den slutliga återgivningen i mörkt läge för olika e-postklienter. Läs mer om [E-poståtergivning](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

   >[!IMPORTANT]
   >
   >Simuleringen simulerar i hög grad hur e-postmeddelanden kommer att se ut i mörkt läge, men den faktiska återgivningen kan variera beroende på variationer i e-postleverantörer eller enhetsinställningar.

## Bästa praxis {#best-practices}

Efterhand som användningen av mörkt läge ökar för alla större e-postklienter är det viktigt att tänka på hur dina e-postmeddelanden återges i både ljusa och mörka miljöer, oavsett om du använder [anpassat mörkt läge](#define-custom-dark-mode) eller inte.

Mörkt läge kan ändra färger, bakgrunder och bilder, och ibland åsidosätta designalternativ. För att säkerställa visuell enhetlighet, tillgänglighet och varumärkesintegritet följer du de bästa metoderna nedan.

**Optimera bilder och logotyper**

* Spara logotyper och ikoner som PNG-filer med genomskinliga bakgrunder för att undvika synliga vita rutor i mörkt läge.

* Undvik bilder med hårdkodade vita eller ljusa bakgrunder.

* Om genomskinlighet inte är ett alternativ kan du placera bilder på en solid bakgrund i designen för att förhindra otydliga färgförändringar.

**Se dina bakgrunder**

* Se till att det finns tillräcklig kontrast mellan text och bakgrundsfärger för läsbarhet i både ljust och mörkt läge.

* Undvik att använda enbart bakgrundsfärger för viktigt innehåll. Vissa klienter åsidosätter bakgrundsfärger i mörkt läge, så se till att viktig information fortfarande visas.

**Designa hjälpmedelsanpassat innehåll i mörkt läge**

* Använd färgkombinationer som är enkla att skilja på för färgblinda.

* Använd en mellantonspalett för att säkerställa kontrast mot både ljusa och mörka bakgrunder.

* Använd tillgängliga färgkombinationer med hög kontrast för att förbättra läsbarheten och följa WCAG-standarderna (Web Content Accessibility Guidelines). Använd verktyg som Kontrast i Kontrast i WebAIM för att kontrollera färgkontrasten.

* Undvik tunna teckensnitt eftersom det kan påverka läsbarheten. Om ert varumärke kräver ett tunt teckensnitt kan du fet stil i mörkt läge.

* Hoppa över rent vitt på rent svart eftersom det kan orsaka ögonproblem och kan inverteras automatiskt av vissa e-postklienter.

* Ange hjälpmedelsanpassad grundformatering om mörkt läge inte stöds.

**Testa dina e-postmeddelanden i mörkt läge**

* Använd Designer [förhandsvisning i mörkt läge](#preview-dark-mode) som använder inverterade färgscheman för att upptäcka problem tidigt.

* Använd funktionen [E-poståtergivning](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) som använder Litmus för att simulera dina designer för de vanligaste e-postklienterna och se hur färger och bilder beter sig i mörkt läge.
