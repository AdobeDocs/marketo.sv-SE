---
title: override-person-restrictions-in-a-smart-campaign
description: Åsidosätt personbegränsningar i en smart kampanj
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---

# Åsidosätt personbegränsningar i en smart kampanj

<br> 

Med Marketo kan ni ange det högsta antalet personer som kan kvalificera sig för en smart kampanj. På så sätt slipper du oavsiktligt skicka hela databasen via e-post. Så här åsidosätter du den här gränsen.

>[!IMPORTANT]
>
>Var noga med att [aktivera personbegränsningar för smarta kampanjer](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) i Marketo [!UICONTROL Admin].

1. Hitta din smarta kampanj och klicka på **[!UICONTROL Schedule]**.

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
