---
unique-page-id: 1900573
description: Lägg till en systemtoken som en länk i ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Lägg till en systemtoken som en länk i ett e-postmeddelande
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---


# Lägg till en systemtoken som en länk i ett e-postmeddelande {#add-a-system-token-as-a-link-in-an-email}

Du kan använda dessa systemtokens för att anpassa positionen för särskilda länkar i dina e-postmeddelanden.

Följande variabler kan användas som länkar i en e-postmall eller e-postmall:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Dessa tokens **kan inte** klickas om de inte finns i en ankarlänk. Dessutom kan de **inte** bäddas in i en Min token.

Så här lägger du till dem i ett e-postmeddelande:

1. Sök efter och markera e-postmeddelandet och klicka sedan på **Redigera utkast**.

   ![](assets/one-1.png)

1. Dubbelklicka i ett redigerbart område.

   ![](assets/two-1.png)

1. Markera den text som du vill konvertera till en länk som ska ha variabeln och klicka på knappen **Infoga/redigera länk**.

   ![](assets/three-1.png)

1. Ange token i länk-URL och klicka på **Infoga**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Kopiera/klistra in den token du vill använda: **`{{system.forwardToFriendLink}}`** eller **`{{system.unsubscribeLink}}`** eller **`{{system.viewAsWebpageLink}}`**

1. Klicka på **Spara**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!NOTE]
>
>Glöm inte att [godkänna e-postmeddelandet](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) när du är klar.

Snyggt gjort! Nu vet du hur du lägger till en systemtoken som en länk i ett e-postmeddelande.
