---
unique-page-id: 2950555
description: Redigera Facebook Rich Post Settings - Marketo Docs - Produktdokumentation
title: Redigera inställningar för avancerat inlägg på Facebook
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Redigera inställningar för Facebook Rich Post {#edit-facebook-rich-post-settings}

Anpassa inlägg när någon [delar dig](http://docs.marketo.com/display/docs/social) på Facebook.

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

Marketo [sociala appar](http://docs.marketo.com/display/docs/social) tillåter dina leads att dela dina landningssidor med sina anslutningar i sociala nätverk som Facebook, Twitter osv. Med Facebook OpenGraph-taggar (OG-taggar) kan du ange vilken information från din landningssida som ska ingå i Facebook-inlägg.

## Välj alternativ för Rich Post {#select-rich-post-options}

Du kan ange vilka typer av sidinformation som ska användas i de Facebook-inlägg som genereras av delningar från din landningssida.

1. Välj **Facebook-meddelande** i redigeraren för din **YouTube**-video eller sociala knapp.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Välj bland följande alternativ för ditt Facebook-meddelande.

   * Lägg till statiskt innehåll: Välj det här alternativet om du vill ange rubrik, bildtext och beskrivning manuellt.

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Lägg till dynamiskt innehåll: Din sociala app kan använda landningssidans `<TITLE>`-, `<CAPTION>`- och `<DESCRIPTION>`-taggar för att fylla i ditt inlägg.

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >Dessa bör redan finnas i sidans källa, men om du vill ha mer kontroll kan du [lägga till särskilda Facebook OG-taggar på din startsida](edit-facebook-rich-post-settings.md).

   * Lägg inte till avancerat innehåll: Begränsar Facebook-inlägg från din landningssida till endast huvudmeddelandet och länken.

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## Lägg till OG-taggar för Facebook på en landningssida {#add-facebook-og-tags-to-a-landing-page}

Om du vill styra vilka sidelement som ska inkluderas i Facebook-delningarna från din landningssida kan du lägga till Facebooks OG-taggar (Open Graph) för titel, bildtext och beskrivning på din landningssida.

1. Öppna landningssidan som innehåller din **YouTube-video** eller sociala knapp.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **Startsidans Designer** öppnas i ett nytt fönster.

1. Välj **Åtgärder för landningssida** > **Redigera sidmetataggar****.**

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Lägg till HTML-koden som definierar log:title, og:caption och og:description. Kopiera och klistra in dessa rader och ersätt platshållartexten:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Var noga med att använda rätt HTML-syntax när du lägger till OG-taggarna.
