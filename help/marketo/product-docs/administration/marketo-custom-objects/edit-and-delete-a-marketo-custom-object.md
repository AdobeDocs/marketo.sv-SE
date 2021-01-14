---
unique-page-id: 10093690
description: Redigera och ta bort ett Marketo-anpassat objekt - Marketo-dokument - Produktdokumentation
title: Redigera och ta bort ett markeringsobjekt till anpassat objekt
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Redigera och ta bort ett markerings-till-anpassat objekt {#edit-and-delete-a-marketo-custom-object}

>[!NOTE]
>
>Du kan inte skapa, redigera eller ta bort ett länk- eller borttagningsfält när det anpassade objektet har godkänts.

## Redigera ett anpassat objekt {#edit-a-custom-object}

Använd menyn Anpassade objektåtgärder för att redigera eller ta bort ett anpassat objekt.

1. Klicka på **Admin** och välj **Marketo-anpassade objekt** i **Databashantering**.

   ![](assets/image2016-1-18-13-3a31-3a51.png)

1. Markera det anpassade objekt som du vill redigera till höger.

   ![](assets/image2016-1-18-13-3a33-3a11.png)

1. Klicka på fliken **Anpassade objektåtgärder** och klicka på **Redigera objekt**.

   ![](assets/image2015-9-23-11-3a37-3a44.png)

   >[!NOTE]
   >
   >Redigera objekt visar samma fält som Skapa objekt, förutom API-namnet som inte kan redigeras.

1. Gör ändringar. Dra skjutreglaget över om du vill visa objektet på sidan Leaddetaljer. Klicka på **Spara**.

   ![](assets/image2015-9-15-16-3a48-3a39.png)

1. Var noga med att godkänna [det redigerade objektet](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md).

## Ta bort ett anpassat objekt {#delete-a-custom-object}

Det är enkelt att ta bort ett anpassat objekt, men du måste vara försiktig. Anpassade objekt kan anslutas till andra objekt eller till smarta listor. Marketo varnar dig därför innan du kan klicka på **Ta bort**.

>[!CAUTION]
>
>Du kan inte återställa ett anpassat objekt när du har tagit bort det.

1. Klicka på **Admin** och välj **Marketo-anpassade objekt** i **Databashantering**.

   ![](assets/image2016-1-18-13-3a36-3a0.png)

1. Markera det objekt som du vill ta bort.

   ![](assets/image2015-9-23-16-3a29-3a5.png)

1. Klicka på **Anpassade objektåtgärder** och välj **Ta bort objekt**.

   ![](assets/image2015-9-23-11-3a39-3a5.png)

   >[!TIP]
   >
   >Du kan också högerklicka på objektet och välja **Ta bort objekt**.

1. Om det anpassade objektet är i utkastform, inte godkänt än, får du den här varningen. Om du är säker klickar du på **Ta bort**.

   ![](assets/image2015-9-23-16-3a31-3a2.png)

1. Om det anpassade objektet redan har godkänts finns det en större risk om du tar bort det. Så du får en bättre varning. Ange **Jag förstår**, markera kryssrutan **Det går inte att ångra** och klicka på **Ta bort**.

   ![](assets/image2016-1-15-9-3a49-3a38.png)

   >[!NOTE]
   >
   >Om det anpassade objektet är länkat till ett mellanliggande objekt måste du först ta bort mellanliggande objekt.

>[!MORELIKETHIS]
>
>[Godkänn ett anpassat objekt](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
