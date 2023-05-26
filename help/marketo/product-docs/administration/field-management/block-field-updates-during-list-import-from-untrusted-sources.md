---
unique-page-id: 2360335
description: Blockera fältuppdateringar vid listimport från otillförlitliga källor - Marketo Docs - produktdokumentation
title: Blockera fältuppdateringar vid listimport från otillförlitliga källor
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Blockera fältuppdateringar vid listimport från otillförlitliga källor {#block-field-updates-during-list-import-from-untrusted-sources}

Du kan lita på data i vissa listor mer än andra. Ibland kan du ha tvivelaktiga data och vill ta dem om fältet är tomt, men inte om det finns ett befintligt värde. Du kan uppnå detta genom att blockera fältuppdateringar för nyckelfält.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Blockera fältuppdateringar från otillförlitliga källor {#blocking-field-updates-from-untrusted-sources}

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Hitta det fält du vill använda, markera det och sedan under **[!UICONTROL Field Actions]**, klicka **[!UICONTROL Block Field Updates]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Kontrollera **[!UICONTROL List Import untrusted source]** och klicka **[!UICONTROL Apply]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Du kan skydda fält från alla listor (tillförlitliga och ej tillförlitliga) genom att även kontrollera **[!UICONTROL List Import trusted source]**.

Upprepa stegen ovan för andra fält som du vill skydda från ej tillförlitliga listor.

## Köra en ej betrodd listimport {#running-an-untrusted-list-import}

1. Se till att du väljer **[!UICONTROL Untrusted]** om du vill att alla fält som du skapade i föregående steg ska vara säkra.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaljerade anvisningar om hur du importerar listor finns i [Importera en lista med personer](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Snyggt jobbat! Nu vet du hur du kan skydda nyckelfält från otillförlitliga listor.
