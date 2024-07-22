---
unique-page-id: 4719308
description: Lägg till ett befintligt Salesforce-fält i Marketo Sync - Marketo Docs - produktdokumentation
title: Lägg till ett befintligt Salesforce-fält i Marketo Sync
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---

# Lägg till ett befintligt Salesforce-fält i Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Vanligtvis synkroniseras nya anpassade fält i Salesforce automatiskt till Marketo Engage. Annars kanske inte fälten visas för Marketo Sync-användaren. Så här kan du fixa det här.

1. Klicka på ditt namn och välj sedan **[!UICONTROL Setup]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Skriv &quot;profile&quot; i det vänstra sökfältet och klicka på **[!UICONTROL Profiles]** under **[!UICONTROL Manage Users]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicka på synkroniseringsanvändarens profil.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Klicka **[!UICONTROL View]** bredvid objektet som innehåller fältet under avsnittet **[!UICONTROL Field-Level Security]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Markera kryssrutan **[!UICONTROL Visible]** för fältet som du vill lägga till i synkroniseringen och klicka på **[!UICONTROL Save]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   I nästa synkroniseringscykel kommer Marketo att se fältet och starta magin.

   >[!NOTE]
   >
   > Om fältet redan har värden i Salesforce synkroniseras dessa värden inte till Marketo förrän nästa postuppdatering.
