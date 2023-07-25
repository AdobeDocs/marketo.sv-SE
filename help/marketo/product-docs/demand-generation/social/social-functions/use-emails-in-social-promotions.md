---
unique-page-id: 2359793
description: Använd e-post i sociala kampanjer - Marketo Docs - produktdokumentation
title: Använd e-post i sociala kampanjer
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Använd e-post i sociala kampanjer {#use-emails-in-social-promotions}

När du skapar en [hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) eller en [utlottningar](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)kan du inkludera e-postmeddelanden som skickas när personen registrerar sig och igen när personen har vunnit belöningen.

>[!TIP]
>
>Information om hur du skapar e-postmeddelanden finns i [Skicka ett e-postutdrag](/help/marketo/getting-started/quick-wins/send-an-email.md).

Använd följande variabler i e-postmeddelanden:

* **E-post för registrering**: Använd **`{{social.Share Url}}`** för att skicka en personlig delningslänk till varje deltagare.

* **Fulfillment email**: Använd **`{{social.Promo Code}}`** för att skicka varje vinnare [kampanjkod](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Innan du kan lägga till ett e-postmeddelande i en social app måste det _operativ_ och _godkänd_. Se [Redigera inställningar för ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Välj programmet och klicka på **Redigera utkast**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. I redigeraren för sociala appar går du till **Appinställningar > Erbjudandeinformation** (eller **Information om Lotteriet**).

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
>I utlottningar skickas e-postmeddelandet alltid automatiskt när du [välj vinnaren](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definition**
>
>* **automatiskt på mål**: E-postmeddelandet skickas automatiskt när varje deltagare uppfyller målet.
>* **skicka manuellt**: När man väl börjat uppnå målet kan man gå tillbaka till hänvisningserbjudandet för att manuellt [skicka e-postmeddelandet](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>Nu kan du [välj delnings-URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) eller, i ditt hänvisningserbjudande, kan du [ladda upp kampanjkoder](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) du skickar ut.
