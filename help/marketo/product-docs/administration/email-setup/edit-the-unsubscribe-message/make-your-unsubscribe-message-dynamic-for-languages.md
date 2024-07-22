---
unique-page-id: 6848782
description: Gör ditt avbeställningsmeddelande dynamiskt för språk - Marketo Docs - produktdokumentation
title: Gör ditt avbeställningsmeddelande dynamiskt för språk
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 1%

---

# Gör ditt avbeställningsmeddelande dynamiskt för språk {#make-your-unsubscribe-message-dynamic-for-languages}

Standardmeddelandet och länken för att avbryta prenumerationen är på engelska. Du kan använda dynamiskt innehåll för att visa det på olika språk.

>[!NOTE]
>
>Den här artikeln är en bra metod, men kan användas på andra sätt.

## Förbered dina data {#prepare-your-data}

1. [Skapa ett anpassat fält](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) med namnet&quot;Önskat språk&quot;. (Konfigurera den i CRM om du vill att det här fältet ska synkroniseras).

   >[!TIP]
   >
   >I framtiden ska du använda det här fältet när du [skapar ett formulär](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) för att hämta språkinställningar.

## Skapa segmentering {#create-segmentation}

1. Gå till **[!UICONTROL Database]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. Klicka på **[!UICONTROL New Segmentation]** i listrutan **[!UICONTROL New]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Namnge segmenteringen **[!UICONTROL Preferred Language]**. Klicka på **[!UICONTROL Add Segment]**. Skriv på ett språk.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Standardsegmentet är engelska.

1. Fortsätt att lägga till segment tills alla dina språk finns representerade. Klicka på **[!UICONTROL Create]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Markera ett segment.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Gå till fliken **[!UICONTROL Smart List]**. Ange **[!UICONTROL Preferred Language]** i sökfältet. Dra filtret till arbetsytan.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Ange lämpligt motsvarande språk.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Upprepa för alla dina olika språk. Markera sedan listrutan **[!UICONTROL Segmentation Actions]** och klicka på **[!UICONTROL Approve]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Skapa ett fragment {#create-a-snippet}

1. Gå till **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. Klicka på **[!UICONTROL New Snippet]** i listrutan **[!UICONTROL New]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Namnge fragmentet **Avbeställ meddelande**. Klicka på **[!UICONTROL Create]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Skriv ditt standardmeddelande för att avbryta prenumerationen, markera det och klicka på hyperlänksikonen.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Kopiera och klistra in denna token: `{{system.unsubscribeLink}}` i fältet **[!UICONTROL URL]**. Klicka på **[!UICONTROL Insert]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Välj **[!UICONTROL Segment By]** i avsnittet **[!UICONTROL Segmentation]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. I listrutan **[!UICONTROL Segmentation]** skriver du **[!UICONTROL Preferred]** och väljer **[!UICONTROL Preferred Language]**. Klicka på **[!UICONTROL Save]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Markera ett segment i trädet. Klicka på avbeställningen och klicka sedan på länkikonen.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Kontrollera att `{{system.unsubscribeLink}}` fortfarande finns i fältet **[!UICONTROL URL]**. Redigera **[!UICONTROL Display Text]** så att det matchar det valda språket. Klicka på **[!UICONTROL Apply]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Upprepa för alla segment. Gå sedan tillbaka till **[!UICONTROL Design Studio]**, klicka på listrutan **[!UICONTROL Snippet Actions]** och klicka på **[!UICONTROL Approve]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Häftig. Nästan klart!

## Använd kodfragment i ett e-postmeddelande {#use-snippet-in-an-email}

1. Klicka på det redigerbara elementet i e-postredigeraren. Klicka sedan på kugghjulsikonen och välj **[!UICONTROL Replace with Snippet]**. Om du markerar ett redigerbart fragmentelement klickar du på kugghjulsikonen och väljer **[!UICONTROL Edit]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Sök efter och välj fragmentet i listrutan och klicka på **[!UICONTROL Save]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Om du vill testa det klickar du på **[!UICONTROL Back]**..

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...sedan fliken **[!UICONTROL Dynamic]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Klicka på de olika språken för att se ändringen av fragmentet.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Naturligtvis kan du även redigera resten av e-postmeddelandet för dynamiskt språk. När du är klar gör du samma sak på sidan för att avbryta prenumerationen.

## Anpassa din sida för avanmälan med dynamiskt innehåll {#customizing-your-unsubscribe-page-with-dynamic-content}

Om du vill att dina medarbetare ska komma till en avanmälningssida på det språk de föredrar, kan du använda dynamiskt innehåll på landningssidan och bekräftelsesidan.

1. Navigera till **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Skriv in _Avsluta abonnemang_ i sökfältet och välj den önskade sidan Avsluta abonnemang.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Välj **[!UICONTROL Segment By]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Hitta segmentet **[!UICONTROL Preferred Language]**. Klicka på **[!UICONTROL Save]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Redigera innehållet för varje landningssida, godkänn och var redo!

   >[!NOTE]
   >
   >Läs mer om [dynamiskt innehåll](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) och alla coola saker du kan göra.
