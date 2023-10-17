---
unique-page-id: 1147066
description: Åsidosätt personbegränsningar i en smart kampanj - Marketo Docs - produktdokumentation
title: Åsidosätt personbegränsningar i en smart kampanj
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Åsidosätt personbegränsningar i en smart kampanj {#override-person-restrictions-in-a-smart-campaign}

Med Marketo Engage kan ni ange det maximala antalet personer som kan kvalificera sig för en smart kampanj, vilket hjälper er att undvika att skicka hela databasen med e-post av misstag. Om du vill _åsidosätta_ den här gränsen, så här.

>[!PREREQUISITES]
>
>Se till att [aktivera personbegränsningar för smarta kampanjer](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} i Marketo Admin.

1. Gå till er smarta kampanj i marknadsföringsaktiviteter och klicka på **Schema**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicka på Inställningar för smart kampanj **[!UICONTROL Edit]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Standardgränsen är den som anges i Admin.

1. Ange en ny gräns och klicka sedan på **[!UICONTROL Save]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   Den smarta kampanjen körs inte om antalet personer som är kvalificerade överstiger den angivna gränsen.

   >[!CAUTION]
   >
   >Var försiktig med den här funktionen så att du inte oavsiktligt tar med för många personer.
