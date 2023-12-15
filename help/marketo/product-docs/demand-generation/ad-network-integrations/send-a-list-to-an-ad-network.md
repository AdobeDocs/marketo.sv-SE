---
description: Skicka en lista till ett annonsnätverk - Marketo Docs - produktdokumentation
title: Skicka en lista till ett annonsnätverk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Skicka en lista till ett annonsnätverk {#send-a-list-to-an-ad-network}

Lär dig skicka en statisk lista till LinkedIn, Facebook eller Google.

## Skicka en lista {#how-to-send-a-list}

1. I Marketo Engage väljer du en lista och klickar på **[!UICONTROL List Actions]** och markera **[!UICONTROL Send to Ad Network]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Välj mellan LinkedIn, Facebook eller Google (de andra alternativen är inte tillgängliga just nu). I det här exemplet väljer vi **[!UICONTROL LinkedIn]**. Klicka på **[!UICONTROL Next]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicka på **[!UICONTROL Audience]** och välj önskad målgrupp.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Om du någon gång behöver kontrollera kan du se målgruppen som en lista synkroniseras till via fliken Status.

1. Välj önskad penseltyp och klicka på **[!UICONTROL Update]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Om du väljer&quot;Aktivera kontinuerlig målgruppssynkronisering&quot; håller Marketo listan uppdaterad i det valda annonsnätverket när listan ändras i din Marketo-instans. Vi lägger båda till _och_ ta bort personer från målgruppen om de läggs till/tas bort från den statiska listan.

1. Och det är allt! Klicka **[!UICONTROL OK]** för att avsluta.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Vanliga frågor och svar {#faq}

**Kan en enda statisk lista synkroniseras med flera annonspubliker?**

Nej, en lista kan bara synkroniseras till en enda målgrupp.

**Om jag aktiverar kontinuerlig synkronisering med en befintlig annonspublik, kommer den befintliga publiken att ersättas?**

Nej, den befintliga publiken läggs till, inte ersätts.
