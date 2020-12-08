---
unique-page-id: 2360335
description: Blockera fältuppdateringar vid listimport från otillförlitliga källor - Marketo Docs - produktdokumentation
title: Blockera fältuppdateringar vid listimport från otillförlitliga källor
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Blockera fältuppdateringar vid listimport från otillförlitliga källor {#block-field-updates-during-list-import-from-untrusted-sources}

Du kan lita på data i vissa listor mer än andra. Ibland kan du ha tvivelaktiga data och vill ta dem om fältet är tomt, men inte om det finns ett befintligt värde. Du kan uppnå detta genom att blockera fältuppdateringar för nyckelfält.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Blockera fältuppdateringar från otillförlitliga källor {#blocking-field-updates-from-untrusted-sources}

1. Gå till **Admin** och klicka på **Fälthantering**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Leta reda på fältet som du vill ha, markera det och klicka sedan på Blockera **fältuppdateringar** under **Fältåtgärder**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Markera **Listimport som ej betrodd källa** och klicka på **Använd**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Du kan skydda fält från alla listor (tillförlitliga och ej tillförlitliga) genom att även markera **List Import trusted source**.

Upprepa stegen ovan för andra fält som du vill skydda från ej tillförlitliga listor.

## Köra en ej betrodd listimport {#running-an-untrusted-list-import}

1. När du kör listimporten måste du markera **Ej betrodd **om du vill att alla fält som du konfigurerade i föregående steg ska vara säkra.

   ![](assets/importpersondetails.jpg)

Detaljerade anvisningar om hur du importerar listor finns i [Importera en lista med personer](../../../getting-started/quick-wins/import-a-list-of-people.md).

Snyggt jobbat! Nu vet du hur du kan skydda nyckelfält från otillförlitliga listor.
