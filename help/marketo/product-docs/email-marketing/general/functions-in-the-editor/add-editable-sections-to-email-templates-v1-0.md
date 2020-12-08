---
unique-page-id: 1900585
description: Lägg till redigerbara avsnitt i e-postmallar v1.0 - Marketo Docs - Produktdokumentation
title: Lägg till redigerbara avsnitt i e-postmallar v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Lägg till redigerbara avsnitt i e-postmallar v1.0 {#add-editable-sections-to-email-templates-v1.0}

Om du skapar en mall i e-postmallsredigeraren v1.0 kan du göra alla avsnitt redigerbara genom att placera en särskild mall `<div>` runt dem.

>[!NOTE]
>
>**Exempel**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regler:

1. HTML-koden måste alltid vara giltig.
1. Klassen för **mktEditable** måste inkluderas.
1. ID:t måste vara unikt i den HTML-koden.
1. Inga blanksteg i ID:t.

>[!CAUTION]
>
>mktEditable-satser kan inte kapslas.

Om du vill veta hur du gör detta i e-postmallsredigeraren v2.0 kan du ta en titt på [e-postmallens syntax](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
