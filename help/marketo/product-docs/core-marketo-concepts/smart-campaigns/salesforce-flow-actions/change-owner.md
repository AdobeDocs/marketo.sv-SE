---
unique-page-id: 1147021
description: Ändra ägare - Marketo Docs - produktdokumentation
title: Ändra ägare
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Ändra ägare {#change-owner}

Om du har befintliga personer som redan har tilldelats en ägare kan du använda det här flödessteget för att tilldela dem till en annan ägare.

![](assets/change-owner-1.png)

1. Välj bara ägare eller lead-kö som du vill ändra till och gå till.

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] tillåter inte att kontakter tilldelas till lead-köer. För en post som är en SFDC-kontakt:
   >
   >* Marketo skapar en dubblett av lead **endast** när kontakten synkroniseras med Salesforce. Med andra ord, om du använder flödessteget **[Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** med `AssignTo=<a lead queue>`, skapar Marketo ett duplicerat lead i Salesforce och tilldelar det till lead-kön.
   >
   >* Om du använder flödessteget **[!UICONTROL Change Owner]** för en kontakt skapar Marketo en dubblettlead i Salesforce. Du undviker detta genom att använda ett filter i fältet&quot;SFDC Type&quot; som begränsar åtgärden till endast leads.

   >[!NOTE]
   >
   >Om posten ännu inte finns i ditt [!DNL Salesforce]-konto synkroniserar vi den och tilldelar den sedan till den valda användaren.
