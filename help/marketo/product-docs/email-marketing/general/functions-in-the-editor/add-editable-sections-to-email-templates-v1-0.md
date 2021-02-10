---
unique-page-id: 1900585
description: Lägg till redigerbara avsnitt i e-postmallar v1.0 - Marketo Docs - Produktdokumentation
title: Lägg till redigerbara avsnitt i e-postmallar v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Lägg till redigerbara avsnitt i e-postmallar v1.0 {#add-editable-sections-to-email-templates-v1.0}

Om du skapar en mall i e-postmallsredigeraren v1.0 kan du göra alla avsnitt redigerbara genom att placera en `<div>`-special runt den.

>[!NOTE]
>
>**Exempel**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regler:

1. HTML-koden måste alltid vara giltig.
1. Klassen **mktEditable** måste inkluderas.
1. ID:t måste vara unikt i den HTML-koden.
1. Inga blanksteg i ID:t.

>[!CAUTION]
>
>mktEditable-satser kan inte kapslas.

Om du vill lära dig hur du gör detta i e-postmallsredigeraren v2.0 kan du gå till [e-postmallens syntax](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
