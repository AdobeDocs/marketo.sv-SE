---
unique-page-id: 6848782
description: Gör ditt avbeställningsmeddelande dynamiskt för språk - Marketo Docs - Produktdokumentation
title: Gör ditt avbeställningsmeddelande dynamiskt för språk
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# Gör ditt meddelande om att avbryta prenumerationen dynamiskt för språk {#make-your-unsubscribe-message-dynamic-for-languages}

Standardmeddelandet och länken för att avbryta prenumerationen är på engelska. Du kan använda dynamiskt innehåll för att visa det på olika språk.

>[!NOTE]
>
>Vi har skapat den här lilla lektionen nedan åt dig. Det är en bra metod, men det kan man göra på andra sätt.

## Förbered dina data {#prepare-your-data}

1. [Skapa ett anpassat ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) fält med namnet&quot;Önskat språk&quot;. (Konfigurera den i CRM om du vill att det här fältet ska synkroniseras).

   >[!TIP]
   >
   >I framtiden ska du använda det här fältet när du [skapar ett formulär](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) för att hämta språkinställningar.

## Skapa segmentering {#create-segmentation}

1. Gå till **databasen**.

   ![](assets/db.png)

1. I listrutan **Nytt** klickar du på **Nytt segment**.

   ![](assets/two.png)

1. Namnge segmenteringen **Önskat språk**. Klicka på **Lägg till segment**. Skriv på ett språk.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Standardsegmentet är engelska.

1. Fortsätt att lägga till segment tills alla språk är representerade. Klicka på **Skapa**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Markera ett segment.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Gå till fliken **Smart lista**. Ange **Önskat språk** i sökfältet. Dra och släpp filtret på arbetsytan.

   ![](assets/six.png)

1. Ange lämpligt motsvarande språk.

   ![](assets/seven.png)

1. Upprepa för alla dina olika språk. Välj sedan listrutan **Segmenteringsåtgärder** och klicka på **Godkänn**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## Skapa ett fragment {#create-a-snippet}

1. Gå till **Design Studio**.

   ![](assets/ds.png)

1. I listrutan **Nytt** klickar du på **Nytt fragment**.

   ![](assets/ten.png)

1. Namnge fragmentet **Avsluta prenumeration på meddelande**. Klicka på **Skapa**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Skriv ditt standardmeddelande för att avbryta prenumerationen, markera det och klicka på hyperlänksikonen.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Kopiera och klistra in denna token: `{{system.unsubscribeLink}}` i fältet **Länk-URL**. Klicka på **Infoga**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Välj **Segmentera med** i segmenteringsavsnittet.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. I listrutan Segmentering skriver du **Preferred** och väljer **Preferred Language**. Klicka på **Spara**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Markera ett segment i trädet. Skriv ditt avbeställningsmeddelande på det språket.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Kopiera och klistra in samma token: `{{system.unsubscribeLink}}` i fältet **Länk-URL**. Klicka på **Infoga**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Upprepa för alla segment. Gå sedan tillbaka till Design Studio, klicka på listrutan **Fragmentåtgärder** och klicka på **Godkänn**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Häftig. Nästan klart.

## Använd kodfragment i ett e-postmeddelande {#use-snippet-in-an-email}

1. Klicka på det redigerbara elementet i e-postredigeraren. Klicka sedan på kugghjulsikonen och välj **Ersätt med fragment**. Om du markerar ett redigerbart fragmentelement klickar du på kugghjulsikonen och väljer **Redigera**.

   ![](assets/4.1.png)

1. Sök efter och välj kodfragment i listrutan och klicka på **Spara**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Om du vill testa den klickar du på **Bakåt**..

   ![](assets/4.3.png)

1. ...sedan fliken **Dynamisk**.

   ![](assets/4.4.png)

1. Klicka på de olika språken för att se ändringen av fragmentet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Naturligtvis kan du även redigera resten av e-postmeddelandet för dynamiskt språk. När du är klar gör du samma sak på sidan för att avbryta prenumerationen.

## Anpassa din sida för avanmälan med dynamiskt innehåll {#customizing-your-unsubscribe-page-with-dynamic-content}

Om du vill att dina medarbetare ska komma till en avanmälningssida på det språk de föredrar, kan du använda dynamiskt innehåll på landningssidan och bekräftelsesidan.

1. Gå till Design Studio.

   ![](assets/ds.png)

1. Skriv in _Unsubscribe_ i sökfältet. Du hittar sidorna för Avbeställ.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. Klicka på **Redigera utkast**.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. Välj **Segmentera med**.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. Hitta segmentet Önskat språk. Klicka på **Spara**.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Redigera innehållet för varje landningssida, godkänn och var redo!

   >[!NOTE]
   >
   >Läs mer om [dynamiskt innehåll](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) och alla coola saker du kan göra.
