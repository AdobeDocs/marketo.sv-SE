---
unique-page-id: 7505310
description: Prenumerera på en smart lista - Marketo Docs - produktdokumentation
title: Prenumerera på en smart lista
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Prenumerera på en smart lista {#subscribe-to-a-smart-list}

Att prenumerera på smarta listor är ett bra sätt att hålla reda på personer, med rapporter som skickas direkt till din inkorg.

Du kan skapa en prenumeration på en smart lista på två olika platser:

* [!UICONTROL Marketing Activities]
* [!UICONTROL Database]

Prenumerationer använder den fullständiga listan över personer när prenumerationen körs.

Prenumerationer bor där din smarta lista finns, i [!UICONTROL Marketing Activities] eller [!UICONTROL Database].

Du kan skapa flera prenumerationer från samma smarta lista.

Prenumerationer är specifika för arbetsytan. Den här listan över prenumerationer finns till exempel på en annan arbetsyta än de som visas i resten av den här artikeln:

![](assets/one.png)

>[!NOTE]
>
>Du är begränsad till 100 prenumerationer och högst 100 000 personer per prenumeration, över arbetsytor och i Marketo-instanser. Om den smarta listan innehåller fler än 100 000 namn kör Marketo prenumerationen för de första 100 000.

## Skapa en prenumeration på en smart lista {#create-a-smart-list-subscription}

1. Gå till **[!UICONTROL Database]** eller **[!UICONTROL Marketing Activities]**.

   ![](assets/db.png)

1. Välj den smarta lista som du vill skapa en prenumeration för. Klicka på **[!UICONTROL List Actions]** och välj **[!UICONTROL New Smart List Subscription]**.

   ![](assets/three.png)

1. Ge din prenumeration **[!UICONTROL Name]** och välj eller ange e-postadresserna till **[!UICONTROL Recipients]**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Klicka på listan **[!UICONTROL Frequency]** och välj en frekvens.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Ange datumet **[!UICONTROL End Delivery]**. Du kan välja **[!UICONTROL Never]** eller ett kalenderdatum.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Klicka på **[!UICONTROL Format]** och välj i listan.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Din nya smarta listprenumeration visas högst upp i listan på fliken Prenumerationer. Klicka på **[!UICONTROL Send]** om du vill skicka nu och inte vänta tills den schemalagda e-postleveransen.

   ![](assets/eight.png)

1. Vi rekommenderar att du avmarkerar kryssrutan **[!UICONTROL Active]** för att inaktivera en smart listprenumeration om ingen prenumererar på den.

   ![](assets/nine.png)

   Det var lätt, eller hur?

## E-postmeddelande {#email-message}

Mottagarna får ett mejl med möjlighet att ladda ned rapporten samt en länk direkt till listan i Marketo-instansen. Hämtningslänken upphör om fyra dagar.

>[!NOTE]
>
>Om inställningen [Administratör för säker prenumeration](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) är **[!UICONTROL Yes]** kan bara personer med åtkomst till Marketo-instansen hämta rapporten.

![](assets/image2015-4-17-15-3a46-3a47.png)

Om det finns 0 personer i en rapport får mottagarna fortfarande ett e-postmeddelande. I e-postmeddelandet står det dock bara att det inte finns några personer att rapportera.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>När du ändrar ett smart listfilter som du har baserat en prenumeration på uppdateras även rapporten.

E-postmeddelandet innehåller även ytterligare information om de filter som används för att skapa listan.

## Ta bort en prenumeration {#delete-a-subscription}

Om du vill ta bort en prenumeration markerar du den på prenumerationsfliken och klickar på **[!UICONTROL Delete Subscription]**.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Redigera en prenumeration på en smart lista](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Skydda inställningen för prenumerationsadministratör](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
