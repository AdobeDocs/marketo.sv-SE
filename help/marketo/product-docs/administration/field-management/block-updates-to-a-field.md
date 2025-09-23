---
unique-page-id: 2360291
description: Blockera uppdateringar till ett fält - Marketo Docs - produktdokumentation
title: Blockera uppdateringar till ett fält
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Blockera uppdateringar till ett fält {#block-updates-to-a-field}

Genom att blockera uppdateringar av ett fält kan du skriva till fältet en gång och sedan behålla det ursprungliga värdet under fältets livstid. Detta kan vara användbart för ett fält som [!UICONTROL Person Source].

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Sök efter fältet, markera det och klicka sedan på **[!UICONTROL Field Actions]** under **[!UICONTROL Block Field Updates]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Du kan även blockera uppdateringar av [anpassade programmedlemsfält](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Markera **[!UICONTROL Input Sources]** som du vill blockera och klicka på **[!UICONTROL Apply]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >När du utför en listimport visas statusen för ett fält som blockeras i importförhandsvisningen endast om fältet identifieras automatiskt av Marketo baserat på namnet på fältet som matchar _exakt_ (eller om alias har upprättats). Om fältet väljs manuellt från listrutan Marketo-fält visas inte spärrstatusen i importförhandsvisningen, men uppdateringsblockering för det fältet kommer fortfarande att implementeras.
