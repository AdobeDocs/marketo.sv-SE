---
description: GenAI Features - Marketo Docs - produktdokumentation
title: GenAI-funktioner
feature: Interactive Webinars
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: ce79145d8186e6d17dbe579aceb90d3c209f1b31
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# GenAI-funktioner {#gen-ai-features}

Generera kapitel och sammanfattningar automatiskt för dina inspelade webbinarier, så att de blir mer tillgängliga och lättare att navigera i.

* **Automatisk kapitelgenerering**: AI-baserad teknik skapar kapitel för ditt webbinariinnehåll.

* **AI-genererad sammanfattning**: Få en automatisk textsammanfattning av ditt webbinarium.

* **Redigerbart innehåll**: Ändra genererade kapitel och sammanfattningar om det behövs, med hjälp av manuella och AI-baserade redigeringsfunktioner.

* **Enkel integrering**: Lägg enkelt till kapitel och sammanfattningar på dina landningssidor genom att kopiera HTML-koden till valfri webbsideredigerare.

## Aktivera GenAI {#enable-genai}

>[!PREREQUISITES]
>
>Innan du använder dessa funktioner måste du godkänna Adobe GenAI-villkoren. Om du ännu inte gjort det kan du kontakta Adobe Account Team (din kontoansvarige) för mer information.

När du har godkänt villkoren i Adobe GenAI är nästa steg att aktivera det för enskilda användare. Gör det genom att gå till **[!UICONTROL Admin]** > **[!UICONTROL Interactive Webinars]** och välja vilka användare som ska ha tillgång till GenAI.

![](assets/gen-ai-features-1.png){width="800" zoomable="yes"}

## Åtkomst {#how-to-access}

1. Gå till webbseminariets översiktssida i Marketo Engage Interactive Webinars.

1. När du har utfört ett on-demand-webbinarium väntar du 30 till 60 minuter tills AI bearbetar inspelningen. Knappen Generera blir klickbar när den är tillgänglig.

1. Klicka på **[!UICONTROL View GenAI Content]**.

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. En ny flik öppnas med AI-genererade kapitel och en textsammanfattning.

## Redigera genererat innehåll {#edit-generated-content}

1. Granska de genererade kapitlen och sammanfattningen.

1. Klicka på knappen **[!UICONTROL Edit]** om det behövs några ändringar.

   Gör ändringar:

   * Redigera text i sammanfattningen och/eller kapitelrubrikerna.

   * Om det behövs kan du justera tidsstämplar genom att redigera värdena i tidsstämpelfält.

   * Ta bort oönskade kapitel genom att markera dem och klicka på **[!UICONTROL Delete]**.

   * Sammanfoga två sammanhängande kapitel genom att markera dem och klicka på **[!UICONTROL Merge]**.

      * AI genererar ett sammansatt kapitel som består av de två valda kapitlen

      * Om du vill sammanfoga flera kapitel måste du göra två åt gången

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* Om du vill kan du klassificera kvaliteten på de genererade kapitlen/sammanfattningen med ikonerna _tummen uppåt_ ![Tummen uppåt ](assets/icon-thumbs-up.png) eller _tummen nedåt_ ![Tummen nedåt ](assets/icon-thumbs-down.png) . Du kan också flagga problematiskt innehåll genom att klicka på flaggikonen ![Flaggikon](assets/icon-flag.png) .
   >
   >* Om du inte är nöjd med den inledande sammanfattningen kan du klicka på knappen **[!UICONTROL Regenerate summary]** så skapas en annan version.

1. Spara ändringarna genom att klicka på knappen **[!UICONTROL Save]** i skärmens övre högra hörn.

## Använd genererat innehåll {#use-generated-content}

När du har kopierat det innehåll du vill använda, klistrar du in det i valfri redigerare (t.ex. Marketo Engage Landing Page editor) och gör eventuella justeringar.

### Sammanfattning {#summary}

**Kopiera HTML** - Klicka på knappen **[!UICONTROL Copy HTML]** om du vill hämta all text, med HTML-kodformatering inuti en tabell.

**Endast text** - Om du bara vill ha texten markerar du den och väljer Ctrl/Cmd+C (eller högerklickar) för att kopiera den.

### Kapitel {#chapters}

**Kopiera HTML** - Klicka på knappen **[!UICONTROL Copy HTML]** för att få alla inspelningar och dess kapitel formaterade inuti en videospelare.

## Rikta er till er målgrupp

Utnyttja Smart Campaign/List-filter och/eller triggers för att se vad varje tittare tittade på, hur många gånger, osv., vilket möjliggör personaliserade uppföljningar.

![](assets/gen-ai-features-4.png){width="800" zoomable="yes"}

* **Utlösare**: _Klicka på Länk på webbsida_, _Besök webbsida_

* **Filter**: _Klicka på Länk på webbsida_, _Besökt webbsida_

&quot;link&quot; är namnet på kapitlet och &quot;web page&quot; är den sida som är värd för ditt On Demand-webbinarium.

>[!TIP]
>
>Använd [begränsningar](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} om du vill förfina målgruppen ytterligare.

## Saker att notera {#things-to-note}

* Om du tar bort eller sammanfogar kapitel påverkas bara kapitelstacken, inte själva videoinnehållet. Dessa åtgärder är permanenta.

* GenAI-funktionerna är flexibla och kan användas med olika webbsideredigerare, inte bara de i Marketo Engage.

* Förhandsgranska alltid ändringarna för att säkerställa önskad funktionalitet och utseende.

* När du tar bort webbinariet tas även GenAI-innehållet bort.

* Om du vill ta bort GenAI-innehållet utan att ta bort webbinariet kontaktar du Adobe Account Team (din kontohanterare) eller skickar en begäran om att ta bort data till: `marketo-webinar-genai-alerts@adobe.com`.
