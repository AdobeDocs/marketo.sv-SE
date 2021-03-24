---
description: Redigera fält som ska synkroniseras innan de tas bort i Dynamics - Marketo Docs - produktdokumentation
title: Redigera fält som ska synkroniseras innan de tas bort i Dynamics
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---


# Redigera fält som ska synkroniseras innan de tas bort i Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Ibland kanske du vill ta bort fält i Dynamics. Marketo behåller fältlistan som referens för synkroniseringen. Om ett fält tas bort i Dynamics medan synkroniseringen är aktiverad kan det uppstå fel i synkroniseringen. Följ stegen nedan innan du tar bort några fält.

1. I Marketo klickar du på **Admin**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Klicka på **Microsoft Dynamics** under Integrering.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicka på **Inaktivera synkronisering**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. På en ny flik i webbläsaren loggar du in i Dynamics och tar bort de önskade fälten.

1. I Marketo klickar du under Microsoft Dynamics på **Redigera** bredvid&quot;Steg 2: Välj fält att synkronisera.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Granska fälten och klicka på **Spara**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Du måste klicka på **Spara** för att spara det uppdaterade schemat för synkroniseringen, även om inga ändringar har gjorts.

>[!NOTE]
>
>Om synkroniseringen inte stoppas innan ett fält i Dynamics tas bort kan det uppstå fel i synkroniseringen. Om det gör det avbryts synkroniseringen. Innan du fortsätter måste Marketo Admin granska Välj fält att synkronisera (beskrivs ovan) och klicka på **Spara** för att synkroniseringen ska acceptera schemaändringarna.

Kom ihåg att aktivera synkroniseringen när ändringarna har sparats!
