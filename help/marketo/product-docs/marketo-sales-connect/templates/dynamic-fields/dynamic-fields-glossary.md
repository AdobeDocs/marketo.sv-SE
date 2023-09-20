---
unique-page-id: 14352509
description: Dynamiska fält - ordlista - Marketo Docs - produktdokumentation
title: Ordlista för dynamiska fält
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Ordlista för dynamiska fält {#dynamic-fields-glossary}

När du skapar en mall i Sales Connect rekommenderar vi alltid att du integrerar dynamiska fält med **MSE Dynamic Fields** -knappen.

Det här verktyget används för att `auto-personalize your email` och spara massor av tid `pulling information from the People page`.

| Dynamiskt fält | Exempel på vad som visas i ditt e-postmeddelande |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Om du inte vill höra av mig igen, var snäll och säg till här |
| `{{my_name}}` | Keith Flynn |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Teknikskribent |
| `{{work_website}}` | https://www.adobe.com |

**Saker att notera**:

* Om en kontakts information är felaktigt angiven eller saknas på sidan Personer, kommer den inte att föras över korrekt till din mall.
* Skillnaden mellan `{{company}}` och `{{company_friendly}}` är att `{{company_friendly}}` tar bort alla formella titlar, som Inc., LLC. osv., från namnet på din kontakts företag.
* När du använder `{{company_friendly}}`ska du avgränsa Inc. eller Co. med ett kommatecken i kontaktinformationen. Så här vet Sales Connect vad som ska tas bort när värdet hämtas.

>[!TIP]
>
>Du kan skapa en egen [anpassat dynamiskt fält](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) för allt du vill ha i mejlen automatiskt
