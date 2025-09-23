---
unique-page-id: 37355600
description: Avinstallera MSI från din MS [!DNL Dynamics] Instance - Marketo Docs - produktdokumentation
title: Avinstallera MSI från din MS [!DNL Dynamics] instans
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 3%

---

# Avinstallera MSI från din MS [!DNL Dynamics]-instans {#uninstall-msi-from-your-ms-dynamics-instance}

Om du vill avinstallera MSI från din MS [!DNL Dynamics]-instans måste du utföra steg i både Marketo och MS [!DNL Dynamics].

>[!PREREQUISITES]
>
>[Inaktivera globalt MS [!DNL Dynamics] Synkronisera](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. Klicka på **[!UICONTROL Admin]** i Marketo.

   ![](assets/one-1.png)

1. Klicka på **[!UICONTROL Sales Insight]**.

   ![](assets/six.png)

1. Klicka på **[!UICONTROL Edit Field Sync]**.

   ![](assets/seven.png)

1. Markera kryssrutan **[!UICONTROL Disable Sync]** och klicka på **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Se till att du [inaktiverar Global MS Dynamics Sync](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) innan du inaktiverar fältsynkroniseringen.

   ![](assets/eight.png)

## Följande steg utförs i din MS [!DNL Dynamics]-instans: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Klicka på **[!UICONTROL Advanced Settings]**.

1. Klicka på **[!UICONTROL Solutions]**.

1. Markera **[!UICONTROL Marketo Sales Insight]** och klicka på borttagningsikonen.

1. När modala avinstallationslösningar visas klickar du på **[!UICONTROL OK]**.

   Det tar vanligtvis cirka 20 minuter för MS [!DNL Dynamics]-lösningen att avinstallera helt. Om du har en stor MS [!DNL Dynamics]-instans kan det dock ta lite längre tid.

   >[!NOTE]
   >
   >Kom ihåg att aktivera synkroniseringen av den globala MS:n [!DNL Dynamics] när du har avinstallerat MSI.
