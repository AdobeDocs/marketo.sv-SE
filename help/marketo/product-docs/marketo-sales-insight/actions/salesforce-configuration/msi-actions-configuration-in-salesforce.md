---
description: MSI Actions Configuration in Salesforce - Marketo Docs - Product Documentation
title: MSI Actions Configuration in Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 84e3c4d525c5bde9e3ebd17d2f29ad42578777ff
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# MSI Actions Configuration in Salesforce {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installera]() eller [Uppgradera]() Sales Insight Package in your Salesforce instance Install/Upgrade to the [MSI-åtgärdspaket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) i Salesforce-instansen.
>* [Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited]()


## Add New Remote Site in Salesforce {#add-new-remote-site-in-salesforce}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Search for “remote site&quot; and select **Remote Site Settings**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Enter the Remote Site Name (it can be something like “MarketoSalesInsight”). Ange URL:en för fjärrplatsen (https://ims-na1-stg1.adobelogin.com) och klicka på **Spara**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Enabling MSI-Actions across the CRM {#enabling-msi-actions-across-the-crm}

1. In Salesforce, click the **Marketo Sales Insight Config** tab.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Om du inte ser &quot;Marketo Sales Insight Config&quot; i det övre fältet klickar du på **+** signera och hitta det under Alla flikar.

1. Välj **Aktivera MSI-åtgärder** kryssrutan.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Ange API-hemlig nyckel.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >If you don&#39;t have your API Secrey Key handy, you can find it by following the steps in [this article](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Click **Save** when done.

This will automatically enable all MSI Actions features outlined in the feature overview article.

>[!NOTE]
>
>Du kan inaktivera alla MSI-åtgärdsfunktioner genom att avmarkera kryssrutan Aktivera MSI-åtgärder.

## Styrning av MSI-åtgärder {#msi-actions-governance}

1. You can disable Sales Campaigns and/or the Task tab in the upcoming section. Detta gäller för lead-, kontakt-, konto- och affärsmöjlighetspanelerna.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. You can disable MSI Actions by unchecking corresponding features under Actions settings.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Governance settings are applicable to all MSI users.
