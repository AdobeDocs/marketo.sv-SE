---
description: MSI Actions Configuration in Salesforce - Marketo Docs - Product Documentation
title: Konfigurering av MSI-åtgärder i Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: daff9a98605b8a5c89c538f711fecb5b7a382f84
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Konfigurering av MSI-åtgärder i Salesforce {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>Installera/uppgradera till [MSI-åtgärdspaket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) i Salesforce-instansen.

## Aktivera MSI-åtgärder i CRM {#enabling-msi-actions-across-the-crm}

1. I Salesforce klickar du på **Marketo Sales Insight Config** -fliken.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

   >[!NOTE]
   >
   >Om du inte ser &quot;Marketo Sales Insight Config&quot; i det övre fältet klickar du på **+** signera och hitta det under Alla flikar.

1. Välj **Aktivera MSI-åtgärder** kryssrutan.

   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Ange API-hemlig nyckel.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

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

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Du kan inaktivera MSI-åtgärder genom att avmarkera motsvarande funktioner under Åtgärder.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

>[!NOTE]
>
>Styrningsinställningar gäller för alla MSI-användare.
