---
unique-page-id: 2950555
description: Redigera Facebook Rich Post Settings - Marketo Docs - produktdokumentation
title: Redigera inställningar för avancerat inlägg på Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Redigera inställningar för [!DNL Facebook] Rich Post {#edit-facebook-rich-post-settings}

Anpassa inlägg när andra delar dig på [!DNL Facebook].

>[!AVAILABILITY]
>
>Alla Marketo Engage-användare har inte köpt den här funktionen. Kontakta Adobe Account Team (din kontoansvarige) för mer information.

Marketo _sociala appar_ tillåter dina leads att dela dina landningssidor med sina anslutningar i sociala nätverk som Facebook, Twitter osv. Med Facebook OpenGraph-taggar (OG-taggar) kan du ange vilken information från din landningssida som ska ingå i Facebook-inlägg.

## Välj alternativ för Rich Post {#select-rich-post-options}

Du kan ange vilka typer av sidinformation som ska användas i de [!DNL Facebook] avancerade inlägg som genereras av delningar från din landningssida.

1. Välj **[!UICONTROL Facebook Message]** i redigeraren för din _[!DNL YouTube_]_-video eller sociala knapp.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Välj bland följande alternativ för ditt [!DNL Facebook]-meddelande.

   * Lägg till statiskt innehåll: Välj det här alternativet om du vill ange rubrik, bildtext och beskrivning manuellt.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Lägg till dynamiskt innehåll: Din sociala app kan använda din startsidas `<TITLE>` -, `<CAPTION>` - och `<DESCRIPTION>` -taggar för att fylla i ditt inlägg.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Dessa bör redan finnas i sidkällan, men om du vill ha mer kontroll kan du lägga till specifika [!DNL Facebook] OG-taggar på landningssidan.

   * Lägg inte till omfattande innehåll: Begränsar [!DNL Facebook] inlägg från din landningssida till enbart huvudmeddelandet och länken.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Lägg till [!DNL Facebook] OG-taggar på en landningssida {#add-facebook-og-tags-to-a-landing-page}

Om du vill styra de sidelement som ska inkluderas i [!DNL Facebook]-delningarna från din landningssida kan du lägga till [!DNL Facebook] OG-taggar (Open Graph) för titel, bildtext och beskrivning på din landningssida.

1. Öppna landningssidan som innehåller din **[!DNL YouTube]video** eller sociala knapp.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **[!UICONTROL Landing Page Designer]** öppnas i ett nytt fönster.

1. Välj **[!UICONTROL Landing Page Actions]** > **[!UICONTROL Edit Page Meta Tags]**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Lägg till den HTML som definierar log:title, og:caption och og:description. Kopiera och klistra in dessa rader och ersätt platshållartexten:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Var noga med att använda rätt HTML-syntax när du lägger till OG-taggarna.
