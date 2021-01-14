---
unique-page-id: 2360335
description: Blockera fältuppdateringar vid listimport från otillförlitliga källor - Marketo Docs - produktdokumentation
title: Blockera fältuppdateringar vid listimport från otillförlitliga källor
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
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

1. Leta reda på fältet du vill använda, markera det och klicka sedan på **Blockera fältuppdateringar** under **Fältåtgärder**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Markera **List Import untrusted source** och klicka på **Apply**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Du kan skydda fält från alla listor (tillförlitliga och ej tillförlitliga) genom att kontrollera **Lista importera betrodd källa**.

Upprepa stegen ovan för andra fält som du vill skydda från ej tillförlitliga listor.

## Köra en ej betrodd listimport {#running-an-untrusted-list-import}

1. När du kör listimporten måste du markera **Otillförlitlig** om du vill att alla fält som du konfigurerade i föregående steg ska vara säkra.

   ![](assets/importpersondetails.jpg)

Detaljerade anvisningar om hur du importerar listor finns i [Importera en lista med personer](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Snyggt jobbat! Nu vet du hur du kan skydda nyckelfält från otillförlitliga listor.
