---
unique-page-id: 14352508
description: Skapa anpassade dynamiska fält - Marketo Docs - produktdokumentation
title: Skapa anpassade dynamiska fält
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Skapa anpassade dynamiska fält {#create-custom-dynamic-fields}

Det finns två sätt att skapa anpassade dynamiska fält.

## Spara anpassade fält för en eller några kontakter {#saving-custom-fields-for-one-or-a-few-contacts}

1. Klicka på namnet på en kontakt på sidan Personer.

1. Välj listrutan intill Avbeställ och välj **Redigera**.

1. Rulla ned till redigeringssidans nedre del. Du kan sedan skapa ett namn och ett värde för fältet.

1. Klicka **Spara**.

## Spara anpassade fält för många kontakter {#saving-custom-fields-for-many-contacts}

1. Skapa ett CSV-kalkylblad med dina anpassade fält i en egen kolumn.

1. Följ [normal CSV-överföringsprocess](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), stoppas på fältmappningsskärmen.

1. I stället för något av de förinställda fälten väljer du **Lägg till ett nytt anpassat fält** i listrutan.

1. Ange det önskade fältnamnet och klicka på **OK**.

1. Slutför överföringen av CSV-filen. Dina kontakter visas med det nya anpassade fältet.

>[!NOTE]
>
>När du har skapat ett anpassat fält kan det ta ca 30 minuter innan fältet visas i listrutan för dynamiska fält i mallredigeraren.

## Så här använder du anpassade fält i en mall {#how-to-use-your-custom-fields-in-a-template}

När dina anpassade fält har lagrats med ovanstående metoder kan du referera till dem i dina mallar.

1. [Skapa en mall](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) och klicka på **Dynamiska fält** som vanligt.

1. Välj **Anpassade fält** i listrutan som visas.

1. Du ser dina förlagrade anpassade fält och kan välja vilka som ska fyllas i i mallen.
