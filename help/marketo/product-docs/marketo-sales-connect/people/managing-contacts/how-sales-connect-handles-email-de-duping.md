---
unique-page-id: 14352514
description: How Sales Connect Handles Email Deduplicing - Marketo Docs - Product Documentation
title: Hur Sales Connect hanterar e-postborttagning av dubbletter
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 0%

---

# Hur [!DNL Sales Connect] hanterar borttagning av dubbletter av e-post {#how-sales-connect-handles-email-de-duping}

När du [överför en CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)-fil till [!DNL Sales Connect] sammanfogas alla liknande kontakter i CSV-filen innan importen sker.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.
