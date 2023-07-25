---
unique-page-id: 7505310
description: Prenumerera på en smart lista - Marketo Docs - produktdokumentation
title: Prenumerera på en smart lista
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Prenumerera på en smart lista {#subscribe-to-a-smart-list}

Att prenumerera på smarta listor är ett bra sätt att hålla reda på personer, med rapporter som skickas direkt till din inkorg.

Du kan skapa en prenumeration på en smart lista på två olika platser:

* Marknadsföringsaktiviteter
* Databas

Prenumerationer använder den fullständiga listan över personer när prenumerationen körs.

Prenumerationer lever där din smarta lista finns, i marknadsföringsaktiviteter eller i databasen.

Du kan skapa flera prenumerationer från samma smarta lista.

Prenumerationer är specifika för arbetsytan. Den här listan över prenumerationer finns till exempel på en annan arbetsyta än de som visas i resten av den här artikeln:

![](assets/one.png)

>[!NOTE]
>
>Du är begränsad till 100 prenumerationer och högst 100 000 personer per prenumeration, över arbetsytor och i Marketo-instanser. Om den smarta listan innehåller fler än 100 000 namn kör Marketo prenumerationen för de första 100 000.

## Skapa en prenumeration på en smart lista {#create-a-smart-list-subscription}

1. Gå till **Databas** eller **Marknadsföringsaktiviteter**.

   ![](assets/db.png)

1. Välj den smarta lista som du vill skapa en prenumeration för. Klicka **Liståtgärder** och markera **Ny prenumeration på Smart List**.

   ![](assets/three.png)

1. Ge din prenumeration en **Namn** väljer eller anger du e-postadresserna till **Mottagare**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Klicka på **Frekvens** och välj en frekvens.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Ange **Slutleverans** datum. Du kan välja **Aldrig** eller ett kalenderdatum.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Klicka **Format** och välj ett alternativ i listan.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Klicka **Skapa**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Din nya smarta listprenumeration visas högst upp i listan på fliken Prenumerationer. Klicka **Skicka** om du vill skicka nu, och inte vänta tills den schemalagda e-postleveransen.

   ![](assets/eight.png)

1. Vi rekommenderar att du avmarkerar kryssrutan Aktiv för att inaktivera en prenumeration på en smart lista om ingen prenumererar på den.

   ![](assets/nine.png)

   Det var lätt, eller hur?

## E-postmeddelande {#email-message}

Mottagarna får ett mejl med möjlighet att ladda ned rapporten samt en länk direkt till listan i Marketo-instansen. Hämtningslänken upphör om fyra dagar.

>[!NOTE]
>
>Om [Säker prenumerationsadministratör](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) inställningen är inställd på **Ja**, kan bara personer med tillgång till Marketo-instansen ladda ned rapporten.

![](assets/image2015-4-17-15-3a46-3a47.png)

Om det finns 0 personer i en rapport får mottagarna fortfarande ett e-postmeddelande. I e-postmeddelandet står det dock bara att det inte finns några personer att rapportera.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>När du ändrar ett smart listfilter som du har baserat en prenumeration på uppdateras även rapporten.

E-postmeddelandet innehåller även ytterligare information om de filter som används för att skapa listan.

## Ta bort en prenumeration {#delete-a-subscription}

Om du vill ta bort en prenumeration markerar du den på prenumerationsfliken och klickar på Ta bort prenumeration.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Redigera en prenumeration på en smart lista](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Skydda inställningen för prenumerationsadministration](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
