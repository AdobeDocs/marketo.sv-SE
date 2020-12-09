---
title: override-person-restrictions-in-a-smart-campaign
description: Åsidosätt personbegränsningar i en smart kampanj
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# Åsidosätt personbegränsningar i en smart kampanj

<br> 

Med Marketo kan ni ange det maximala antalet personer som kan kvalificera sig för en smart kampanj. På så sätt slipper du oavsiktligt skicka hela databasen via e-post. Så här åsidosätter du den här gränsen.

>[!IMPORTANT]
>
>Se till att du [aktiverar personbegränsningar för smarta kampanjer](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) i Marketo [!UICONTROL Admin].

1. Hitta din smarta kampanj och klicka **[!UICONTROL Schedule]**.

   ![Bild ett](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicka **[!UICONTROL Qualification Rules]**.

   ![Bild två](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Standardgränsen är den som anges i Admin.

1. Ange en ny gräns bredvid **[!UICONTROL Abort campaign if qualified leads exceed]**.

   ![Bild tre](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>Den smarta kampanjen körs inte om antalet personer som är kvalificerade överstiger den angivna gränsen.

>[!CAUTION]
>
>Var försiktig med den här funktionen så att du inte oavsiktligt tar med för många personer.
