---
unique-page-id: 4719308
description: Lägg till ett befintligt Salesforce-fält i Marketo Sync - Marketo Docs - produktdokumentation
title: Lägg till ett befintligt Salesforce-fält i Marketo Sync
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Lägg till ett befintligt Salesforce-fält i Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

Vanligtvis synkroniseras nya anpassade fält i Salesforce automatiskt till Marketo. Annars kanske inte fälten visas för Marketo Sync-användaren. Så här kan du fixa det här.

1. Klicka på ditt namn och välj sedan **Inställningar**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Retur **profil** i det vänstra sökfältet och klicka på **Profiler** under **Hantera användare**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicka på synkroniseringsanvändarens profil.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Under **Fältnivåsäkerhet** avsnitt, klicka **Visa** bredvid objektet som innehåller fältet.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicka **Redigera**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Kontrollera **Synlig** kryssrutan för fältet som du vill lägga till i synkroniseringen och klicka **Spara**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Söt! I nästa synkroniseringscykel kommer Marketo att se fältet och starta magin.

   >[!NOTE]
   >
   > Om fältet redan har värden i Salesforce synkroniseras dessa värden inte till Marketo förrän nästa postuppdatering.
