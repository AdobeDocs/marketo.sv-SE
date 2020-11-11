---
title: define-a-smart-list-for-a-batch-campaign
description: Definiera en smart lista för en batchkampanj
translation-type: tm+mt
source-git-commit: cd1b7e65c73de0b31f20289402f1c0832c382b33
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# Definiera en smart lista för en batchkampanj

<br> 

Smarta listor är en mekanism i hela Marketo för att definiera&quot;vem&quot; (vilka personer) som ska inkluderas, oavsett om det är en rapport, en lista eller en smart kampanj. Så här definierar du en smart lista för en batchkampanj.

1. Välj en smart kampanj och klicka sedan på [!UICONTROL **Smart lista**].

   ![Bild ett](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Skriv om du vill söka efter ett filter och sedan dra och släppa det på arbetsytan. Upprepa för flera filter.

   ![Bild två](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >En smart kampanj med bara filter körs i gruppläge. Den hittar personer i databasen som är kvalificerade baserat på filtren och kör alla via flödet samtidigt.

   >[!IMPORTANT]
   >
   >Du kan få en smart kampanj att köras på en person i taget baserat på live-händelser genom att lägga till utlösare, vilket gör att den smarta kampanjen aktiveras i utlösarläget.

1. Klicka på listrutan och välj en filteroperator (t.ex. [!UICONTROL **is**], [!UICONTROL **is not**], o.s.v.) för filtret du valde.

   ![Bild tre](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Röda linjer indikerar fel eller att information saknas. Om den inte korrigeras blir kampanjen ogiltig och körs inte.

1. Ange filtervärdet.

   ![Bild fyra](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Som standard är personer som uppfyller alla smarta listregler
>kvalificerade. Detta kan ändras för att passa era kampanjbehov. Läs [Smart List Rules for Complex Logic](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic) om du vill veta mer.
>
>Lär dig hur du [definierar smarta listor för smarta kampanjer om du vill aktivera direktsända händelser en person i taget | Utlösare](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
