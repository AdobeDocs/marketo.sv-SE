---
unique-page-id: 37355600
description: Avinstallera MSI från din MS Dynamics-instans - Marketo Docs - produktdokumentation
title: Avinstallera MSI från din MS Dynamics-instans
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Avinstallera MSI från din MS Dynamics-instans {#uninstall-msi-from-your-ms-dynamics-instance}

Om du vill avinstallera MSI från MS Dynamics-instansen måste du utföra steg i både Marketo och MS Dynamics.

>[!PREREQUISITES]
>
>[Inaktivera global MS Dynamics-synkronisering](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Klicka på **Admin** i Marketo.

   ![](assets/one-1.png)

1. Klicka på **Sales Insight**.

   ![](assets/six.png)

1. Klicka på **Redigera fältsynkronisering**.

   ![](assets/seven.png)

1. Markera kryssrutan **Inaktivera synkronisering** och klicka på **Spara**.

   >[!NOTE]
   >
   >Se till att du [inaktiverar Global MS Dynamics Sync](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) innan du inaktiverar fältsynkroniseringen.

   ![](assets/eight.png)

## Följande steg utförs i MS Dynamics-instansen: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Klicka på **Avancerade inställningar**.

1. Klicka på **Lösningar**.

1. Välj **Marketo Sales Insight** och klicka på borttagningsikonen.

1. När modala avinstallationslösningar visas klickar du på **OK**.

   Det tar vanligtvis cirka 20 minuter för MS Dynamics-lösningen att avinstallera helt. Men om du har en stor MS Dynamics-instans kan det ta lite längre tid.

   >[!NOTE]
   >
   >Kom ihåg att aktivera synkroniseringen för Global MS Dynamics när du har avinstallerat MSI.
