---
description: Skicka en lista till ett annonsnätverk - Marketo Docs - produktdokumentation
title: Skicka en lista till ett annonsnätverk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Skicka en lista till ett annonsnätverk {#send-a-list-to-an-ad-network}

Lär dig hur du skickar en statisk lista till LinkedIn, Facebook eller Google.

## Skicka en lista {#how-to-send-a-list}

1. I Marketo väljer du en lista och klickar på **Liståtgärder** och markera **Skicka till annonsnätverk**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Välj mellan LinkedIn, Facebook eller Google (de andra alternativen är inte tillgängliga just nu). I det här exemplet väljer vi **linkedIn**. Klicka **Nästa**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicka på listrutan Målgrupp och välj önskad målgrupp.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Om du någon gång behöver kontrollera kan du se målgruppen som en lista synkroniseras till via fliken Status.

1. Välj önskad penseltyp och klicka på **Uppdatera**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Om du väljer&quot;Aktivera kontinuerlig målgruppssynkronisering&quot; håller Marketo listan uppdaterad i det valda annonsnätverket när listan ändras i din Marketo-instans. Vi lägger båda till **och** ta bort personer från målgruppen om de läggs till/tas bort från den statiska listan.

1. Och det är allt! Klicka **OK** för att avsluta.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Vanliga frågor {#faq}

**Kan en enda statisk lista synkroniseras med flera annonspubliker?**

Nej, en lista kan bara synkroniseras till en enda målgrupp.

**Om jag aktiverar kontinuerlig synkronisering med en befintlig annonspublik, kommer den befintliga publiken att ersättas?**

Nej, den befintliga publiken läggs till, inte ersätts.
