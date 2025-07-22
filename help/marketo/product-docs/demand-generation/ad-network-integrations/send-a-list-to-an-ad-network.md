---
description: Skicka en lista till ett annonsnätverk - Marketo Docs - produktdokumentation
title: Skicka en lista till ett annonsnätverk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---

# Skicka en lista till ett annonsnätverk {#send-a-list-to-an-ad-network}

Lär dig hur du skickar en statisk lista till [!DNL LinkedIn], [!DNL Facebook] eller Google.

## Skicka en lista {#how-to-send-a-list}

1. I Marketo väljer du din lista, klickar på listrutan **[!UICONTROL List Actions]** och väljer **[!UICONTROL Send to Ad Network]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Välj mellan [!DNL LinkedIn], [!DNL Facebook] eller Google (de andra alternativen är inte tillgängliga just nu). I detta exempel väljer vi **[!DNL LinkedIn]**. Klicka på **[!UICONTROL Next]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicka på listrutan **[!UICONTROL Audience]** och välj önskad målgrupp.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Om du någon gång behöver kontrollera kan du se målgruppen som en lista synkroniseras till via fliken Status.

1. Välj önskad [!UICONTROL Push Type] och klicka på **[!UICONTROL Update]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Om du väljer [!UICONTROL Enable continuous audience sync] håller Marketo listan uppdaterad i det valda annonsnätverket när listan ändras i din Marketo-instans. Vi lägger båda till **och** till att ta bort personer från målgruppen om de läggs till/tas bort från den statiska listan.

1. Och det är allt! Klicka på **[!UICONTROL OK]** för att avsluta.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Vanliga frågor och svar {#faq}

**Kan en enskild statisk lista synkroniseras med flera annonspubliker?**

Nej, en lista kan bara synkroniseras till en enda målgrupp.

**Om jag aktiverar kontinuerlig synkronisering med en befintlig annonspublik, ersätts den befintliga publiken?**

Nej, den befintliga publiken läggs till, inte ersätts.
