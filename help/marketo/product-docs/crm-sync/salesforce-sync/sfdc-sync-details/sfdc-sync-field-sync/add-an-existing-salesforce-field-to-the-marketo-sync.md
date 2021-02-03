---
unique-page-id: 4719308
description: Lägg till ett befintligt Salesforce-fält i Marketo Sync - Marketo Docs - Produktdokumentation
title: Lägg till ett befintligt Salesforce-fält i Marketo-synkronisering
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Lägg till ett befintligt Salesforce-fält i Marketo-synkronisering {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Vanligtvis synkroniseras nya anpassade fält i Salesforce automatiskt till Marketo. Annars kanske inte fälten visas för Marketo Sync-användaren. Så här kan du fixa det här.

1. Klicka på ditt namn och välj sedan **Inställningar**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Ange **profil** i det vänstra sökfältet och klicka på **Profiler** under **Hantera användare**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Klicka på synkroniseringsanvändarens profil.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Under avsnittet **Fältnivåsäkerhet** klickar du på **Visa** bredvid objektet som innehåller fältet.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Klicka på **Redigera**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Markera kryssrutan **Synlig** för fältet som du vill lägga till i synkroniseringen och klicka på **Spara**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Söt! I nästa synkroniseringscykel ser Marketo fältet och startar magin.

   >[!NOTE]
   >
   > Om fältet redan har värden i Salesforce synkroniseras dessa värden inte till Marketo förrän nästa postuppdatering.
