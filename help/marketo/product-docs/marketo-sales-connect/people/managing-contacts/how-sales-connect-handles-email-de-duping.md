---
unique-page-id: 14352514
description: How Sales Connect Handles Email Deduplicing - Marketo Docs - Product Documentation
title: Hur Sales Connect hanterar borttagning av dubbletter av e-post
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Hur Sales Connect hanterar e-postborttagning av dubbletter {#how-sales-connect-handles-email-de-duping}

När du [överför en CSV](http://docs.marketo.com/x/VADb)-fil till Sales Connect sammanfogas alla liknande kontakter i CSV-filen innan importen äger rum.

Vi gör detta baserat på e-postadressen. Om det finns två identiska e-postadresser sammanfogar vi dem till en kontakt.

Om du senare försöker lägga till/överföra samma kontakt manuellt, sammanfogas den inte.

Om du försöker lägga till en kontakt som redan finns i databasen kommer du inte att kunna lägga till den.

