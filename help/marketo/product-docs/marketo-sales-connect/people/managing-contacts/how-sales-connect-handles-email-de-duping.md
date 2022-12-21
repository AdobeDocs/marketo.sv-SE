---
unique-page-id: 14352514
description: How Sales Connect Handles Email Deduplicing - Marketo Docs - Product Documentation
title: Hur Sales Connect hanterar borttagning av dubbletter av e-post
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Hur Sales Connect hanterar borttagning av dubbletter av e-post {#how-sales-connect-handles-email-de-duping}

När du är [överföra en CSV-fil](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) till Sales Connect, vi sammanfogar alla som kontakter i CSV-filen innan importen äger rum.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.
