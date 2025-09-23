---
unique-page-id: 1900573
description: Lägg till en systemtoken som en länk i ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Lägg till en systemtoken som en länk i ett e-postmeddelande
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '205'
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

1. Sök efter och välj din e-postadress och klicka sedan på **[!UICONTROL Edit Draft]**.

   ![](assets/one-1.png)

1. Dubbelklicka i ett redigerbart område.

   ![](assets/two-1.png)

1. Markera den text som du vill konvertera till en länk som har token och klicka på knappen **[!UICONTROL Insert/Edit Link]**.

   ![](assets/three-1.png)

1. Ange token i länk-URL och klicka på **[!UICONTROL Insert]**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Kopiera/klistra in den token du vill använda: **`{{system.forwardToFriendLink}}`**, **`{{system.unsubscribeLink}}`** eller **`{{system.viewAsWebpageLink}}`**

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Om du använder den här metoden för att lägga till systemtoken &quot;viewAsWebpageLink&quot; kan du **inte** åsidosätta den med token. Använd i stället [Lägg till en vy som webbsideslänk i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) som gör att du kan åsidosätta viewAsWebPageLink med hjälp av token.

>[!NOTE]
>
>Glöm inte att [godkänna e-postmeddelandet](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) när du är klar.

Snyggt gjort! Nu vet du hur du lägger till en systemtoken som en länk i ett e-postmeddelande.
