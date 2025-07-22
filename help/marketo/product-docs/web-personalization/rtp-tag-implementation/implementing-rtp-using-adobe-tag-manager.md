---
unique-page-id: 4720218
description: Implementera RTP med Adobe Tag Manager - Marketo Docs - produktdokumentation
title: Implementera RTP med Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Implementera RTP med Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Följ installationsanvisningarna nedan för att implementera RTP-taggen:

1. Logga in på ditt RTP-konto.

1. Gå till **[!UICONTROL Account Settings]**.

   a. Om du redan har fått din JavaScript-tagg från Support fortsätter du till steg 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Under [!UICONTROL Domain] letar du reda på den relevanta domänen och klickar på **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Logga in på ditt [!DNL Dynamic Tag Manager]-konto ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Gå till **[!UICONTROL Dashboard].** Klicka på den relevanta webbegenskapen.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Gå till **[!UICONTROL Rules]**, klicka på **[!UICONTROL Create New Rule]**.

1. Fyll i följande

   1. [!UICONTROL Name]: **Marketo RTP**
   1. [!UICONTROL Conditions] (komprimering) : Utlösarregel vid - **[!UICONTROL Top of Page]**
   1. [!UICONTROL Javascript] (komprimera): klicka **[!UICONTROL Add New Script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Anropa den nya taggen: **Marketo RTP-tagg**

1. Ta bort följande kod från [!UICONTROL RTP tag]

   * `<script type='text/javascript'>`
   * `</script>`

1. Klistra in JavaScript-taggen RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Se till att du tar bort alla taggar och bara låter skriptet vara (nej `<script type='text/javascript'>` , `</script>` )

1. Klicka på **[!UICONTROL Save Code]** i skriptredigeraren och **[!UICONTROL Save Rule]** i regelredigeraren.

1. Leta reda på Marketo RTP-sidans inläsningsregel på panelen Regler och välj **[!UICONTROL Actions]** i listrutan **[!UICONTROL Activate Rules]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Verify]** att det visas på alla sidor, inklusive landningssidor och underdomäner.

   Du kan göra det genom att högerklicka på webbplatsens sidor. Gå till **[!UICONTROL Inspect Element]**, klicka på **[!UICONTROL Network]**, Sök: **RTP**.
