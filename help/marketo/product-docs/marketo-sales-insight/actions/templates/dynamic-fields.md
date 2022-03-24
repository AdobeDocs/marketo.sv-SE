---
description: Dynamiska fält - Marketo Docs - produktdokumentation
title: Dynamiska fält
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Dynamiska fält {#dynamic-fields}

Vi låter dig anpassa dina e-postmallar med fördefinierade attribut som `{{first_name}}` eller `{{company}}`. Dessa fält gör att du kan skicka e-post till flera kontakter och fylla i fälten automatiskt utan att behöva skriva ut dem separat för varje kontakt.

>[!TIP]
>
>Fälten&quot;first_name&quot; och&quot;company&quot; är de enda fält som kommer att användas för både Sales Insight Actions och Salesforce. Det innebär att en kontakt inte finns i [webbprogram](https://toutapp.com/login)söker vi i Salesforce för att se om vi kan hitta en kontakt-/lead-post med en matchande e-postadress. Vi använder sedan information från den posten för att fylla i fältet.

## Infoga ett dynamiskt fält i en mall {#insert-a-dynamic-field-into-a-template}

1. I **Mallar och kampanjer** söker du efter den mall som du vill redigera och klickar på **Redigera mall**.

1. Klicka **Infoga dynamiskt fält**.

   >[!NOTE]
   >
   >När du skickar e-postkontakter som finns i Sales Insight-åtgärder kan du använda de grundläggande dynamiska fälten. De här kommer att dras direkt från kontakten.

Om du skickar e-post till kontakter som finns i Salesforce kan du dra nytta av de dynamiska fälten i Salesforce. De här börjar alla med &quot;sfdc&quot;. Så länge du har en anslutning till Salesforce kommer dessa fält att anropa direkt till leadet/kontakten i Salesforce för att fylla i information i mallen.

## Infoga dynamiska fält i en ämnesrad {#insert-dynamic-fields-in-a-subject-line}

Kopiera dem manuellt och klistra in dem i ämnesfältet i ett e-postmeddelande. Se till att du har rätt formatering.

## Ordlista för dynamiska fält {#dynamic-fields-glossary}

När du skapar en mall i Sales Insight Actions rekommenderar vi alltid att du integrerar dynamiska fält med **Infoga dynamiskt fält** -knappen.

Det här verktyget används för att `auto-personalize your email` och spara massor av tid `pulling information from the People page`.

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
* Skillnaden mellan `{{company}}` och `{{company_friendly}}` är `{{company_friendly}}` tar bort alla formella titlar, som Inc., LLC. osv., från namnet på din kontakts företag.
* När du använder `{{company_friendly}}`ska du avgränsa Inc. eller Co. med ett kommatecken i kontaktinformationen. Så här vet Sales Insight Actions vad som ska tas bort när värdet hämtas.
* Vi låter dig anpassa dina e-postmallar med fördefinierade attribut som `{{my_name}}` eller `{{my_title}}`. Med dessa fält kan du snabbt referera till dig själv i e-postmallar.

>[!TIP]
>
>Om dina dynamiska fält inte fylls i, checka ut [den här artikeln](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
