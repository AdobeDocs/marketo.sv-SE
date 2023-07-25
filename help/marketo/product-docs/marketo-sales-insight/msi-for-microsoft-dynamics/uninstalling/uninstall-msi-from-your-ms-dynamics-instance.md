---
unique-page-id: 37355600
description: Avinstallera MSI från din MS Dynamics-instans - Marketo Docs - produktdokumentation
title: Avinstallera MSI från din MS Dynamics-instans
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Avinstallera MSI från din MS Dynamics-instans {#uninstall-msi-from-your-ms-dynamics-instance}

Om du vill avinstallera MSI från MS Dynamics-instansen måste du utföra steg i både Marketo och MS Dynamics.

>[!PREREQUISITES]
>
>[Inaktivera global MS Dynamics-synkronisering](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. I Marketo klickar du på **Administratör**.

   ![](assets/one-1.png)

1. Klicka **Försäljningsinsikter**.

   ![](assets/six.png)

1. Klicka **Redigera fältsynkronisering**.

   ![](assets/seven.png)

1. Välj **Inaktivera synkronisering** kryssruta och klicka **Spara**.

   >[!NOTE]
   >
   >Se till att du [inaktivera Global MS Dynamics Sync](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) innan fältsynkroniseringen inaktiveras.

   ![](assets/eight.png)

## Följande steg utförs i MS Dynamics-instansen: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Klicka **Avancerade inställningar**.

1. Klicka **Lösningar**.

1. Välj **Marketo Sales Insight** och klicka på ikonen Ta bort.

1. När avinstallationslösningen visas klickar du på **OK**.

   Det tar vanligtvis cirka 20 minuter för MS Dynamics-lösningen att avinstallera helt. Men om du har en stor MS Dynamics-instans kan det ta lite längre tid.

   >[!NOTE]
   >
   >Kom ihåg att aktivera synkroniseringen för Global MS Dynamics när du har avinstallerat MSI.
