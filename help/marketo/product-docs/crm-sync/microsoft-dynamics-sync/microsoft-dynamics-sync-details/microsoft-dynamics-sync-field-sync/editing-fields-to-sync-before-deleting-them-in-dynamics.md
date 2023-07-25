---
description: Redigera fält som ska synkroniseras innan de tas bort i Dynamics - Marketo Docs - produktdokumentation
title: Redigera fält som ska synkroniseras innan de tas bort i Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Redigera fält som ska synkroniseras innan de tas bort i Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Ibland kanske du vill ta bort fält i Dynamics. Marketo behåller fältlistan som referens för synkroniseringen. Om ett fält tas bort i Dynamics medan synkroniseringen är aktiverad kan det uppstå fel i synkroniseringen. Följ stegen nedan innan du tar bort några fält.

1. I Marketo klickar du på **Administratör**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Under Integrering klickar du på **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicka **Inaktivera synkronisering**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. På en ny flik i webbläsaren loggar du in i Dynamics och tar bort de önskade fälten.

1. I Marketo, under Microsoft Dynamics, klickar du **Redigera** bredvid&quot;Steg 2: Välj fält att synkronisera.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Granska fälten och klicka **Spara**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Klicka **Spara** krävs för att spara det uppdaterade schemat för synkroniseringen, även om inga ändringar gjorts.

>[!NOTE]
>
>Om synkroniseringen inte stoppas innan ett fält i Dynamics tas bort kan det uppstå fel i synkroniseringen. Om det gör det avbryts synkroniseringen. Innan du fortsätter måste Marketo Admin granska&quot;Välj fält att synkronisera&quot; (som beskrivs ovan) och klicka på **Spara** för att synkroniseringen ska acceptera schemaändringarna.

Kom ihåg att aktivera synkroniseringen när ändringarna har sparats!
