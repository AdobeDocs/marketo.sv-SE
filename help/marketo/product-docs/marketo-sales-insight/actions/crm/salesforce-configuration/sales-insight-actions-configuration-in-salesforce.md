---
description: Konfiguration av Sales Insight Actions i Salesforce - Marketo Docs - produktdokumentation
title: Konfiguration av åtgärder för försäljningsinsikter i Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Konfiguration av åtgärder för försäljningsinsikter i Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installera](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) eller [Uppgradera](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Sales Insight Package in your Salesforce instance
>* [Konfigurera Marketo Sales Insight i Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Lägg till ny fjärrplats i Salesforce {#add-new-remote-site-in-salesforce}

1. I Salesforce klickar du på **Inställningar**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Sök efter&quot;fjärrwebbplats&quot; och välj **Inställningar för fjärrplats**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicka **Ny fjärrplats**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSalesInsight1&quot;). Ange URL för fjärrplatsen `https://ims-na1.adobelogin.com` och klicka **Spara**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Klicka **Ny fjärrplats** igen.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Ange namnet på fjärrplatsen (det kan vara något som &quot;MarketoSalesInsight2&quot;). Ange URL för fjärrplats `https://mkto-sales-connect.adobe.io` och klicka **Spara**.

## Aktivera åtgärder för säljinsikter i hela CRM {#enabling-sales-insight-actions-across-the-crm}

1. I Salesforce klickar du på **Marketo Sales Insight Config** -fliken.

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
   >Om du inte har tillgång till API:ts säkerhetsnyckel kan du hitta den genom att följa stegen i [den här artikeln](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Klicka **Spara** när det är klart.

Detta aktiverar automatiskt alla MSI-funktionsmakron som beskrivs i artikeln om funktionsöversikten.

>[!NOTE]
>
>Du kan inaktivera alla MSI-åtgärdsfunktioner genom att avmarkera kryssrutan Aktivera MSI-åtgärder.

## Styrning av MSI-åtgärder {#msi-actions-governance}

1. Du kan inaktivera Säljkampanjer och/eller fliken Uppgift i det kommande avsnittet. Detta gäller för lead-, kontakt-, konto- och affärsmöjlighetspanelerna.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Du kan inaktivera MSI-åtgärder genom att avmarkera motsvarande funktioner under Åtgärder.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Styrningsinställningar gäller för alla MSI-användare.
