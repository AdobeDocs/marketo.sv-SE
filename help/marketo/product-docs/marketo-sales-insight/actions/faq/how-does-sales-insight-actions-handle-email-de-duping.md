---
description: Hur hanterar Sales Insight Actions borttagning av dubbletter via e-post - Marketo Docs - produktdokumentation
title: Hur hanterar Sales Insight-åtgärder borttagning av dubbletter av e-post
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Hur hanterar Sales Insight-åtgärder borttagning av dubbletter via e-post? {#how-does-sales-insight-actions-handle-email-de-duping}

När du är [överföra en CSV-fil](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) i Sales Insight Actions sammanfogar vi alla som kontakter i CSV innan importen äger rum.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.
