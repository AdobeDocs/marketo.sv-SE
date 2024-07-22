---
description: Hur hanterar Sales Insight Actions borttagning av dubbletter via e-post - Marketo Docs - produktdokumentation
title: Hur hanterar Sales Insight-åtgärder borttagning av dubbletter av e-post
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Hur hanterar Sales Insight-åtgärder borttagning av dubbletter via e-post? {#how-does-sales-insight-actions-handle-email-de-duping}

När du [överför en CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md)-fil till Sales Insight Actions sammanfogas alla liknande kontakter i CSV-filen innan importen äger rum.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.
