---
unique-page-id: 1900585
description: Lägg till redigerbara avsnitt i e-postmallar v1.0 - Marketo Docs - produktdokumentation
title: Lägg till redigerbara avsnitt i e-postmallar v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Lägg till redigerbara avsnitt i e-postmallar v1.0 {#add-editable-sections-to-email-templates-v1.0}

Om du skapar en mall i e-postmallsredigeraren v1.0 kan du göra vilket avsnitt som helst redigerbart genom att placera en särskild `<div>` runt det.

>[!NOTE]
>
>**Exempel**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regler:

1. HTML måste alltid vara giltigt.
1. Klassen **mktEditable** måste inkluderas.
1. ID:t måste vara unikt i denna HTML.
1. Inga blanksteg i ID:t.

>[!CAUTION]
>
>mktEditable-satser kan inte kapslas.

Om du vill lära dig hur du gör detta i e-postmallsredigeraren v2.0 kan du checka ut [e-postmallens syntax](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
