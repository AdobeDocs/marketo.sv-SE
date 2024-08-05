---
unique-page-id: 2359793
description: Använd e-post i sociala kampanjer - Marketo Docs - produktdokumentation
title: Använd e-post i sociala kampanjer
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Använd e-post i sociala kampanjer {#use-emails-in-social-promotions}

När du skapar ett [hänvisningserbjudande](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) eller en [utlottning](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md) kan du inkludera e-postmeddelanden som skickas när personen registrerar sig och igen när personen har vunnit belöningen.

>[!IMPORTANT]
>
>Den 31 juli 2024 började vi ta bort den här funktionen. Nya resurser kan inte längre skapas. Befintliga tillgångar kommer att fortsätta att fungera fram till 31 januari 2025. [Läs mer](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!TIP]
>
>Mer information om hur du skapar e-postmeddelanden finns i [Skicka en e-postblast](/help/marketo/getting-started/quick-wins/send-an-email.md).

Använd följande variabler i e-postmeddelanden:

* **E-post för registrering**: Använd **`{{social.Share Url}}`** för att skicka en personlig delningslänk till alla deltagande.

* **Efterlevnad av e-post**: Använd **`{{social.Promo Code}}`** för att skicka en [kampanjkod](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) till varje vinnare.

>[!PREREQUISITES]
>
>Innan du kan lägga till ett e-postmeddelande i en social app måste det vara _operativt_ och _godkänt_. Se [Redigera inställningar för ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Markera appen och klicka på **Redigera utkast**.

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
>* **auto på mål**: E-postmeddelandet skickas automatiskt när varje deltagare uppfyller målet.
>* **skicka** manuellt: När någon har börjat uppnå målet återgår du till ditt hänvisningserbjudande och [skickar e-postmeddelandet](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) manuellt.
>

>[!MORELIKETHIS]
>
>Därefter kan du [välja resurs-URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) eller, i ditt hänvisningserbjudande, [överföra de kampanjkoder](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) som du skickar ut.
