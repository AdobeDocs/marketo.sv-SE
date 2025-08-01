---
description: Sales Insight Actions Configuration in Salesforce - Marketo Docs - Product Documentation
title: Konfiguration av Sales Insight Actions i Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# [!DNL Sales Insight Actions]-konfiguration i [!DNL Salesforce] {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installera](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) eller [Uppgradera](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) säljannonspaket i din [!DNL Salesforce]-instans
>* [Konfigurera Marketo Sales Insight i [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Lägg till ny fjärrplats i [!DNL Salesforce] {#add-new-remote-site-in-salesforce}

1. Klicka på [!DNL Salesforce] i **[!UICONTROL Setup]**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Sök efter [!UICONTROL remote site] och välj **[!UICONTROL Remote Site Settings]**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicka på **[!UICONTROL New Remote Site]**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSalesInsight1&quot;). Ange URL:en för fjärrplatsen `https://ims-na1.adobelogin.com` och klicka på **[!UICONTROL Save]**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Klicka på **[!UICONTROL New Remote Site]** igen.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSalesInsight2&quot;). Ange URL för fjärrplatsen `https://mkto-sales-connect.adobe.io` och klicka på **[!UICONTROL Save]**.

## Aktivera [!DNL Sales Insight Actions] i CRM {#enabling-sales-insight-actions-across-the-crm}

1. Klicka på fliken [!DNL Salesforce] i **[!UICONTROL Marketo Sales Insight Config]**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Om du inte ser [!UICONTROL Marketo Sales Insight Config] i det övre fältet klickar du på **+**-tecknet och hittar det under Alla flikar.

1. Markera kryssrutan **[!UICONTROL Enable MSI Actions]**.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Ange [!UICONTROL API Secret Key].

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Om du inte har tillgång till din [!UICONTROL API Secrey Key] kan du hitta den genom att följa stegen i [den här artikeln](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Klicka på **[!UICONTROL Save]** när du är klar.

Detta aktiverar automatiskt alla MSI-funktionsmakron som beskrivs i artikeln om funktionsöversikten.

>[!NOTE]
>
>Du kan inaktivera alla MSI-åtgärdsfunktioner genom att avmarkera kryssrutan Aktivera MSI-åtgärder.

## Styrning av MSI-åtgärder {#msi-actions-governance}

1. Du kan inaktivera Säljkampanjer och/eller fliken Uppgift i det kommande avsnittet. Detta gäller för lead-, kontakt-, konto- och affärsmöjlighetspanelerna.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Du kan inaktivera MSI-åtgärder genom att avmarkera motsvarande funktioner under [!UICONTROL Actions settings].

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Styrningsinställningar gäller för alla MSI-användare.
