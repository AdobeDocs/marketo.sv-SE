---
description: Redigera fält som ska synkroniseras innan de tas bort i Dynamics - Marketo Docs - produktdokumentation
title: Redigera fält som ska synkroniseras innan de tas bort i Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Redigerar fält som ska synkroniseras innan de tas bort i [!DNL Dynamics] {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Ibland kanske du vill ta bort fält i [!DNL Dynamics]. Marketo behåller fältlistan som referens för synkroniseringen. Om ett fält tas bort i [!DNL Dynamics] när synkroniseringen är aktiverad kan det uppstå fel i synkroniseringen. Följ stegen nedan innan du tar bort några fält.

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Klicka på [!UICONTROL Integration] under **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicka på **[!UICONTROL Disable Sync]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Logga in på [!DNL Dynamics] och ta bort de önskade fälten på en ny flik i webbläsaren.

1. I Marketo, under [!DNL Microsoft Dynamics], klickar du på **[!UICONTROL Edit]** bredvid [!UICONTROL Step 2: Select Fields to Sync].

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Granska fälten och klicka på **[!UICONTROL Save]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Du måste klicka på **[!UICONTROL Save]** för att spara det uppdaterade schemat för synkroniseringen, även om inga ändringar har gjorts.

>[!NOTE]
>
>Om synkroniseringen inte stoppas innan du tar bort ett fält i [!DNL Dynamics] kan det uppstå fel i synkroniseringen. Om det gör det avbryts synkroniseringen. Marketo Admin måste granska [!UICONTROL Select Fields to Sync] (beskrivs ovan) och klicka på **[!UICONTROL Save]** för att synkroniseringen ska acceptera schemaändringarna innan du fortsätter.

Kom ihåg att aktivera synkroniseringen när ändringarna har sparats!
