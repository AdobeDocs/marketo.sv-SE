---
unique-page-id: 2360335
description: Blockera fältuppdateringar vid listimport från otillförlitliga källor - Marketo Docs - produktdokumentation
title: Blockera fältuppdateringar vid listimport från otillförlitliga källor
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
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

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Hitta det fält du vill använda, markera det och klicka sedan på **[!UICONTROL Block Field Updates]** under **[!UICONTROL Field Actions]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Markera **[!UICONTROL List Import untrusted source]** och klicka på **[!UICONTROL Apply]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Du kan skydda fält från alla listor, betrodda och ej tillförlitliga, genom att även kontrollera **[!UICONTROL List Import trusted source]**.

Upprepa stegen ovan för andra fält som du vill skydda från ej tillförlitliga listor.

## Köra en ej betrodd listimport {#running-an-untrusted-list-import}

1. När du kör listimporten ska du markera **[!UICONTROL Untrusted]** om du vill att alla fält som du konfigurerade i föregående steg ska vara säkra.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaljerade instruktioner om hur du importerar listor finns i [Importera en lista med personer](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Snyggt jobbat! Nu vet du hur du kan skydda nyckelfält från otillförlitliga listor.
