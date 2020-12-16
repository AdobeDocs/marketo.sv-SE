---
unique-page-id: 1147066
description: Åsidosätt personbegränsningar i en smart kampanj - Marketo Docs - produktdokumentation
title: Åsidosätt personbegränsningar i en smart kampanj
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---


# Åsidosätt personbegränsningar i en smart kampanj {#override-person-restrictions-in-a-smart-campaign}

Med Marketo kan du ange det högsta antalet* *personer som kan kvalificera sig för en smart kampanj; På så sätt slipper du oavsiktligt skicka hela databasen via e-post. Så här *åsidosätter* du den här gränsen.

>[!PREREQUISITES]
>
>Se till att du [aktiverar personbegränsningar för smarta kampanjer](../../../../product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) i Marketo Admin.

1. Gå till din** **smarta kampanj och klicka på **Schemalägg** i Marknadsföringsaktiviteter.

   ![](assets/one.png)

   Klicka på Redigera i Inställningar för smart kampanj.
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

