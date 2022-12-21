---
unique-page-id: 1147066
description: Åsidosätt personbegränsningar i en smart kampanj - Marketo Docs - produktdokumentation
title: Åsidosätt personbegränsningar i en smart kampanj
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Åsidosätt personbegränsningar i en smart kampanj {#override-person-restrictions-in-a-smart-campaign}

Med Marketo kan ni ange det högsta antalet personer som kan kvalificera sig för en smart kampanj. På så sätt slipper du oavsiktligt skicka hela databasen via e-post. Om du vill _åsidosätta_ den här gränsen, så här.

>[!PREREQUISITES]
>
>Se till att [aktivera personbegränsningar för smarta kampanjer](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) i Marketo Admin.

1. Gå till er smarta kampanj i marknadsföringsaktiviteter och klicka på **Schema**.

   ![](assets/one.png)

1. Klicka på Inställningar för smart kampanj **Redigera**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Standardgränsen är den som anges i Admin.

1. Ange en ny gräns och klicka sedan på **Spara.**

   ![](assets/three.png)

   Den smarta kampanjen körs inte om antalet personer som är kvalificerade överstiger den angivna gränsen.

   >[!CAUTION]
   >
   >Var försiktig med den här funktionen så att du inte oavsiktligt tar med för många personer.
