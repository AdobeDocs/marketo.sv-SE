---
unique-page-id: 1900573
description: Lägg till en systemtoken som en länk i ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Lägg till en systemtoken som en länk i ett e-postmeddelande
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
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
>Dessa variabler kommer att **not** klickbara om de inte finns inuti en ankarlänk. Dessutom kan de **not** vara inbäddad i en My Token.

Så här lägger du till dem i ett e-postmeddelande:

1. Sök och välj e-postadress och klicka sedan på **Redigera utkast**.

   ![](assets/one-1.png)

1. Dubbelklicka i ett redigerbart område.

   ![](assets/two-1.png)

1. Markera den text som du vill konvertera till en länk med variabeln och klicka på knappen **Infoga/redigera länk** -knappen.

   ![](assets/three-1.png)

1. Ange token i länkens URL och klicka på **Infoga**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Kopiera/klistra in den token du vill använda: **`{{system.forwardToFriendLink}}`** eller **`{{system.unsubscribeLink}}`** eller **`{{system.viewAsWebpageLink}}`**

1. Klicka **Spara**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Om du använder den här metoden för att lägga till systemtoken &quot;viewAsWebpageLink&quot; kan du **not** åsidosätt den med hjälp av variabler. Använd i stället [Lägg till en länk för Visa som webbsida i ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) som gör att du kan åsidosätta viewAsWebPageLink med hjälp av variabler.

>[!NOTE]
>
>Glöm inte att [godkänna din e-post](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) när det är klart.

Snyggt gjort! Nu vet du hur du lägger till en systemtoken som en länk i ett e-postmeddelande.
