---
unique-page-id: 14352508
description: Skapa anpassade dynamiska fält - Marketo Docs - produktdokumentation
title: Skapa anpassade dynamiska fält
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Skapa anpassade dynamiska fält {#create-custom-dynamic-fields}

Det finns två sätt att skapa anpassade dynamiska fält.

## Spara anpassade fält för en eller några kontakter {#saving-custom-fields-for-one-or-a-few-contacts}

1. Klicka på namnet på en kontakt på sidan [!UICONTROL People].

1. Välj listrutan bredvid [!UICONTROL Unsubscribe] och välj **[!UICONTROL Edit]**.

1. Bläddra nedåt till redigeringssidans nederkant. Du kan sedan skapa ett namn och ett värde för fältet.

1. Klicka på **[!UICONTROL Save]**.

## Spara anpassade fält för många kontakter {#saving-custom-fields-for-many-contacts}

1. Skapa ett CSV-kalkylblad med dina anpassade fält i en egen kolumn.

1. Följ den [normala CSV-överföringsprocessen](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) och stoppa på fältmappningsskärmen.

1. Välj **[!UICONTROL Add a new Custom Field]** i listrutan i stället för ett av förinställningsfälten.

1. Ange önskat fältnamn och klicka på **[!UICONTROL OK]**.

1. Slutför överföringen av CSV-filen. Dina kontakter visas med det nya anpassade fältet.

>[!NOTE]
>
>När du har skapat ett anpassat fält kan det ta ca 30 minuter innan fältet visas i listrutan för dynamiska fält i mallredigeraren.

## Så här använder du anpassade fält i en mall {#how-to-use-your-custom-fields-in-a-template}

När dina anpassade fält har lagrats med ovanstående metoder kan du referera till dem i dina mallar.

1. [Skapa en mall](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) och klicka på knappen **[!UICONTROL Dynamic Fields]** som vanligt.

1. Välj **[!UICONTROL Custom Fields]** i listrutan som visas.

1. Du ser dina förlagrade anpassade fält och kan välja vilka som ska fyllas i i mallen.
