---
unique-page-id: 1147066
description: Åsidosätt personbegränsningar i en smart kampanj - Marketo Docs - produktdokumentation
title: Åsidosätt personbegränsningar i en smart kampanj
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 0%

---

# Åsidosätt personbegränsningar i en smart kampanj {#override-person-restrictions-in-a-smart-campaign}

Med Marketo Engage kan ni ange det maximala antalet personer som kan kvalificera sig för en smart kampanj, vilket hjälper er att undvika att skicka hela databasen med e-post av misstag. Om du vill _åsidosätta_ den här gränsen, så här.

>[!PREREQUISITES]
>
>Se till att [aktivera personbegränsningar för smarta kampanjer](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} i Marketo Admin.

1. I **[!UICONTROL Marketing Activities]**, gå till din smarta kampanj och klicka på **[!UICONTROL Schedule]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicka på Inställningar för smart kampanj **[!UICONTROL Edit]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Standardgränsen är den som anges i Admin.

1. Ange en ny gräns och klicka på **[!UICONTROL Save]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   Den smarta kampanjen körs inte om antalet personer som är kvalificerade överstiger den angivna gränsen.

   >[!CAUTION]
   >
   >Var försiktig med den här funktionen så att du inte oavsiktligt tar med för många personer.
