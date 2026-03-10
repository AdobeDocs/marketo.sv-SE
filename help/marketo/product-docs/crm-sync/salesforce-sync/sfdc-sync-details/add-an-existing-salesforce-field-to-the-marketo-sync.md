---
unique-page-id: 4719308
description: Lär dig hur du lägger till ett befintligt Salesforce-fält i Marketo-synkroniseringen. Gör fältet synligt för synkroniseringsanvändaren i Salesforce så att det synkroniseras i nästa cykel.
title: Lägg till ett befintligt Salesforce-fält i Marketo Sync
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Lägg till ett befintligt [!DNL Salesforce]-fält i Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

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

1. Klicka **[!UICONTROL Field-Level Security]** bredvid objektet som innehåller fältet under avsnittet **[!UICONTROL View]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicka på **[!UICONTROL Edit]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Markera kryssrutan **[!UICONTROL Visible]** för fältet som du vill lägga till i synkroniseringen och klicka på **[!UICONTROL Save]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   I nästa synkroniseringscykel kommer Marketo att se fältet och starta magin.

   >[!NOTE]
   >
   > Om fältet redan har värden i [!DNL Salesforce] synkroniseras dessa värden inte till Marketo förrän nästa postuppdatering.
