---
unique-page-id: 2359793
description: Använd e-post i sociala kampanjer - Marketo Docs - Produktdokumentation
title: Använd e-post i sociala kampanjer
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Använd e-post i sociala kampanjer {#use-emails-in-social-promotions}

När du skapar ett [hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) eller en [utlottning](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md) kan du inkludera e-postmeddelanden som skickas när personen registrerar sig och igen när personen har vunnit belöningen.

>[!TIP]
>
>Mer information om hur du skapar e-postmeddelanden finns i [Skicka en e-poststund](/help/marketo/getting-started/quick-wins/send-an-email.md).

Använd följande variabler i e-postmeddelanden:

* **E-post** för registrering: Används  **`{{social.Share Url}}`** för att skicka en personlig delningslänk till varje deltagare.

* **Fulfillment email**: Skicka  **`{{social.Promo Code}}`** en  [kampanjkod](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) till varje vinnare.

>[!PREREQUISITES]
>
>Innan du kan lägga till ett e-postmeddelande i en social app måste det vara _användbart_ och _godkänt_. Se [Redigera inställningar för ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Markera programmet och klicka på **Redigera utkast**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Gå till **Appinställningar > Erbjudandeinformation** (eller **Information om Lotteriet**) i redigeraren för sociala appar.

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Lägg till e-postmeddelandet om registrering.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >Bekräftelsemeddelandet skickas automatiskt när en person registrerar sig.

1. Lägg till e-postmeddelandet.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. I ett hänvisningserbjudande väljer du om mejlet ska skickas automatiskt eller manuellt.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>I utlottningar skickas e-postmeddelandet alltid automatiskt när du [väljer vinnaren](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definition**
>
>* **automatiskt på mål**: E-postmeddelandet skickas automatiskt när varje deltagare uppfyller målet.
>* **skicka** manuellt: När man börjat uppnå målet återgår man till hänvisningserbjudandet för att manuellt  [skicka e-postmeddelandet](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).

>



>[!MORELIKETHIS]
>
>Därefter kan du [välja resurs-URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) eller, i ditt hänvisningserbjudande, [ladda upp de kampanjkoder](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) som du skickar ut.
