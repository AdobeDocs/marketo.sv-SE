---
description: Hur hanterar Sales Insight Actions borttagning av dubbletter via e-post - Marketo Docs - produktdokumentation
title: Hur hanterar Sales Insight-åtgärder borttagning av dubbletter av e-post
hide: true
hidefromtoc: true
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Hur hanterar Sales Insight-åtgärder borttagning av dubbletter via e-post? {#how-does-sales-insight-actions-handle-email-de-duping}

När du är [överföra en CSV-fil](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) i Sales Insight Actions sammanfogar vi alla som kontakter i CSV innan importen äger rum.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.
