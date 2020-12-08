---
unique-page-id: 14352509
description: Dynamiska fält - ordlista - Marketo Docs - produktdokumentation
title: Ordlista för dynamiska fält
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---


# Ordlista för dynamiska fält {#dynamic-fields-glossary}

När du skapar en mall i Sales Connect rekommenderar vi alltid att du integrerar dynamiska fält med knappen **MSE Dynamic Fields** .

Det här verktyget används för att `auto-personalize your email` spara massor av tid i `pulling information from the People page`taget.

| Dynamiskt fält | Exempel på vad som visas i ditt e-postmeddelande |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Om du inte vill höra av mig igen, var snäll och säg till här |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | [[e-postskyddad]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Teknikskribent |
| `{{work_website}}` | https://www.marketo.com |

**Saker att notera**:

* Om en kontakts `information is entered incorrectly` eller saknas på sidan Personer, läggs den `will not pull over correctly` in i din mall.

* Skillnaden mellan `{{company}}` och `{{company_friendly}}` är att `{{company_friendly}}` kommer `remove any formal title`, som Inc., LLC. osv., från namnet på din kontakts företag.
* När du använder `{{company_friendly}}`måste du separera Inc. eller Co. med ett kommatecken i kontaktinformationen. Så här vet Sales Connect vad som ska tas bort när värdet hämtas.

>[!TIP]
>
>Du kan skapa ett eget [anpassat dynamiskt fält](http://docs.marketo.com/x/fADb) för allt du vill ha i dina e-postmeddelanden automatiskt

