---
unique-page-id: 2360335
description: Blockera fältuppdateringar vid listimport från otillförlitliga källor - Marketo Docs - produktdokumentation
title: Blockera fältuppdateringar vid listimport från otillförlitliga källor
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Blockera fältuppdateringar vid listimport från otillförlitliga källor {#block-field-updates-during-list-import-from-untrusted-sources}

Du kan lita på data i vissa listor mer än andra. Ibland kan du ha tvivelaktiga data och vill ta dem om fältet är tomt, men inte om det finns ett befintligt värde. Du kan uppnå detta genom att blockera fältuppdateringar för nyckelfält.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Blockera fältuppdateringar från otillförlitliga källor {#blocking-field-updates-from-untrusted-sources}

1. Gå till **Administratör** område.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicka **Fälthantering**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Hitta det fält du vill använda, markera det och sedan under **Fältåtgärder**, klicka **Blockera fältuppdateringar**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Kontrollera **Lista Importera ej betrodd källa** och klicka **Använd**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Du kan skydda fält från alla listor (tillförlitliga och ej tillförlitliga) genom att även kontrollera **Lista Importera betrodd källa**.

Upprepa stegen ovan för andra fält som du vill skydda från ej tillförlitliga listor.

## Köra en ej betrodd listimport {#running-an-untrusted-list-import}

1. Se till att du väljer **Otillförlitlig** om du vill att alla fält som du skapade i föregående steg ska vara säkra.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaljerade anvisningar om hur du importerar listor finns i [Importera en lista med personer](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Snyggt jobbat! Nu vet du hur du kan skydda nyckelfält från otillförlitliga listor.
