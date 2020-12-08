---
unique-page-id: 2360291
description: Blockera uppdateringar till ett fält - Marketo Docs - Produktdokumentation
title: Blockera uppdateringar till ett fält
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# Blockera uppdateringar till ett fält {#block-updates-to-a-field}

Genom att blockera uppdateringar av ett fält kan du skriva till fältet en gång och sedan behålla det ursprungliga värdet under fältets livstid. Detta kan vara användbart för ett fält som Personkälla.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Admin** och klicka på **Fälthantering**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Leta reda på fältet, markera det och klicka sedan på **Blockera fältuppdateringar** under **Fältåtgärder**.

   ![](assets/two-1.png)

1. Markera de **indatakällor** som du vill blockera och klicka på **Använd**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >När du utför en listimport visas statusen för ett fält som blockeras i importförhandsvisningen endast om fältet identifieras automatiskt av Marketo baserat på namnet på det fält som matchar **exakt** (eller om alias har upprättats). Om fältet väljs manuellt från listrutan Marketfält visas inte spärrstatusen i importförhandsvisningen, men uppdateringsblockering för det fältet kommer fortfarande att implementeras.

