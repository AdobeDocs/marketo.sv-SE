---
unique-page-id: 2950555
description: Redigera Facebook Rich Post Settings - Marketo Docs - produktdokumentation
title: Redigera inställningar för Facebook Rich Post
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
feature: Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Redigera inställningar för Facebook Rich Post {#edit-facebook-rich-post-settings}

Anpassa inlägg när andra delar dig på Facebook.

>[!AVAILABILITY]
>
>Alla användare i Marketo Engage har inte köpt den här funktionen. Kontakta kontoteamet (din kontoansvarige) för mer information.

Marketo [sociala appar](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) tillåter dina leads att dela dina landningssidor med sina anslutningar i sociala nätverk som Facebook, Twitter osv. Med facebook OpenGraph-taggar (OG-taggar) kan du ange vilken information från landningssidan som ska ingå i Facebook-inlägg.

## Välj alternativ för Rich Post {#select-rich-post-options}

Du kan ange vilka typer av sidinformation som ska användas i Facebook-inlägg som genereras av delningar från din landningssida.

1. Välj **Facebook-meddelande** i redigeraren för **YouTube**-videon eller den sociala knappen.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Välj bland följande alternativ för ditt Facebook-meddelande.

   * Lägg till statiskt innehåll: Välj det här alternativet om du vill ange rubrik, bildtext och beskrivning manuellt.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Lägg till dynamiskt innehåll: Din sociala app kan använda din startsidas `<TITLE>` -, `<CAPTION>` - och `<DESCRIPTION>` -taggar för att fylla i ditt inlägg.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Dessa bör redan finnas i sidkällan, men för större kontroll kan du lägga till särskilda Facebook OG-taggar på landningssidan.

   * Lägg inte till avancerat innehåll: Begränsar Facebook-inlägg från landningssidan till bara huvudmeddelandet och länken.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Lägga till Facebook OG-taggar på en landningssida {#add-facebook-og-tags-to-a-landing-page}

Om du vill styra vilka sidelement som ska inkluderas i Facebook-delningarna från din landningssida kan du lägga till Facebook OG-taggar (Open Graph) för titel, bildtext och beskrivning på din landningssida.

1. Öppna landningssidan som innehåller din **YouTube-video** eller sociala knapp.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **Startsidan för Designer** öppnas i ett nytt fönster.

1. Välj **Åtgärder för landningssida** > **Redigera sidmetataggar**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Lägg till HTML som definierar og:title, og:caption och og:description. Kopiera och klistra in dessa rader och ersätt platshållartexten:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Var noga med att använda rätt HTML-syntax när du lägger till OG-taggarna.
