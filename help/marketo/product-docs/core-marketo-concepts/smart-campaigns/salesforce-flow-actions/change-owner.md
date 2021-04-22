---
unique-page-id: 1147021
description: Ändra ägare - Marketo Docs - produktdokumentation
title: Ändra ägare
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
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
   >1. Marketo skapar endast en dubblett av lead **när kontakten synkroniseras med Salesforce.** Med andra ord, om du använder flödessteget **[Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** med `AssignTo=<a lead queue>`, skapar Marketo en dubblett av lead i Salesforce och tilldelar den till lead-kön.
      >
      >
   1. Om du försöker använda flödessteget **Ändra ägare** för en kontakt skapas ingen dubblett i Salesforce.


   >[!NOTE]
   >
   >Om posten ännu inte finns i ditt Salesforce-konto synkroniserar vi den och tilldelar den till den valda användaren.
