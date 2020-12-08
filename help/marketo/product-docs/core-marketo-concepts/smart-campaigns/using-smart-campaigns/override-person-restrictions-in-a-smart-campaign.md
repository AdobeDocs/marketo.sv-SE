---
unique-page-id: 1147066
description: Åsidosätt personbegränsningar i en smart kampanj - Marketo Docs - produktdokumentation
title: Åsidosätt personbegränsningar i en smart kampanj
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Åsidosätt personbegränsningar i en smart kampanj {#override-person-restrictions-in-a-smart-campaign}

Med Marketo kan du ange det högsta antalet* *personer som kan kvalificera sig för en smart kampanj; På så sätt slipper du oavsiktligt skicka hela databasen via e-post. Så här *åsidosätter* du den här gränsen.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Förutsättningar**
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

