---
unique-page-id: 10093690
description: Redigera och ta bort ett anpassat Marketo-objekt - Marketo Docs - produktdokumentation
title: Redigera och ta bort ett anpassat Marketo-objekt
exl-id: 97bae63e-f679-490b-bfa2-51d88355b29c
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 1%

---

# Redigera och ta bort ett anpassat Marketo-objekt {#edit-and-delete-a-marketo-custom-object}

>[!NOTE]
>
>Du kan inte skapa, redigera eller ta bort ett länk- eller borttagningsfält när det anpassade objektet har godkänts.

## Redigera ett anpassat objekt {#edit-a-custom-object}

Använd menyn Anpassade objektåtgärder för att redigera eller ta bort ett anpassat objekt.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-1.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-2.png)

1. Markera det anpassade objekt som du vill redigera till höger.

   ![](assets/edit-and-delete-a-marketo-custom-object-3.png)

1. Klicka på fliken **[!UICONTROL Custom Object Actions]** och klicka på **[!UICONTROL Edit Object]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-4.png)

1. Gör önskade ändringar. Dra skjutreglaget över om du vill visa objektet på sidan Leaddetaljer. Klicka på **[!UICONTROL Save]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-5.png)

1. Var noga med att godkänna [det redigerade objektet](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md).

## Ta bort ett anpassat objekt {#delete-a-custom-object}

Det är enkelt att ta bort ett anpassat objekt, men du måste vara försiktig. Anpassade objekt kan anslutas till andra objekt eller till smarta listor. Marketo varnar dig innan du kan klicka på **[!UICONTROL Delete]**.

>[!CAUTION]
>
>Du kan inte återställa ett anpassat objekt när du har tagit bort det.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-6.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-7.png)

1. Markera det objekt som du vill ta bort.

   ![](assets/edit-and-delete-a-marketo-custom-object-8.png)

1. Klicka på **[!UICONTROL Custom Object Actions]** och välj **[!UICONTROL Delete Object]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-9.png)

   >[!TIP]
   >
   >Du kan också högerklicka på objektet och välja **[!UICONTROL Delete Object]**.

1. Om det anpassade objektet är i utkastform, inte godkänt än, får du den här varningen. Klicka på **[!UICONTROL Delete]** om du är säker.

   ![](assets/edit-and-delete-a-marketo-custom-object-10.png)

1. Om det anpassade objektet redan har godkänts finns det en större risk om du tar bort det. Så du får en bättre varning. Ange **[!UICONTROL I understand]**, markera kryssrutan **[!UICONTROL Cannot Undo]** och klicka på **[!UICONTROL Delete]**.

   ![](assets/edit-and-delete-a-marketo-custom-object-11.png)

   >[!NOTE]
   >
   >Om det anpassade objektet är länkat till ett mellanliggande objekt måste du först ta bort mellanliggande objekt.

>[!MORELIKETHIS]
>
>[Godkänn ett anpassat objekt](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
