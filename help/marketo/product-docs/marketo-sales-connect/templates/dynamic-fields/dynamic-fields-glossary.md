---
unique-page-id: 14352509
description: Dynamiska fält - ordlista - Marketo Docs - produktdokumentation
title: Ordlista för dynamiska fält
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Ordlista för dynamiska fält {#dynamic-fields-glossary}

När du skapar en mall i Sales Connect rekommenderar vi alltid att du integrerar dynamiska fält med knappen **MSE Dynamic Fields**.

Det här verktyget används för att `auto-personalize your email` och spara massor av tid med `pulling information from the People page`.

| Dynamiskt fält | Exempel på vad som visas i ditt e-postmeddelande |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Om du inte vill höra av mig igen, var snäll och säg till här |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Teknikskribent |
| `{{work_website}}` | https://www.marketo.com |

**Saker att notera**:

* Om en kontakts information är felaktigt angiven eller saknas på sidan Personer, kommer den inte att läggas in korrekt i mallen.
* Skillnaden mellan `{{company}}` och `{{company_friendly}}` är att `{{company_friendly}}` kommer att ta bort all formell titel, som Inc., LLC. osv., från namnet på din kontakts företag.
* När du använder `{{company_friendly}}` måste du separera Inc. eller Co. med ett kommatecken i kontaktinformationen. Så här vet Sales Connect vad som ska tas bort när värdet hämtas.

>[!TIP]
>
>Du kan skapa ett eget [anpassat dynamiskt fält](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) för allt du vill ha automatiskt i dina e-postmeddelanden
