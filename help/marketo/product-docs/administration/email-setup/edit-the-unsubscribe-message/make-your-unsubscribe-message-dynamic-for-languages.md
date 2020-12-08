---
unique-page-id: 6848782
description: Gör ditt avbeställningsmeddelande dynamiskt för språk - Marketo Docs - Produktdokumentation
title: Gör ditt avbeställningsmeddelande dynamiskt för språk
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# Gör ditt avbeställningsmeddelande dynamiskt för språk {#make-your-unsubscribe-message-dynamic-for-languages}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Standardmeddelandet och länken för att avbryta prenumerationen är på engelska. Du kan använda dynamiskt innehåll för att visa det på olika språk.

>[!NOTE]
>
>Vi har skapat den här lilla lektionen nedan åt dig. Det är en bra metod, men det kan man göra på andra sätt.

1. Förbered dina data
1. [Skapa ett anpassat](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)fält med namnet&quot;Önskat språk&quot;. (Konfigurera den i CRM om du vill att det här fältet ska synkroniseras).

   >[!TIP]
   >
   >I framtiden ska du använda det här fältet när du [skapar ett formulär](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) för att hämta språkinställningar.

1. Skapa segmentering
1. Gå till **databasen**.
** ![](assets/db.png)

   **

1. Klicka på **Nytt segment i listrutan** Nytt ****.

   ![](assets/two.png)

1. Namnge segmenteringen **Standardspråk**. Klicka på **Lägg till segment**. Skriv på ett språk.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Standardsegmentet är engelska.

1. Fortsätt att lägga till segment tills alla språk är representerade. Klicka på **Skapa**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Markera ett segment.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Gå till fliken **Smart lista** . Ange **Önskat språk** i sökfältet. Dra och släpp filtret på arbetsytan.

   ![](assets/six.png)

1. Ange lämpligt motsvarande språk.

   ![](assets/seven.png)

1. Upprepa för alla dina olika språk. Välj sedan listrutan **Segmenteringsåtgärder** och klicka på **Godkänn**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. Skapa ett fragment
1. Gå till **Design Studio**.

   ![](assets/ds.png)

1. I listrutan **Nytt** klickar du på **Nytt fragment**.

   ** ![](assets/ten.png)

   **

1. Ge fragmentet namnet **Unsubscribe Message**. Klicka på **Skapa**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Skriv ditt standardmeddelande för att avbryta prenumerationen, markera det och klicka på hyperlänksikonen.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Kopiera och klistra in denna token: **`{{system.unsubscribeLink}}`** till fältet **Länk-URL** . Klicka på **Infoga**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Markera **Segmentera efter** i segmenteringsavsnittet.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. I listrutan Segmentering skriver du **Preferred** och väljer **Preferred Language**. Klicka på **Spara**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Markera ett segment i trädet. Skriv ditt avbeställningsmeddelande på det språket.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Kopiera och klistra in samma token: **`{{system.unsubscribeLink}}`** till fältet **Länk-URL** . Klicka på **Infoga**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Upprepa för alla segment. Gå sedan tillbaka till Design Studio, klicka på listrutan **Fragmentåtgärder** och klicka på **Godkänn**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Häftig. Nästan klart.

1. Använd kodfragment i ett e-postmeddelande
1. Klicka på det redigerbara elementet i e-postredigeraren. Klicka sedan på kugghjulsikonen och välj **Ersätt med kodutdrag**. Om du markerar ett redigerbart fragmentelement klickar du på kugghjulsikonen och väljer **Redigera**.

   ![](assets/4.1.png)

1. Leta upp och markera fragmentet i listrutan och klicka på **Spara**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Klicka på **Bakåt** om du vill testa den..

   ![](assets/4.3.png)

1. ...sedan fliken **Dynamisk** .

   ![](assets/4.4.png)

1. Klicka på de olika språken för att se ändringen av fragmentet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Naturligtvis kan du även redigera resten av e-postmeddelandet för dynamiskt språk. När du är klar gör du samma sak på sidan för att avbryta prenumerationen.

1. Anpassa din sida för avanmälan med dynamiskt innehåll

   Om du vill att dina medarbetare ska komma till en avanmälningssida på det språk de föredrar, kan du använda dynamiskt innehåll på landningssidan och bekräftelsesidan.

   Gå till Design Studio.

   ![](assets/ds.png)

   Skriv in Avbeställ i sökfältet. Du hittar sidorna för Avbeställ.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   Klicka på Redigera utkast.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   Välj Segment efter.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   Hitta segmentet Önskat språk. Klicka på Spara.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Redigera innehållet för varje landningssida, godkänn och var redo!

   >[!NOTE]
   >
   >**Djupdykning**
   >
   >
   >Läs mer om [dynamiskt innehåll](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) och allt annat du kan göra.

