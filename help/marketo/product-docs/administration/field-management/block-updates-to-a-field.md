---
unique-page-id: 2360291
description: Blockera uppdateringar till ett fält - Marketo Docs - produktdokumentation
title: Blockera uppdateringar till ett fält
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Blockera uppdateringar till ett fält {#block-updates-to-a-field}

Genom att blockera uppdateringar av ett fält kan du skriva till fältet en gång och sedan behålla det ursprungliga värdet under fältets livstid. Detta kan vara användbart för ett fält som Personkälla.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till **Administratör** område.

   ![](assets/block-updates-to-a-field-1.png)

1. Klicka **Fälthantering**.

   ![](assets/block-updates-to-a-field-2.png)

1. Sök efter fältet, markera det och sedan under **Fältåtgärder**, klicka **Blockera fältuppdateringar**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Du kan blockera uppdateringar till [Anpassade fält för programmedlem](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) också.

1. Välj **Indatakällor** du vill blockera och klicka **Använd**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >När du utför en listimport visas statusen för ett fält som blockeras i importförhandsvisningen endast om fältet identifieras automatiskt av Marketo baserat på namnet på det fält som matchar _exakt_ (eller om alias upprättas). Om fältet väljs manuellt från listrutan Marketo-fält visas inte spärrstatusen i importförhandsvisningen, men uppdateringsblockering för det fältet kommer fortfarande att implementeras.
