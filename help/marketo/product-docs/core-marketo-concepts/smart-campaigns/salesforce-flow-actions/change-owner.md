---
unique-page-id: 1147021
description: Ändra ägare - Marketo Docs - produktdokumentation
title: Ändra ägare
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
source-git-commit: 44c134811242b4136a3137cdd60e60edeb838c8c
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Ändra ägare {#change-owner}

Om du har befintliga personer som redan har tilldelats en ägare kan du använda det här flödessteget för att tilldela dem till en annan ägare.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Användning**

1. Välj bara ägare eller lead-kö som du vill ändra till och gå till.

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce tillåter inte att kontakter tilldelas till lead-köer. För en post som är en SFDC-kontakt:
   >
   >1. Marketo skapar en dubblett av lead **endast** när kontakten synkroniseras med Salesforce. Med andra ord, om du använder **[Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** flöda steg med `AssignTo=<a lead queue>`skapar Marketo ett duplicerat lead i Salesforce och tilldelar det till lead-kön.
   >
   >1. Om du använder **Ändra ägare** flödessteg för en kontakt skapar Marketo en dubblett av lead i Salesforce. Du undviker detta genom att använda ett filter i fältet SFDC-typ som begränsar åtgärden till endast leads.


   >[!NOTE]
   >
   >Om posten ännu inte finns i ditt Salesforce-konto synkroniserar vi den och tilldelar den till den valda användaren.
