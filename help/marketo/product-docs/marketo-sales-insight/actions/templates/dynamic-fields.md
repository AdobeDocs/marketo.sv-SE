---
description: Dynamiska fält - Marketo Docs - produktdokumentation
title: Dynamiska fält
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Dynamiska fält {#dynamic-fields}

Du kan anpassa dina e-postmallar med fördefinierade attribut som `{{first_name}}` eller `{{company}}`. Dessa fält gör att du kan skicka e-post till flera kontakter och fylla i fälten automatiskt utan att behöva skriva ut dem separat för varje kontakt.

>[!TIP]
>
>Fälten&quot;first_name&quot; och&quot;company&quot; är de enda fälten som kommer att användas för både [!DNL Sales Insight Actions] och [!DNL Salesforce]. Det innebär att om det inte finns någon kontakt i [webbprogrammet](https://toutapp.com/login), söker vi i [!DNL Salesforce] för att se om det går att hitta en kontakt-/lead-post med en matchande e-postadress. Vi använder sedan information från den posten för att fylla i fältet.

## Infoga ett dynamiskt fält i en mall {#insert-a-dynamic-field-into-a-template}

1. I **[!UICONTROL Templates & Campaigns]** letar du reda på mallen som du vill redigera och klickar på **[!UICONTROL Edit Template]**.

1. Klicka på **[!UICONTROL Insert Dynamic Field]**.

   >[!NOTE]
   >
   >När du skickar e-post till kontakter som finns i [!DNL Sales Insight Actions] kan du använda de grundläggande dynamiska fälten. De här kommer att dras direkt från kontakten.

Om du skickar e-post till kontakter som finns i [!DNL Salesforce] kan du dra nytta av de dynamiska fälten i [!DNL Salesforce]. De här börjar alla med &quot;sfdc&quot;. Så länge du har en anslutning till [!DNL Salesforce] anropar de här fälten direkt till lead/kontakt i [!DNL Salesforce] för att fylla i information i mallen.

## Infoga dynamiska fält i en ämnesrad {#insert-dynamic-fields-in-a-subject-line}

Kopiera dem manuellt och klistra in dem i ämnesfältet i ett e-postmeddelande. Se till att du har rätt formatering.

## Standardvärden för dynamiskt fält {#dynamic-field-default-values}

När du lägger till dynamiska fält i e-postmallar kan du lägga till ett standardvärde som det dynamiska fältet kommer att resultera i om det inte finns något annat värde tillgängligt.

Det gör du genom att lägga till &quot;|&quot; efter etiketten för det dynamiska fältet och sedan lägga till &quot;default:&quot; (båda utan citattecken). Lägg sedan till värdet som du vill att fältet ska matchas till (omslutna med citattecken) om inget annat värde hittas.

**Exempel:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Ordlista för dynamiska fält {#dynamic-fields-glossary}

När du skapar en mall i [!DNL Sales Insight Actions] rekommenderar vi alltid att du integrerar dynamiska fält med knappen **[!UICONTROL Insert Dynamic Field]** .

Det här verktyget används för att `auto-personalize your email` och sparar dig massor av tid av `pulling information from the People page`.

| Dynamiskt fält | Exempel på vad som visas i ditt e-postmeddelande |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Om du inte längre vill få e-post från oss klickar du här |
| `{{friendly_unsubscribe}}` | Trött på alla e-postmeddelanden? Meddela mig här |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Teknikskribent |
| `{{work_website}}` | https://www.adobe.com |

**Saker att notera**:

* Om en kontakts information är felaktigt angiven eller saknas på sidan Personer, kommer den inte att föras över korrekt till din mall.
* Skillnaden mellan `{{company}}` och `{{company_friendly}}` är att `{{company_friendly}}` kommer att ta bort alla formella titlar, som Inc., LLC osv., från namnet på din kontakts företag.
* När du använder `{{company_friendly}}` måste du separera Inc. eller Co. med ett kommatecken i kontaktinformationen. Så här vet [!DNL Sales Insight Actions] vad som ska tas bort när värdet dras in.
* Du kan anpassa dina e-postmallar med fördefinierade attribut som `{{my_name}}` eller `{{my_title}}`. Med dessa fält kan du snabbt referera till dig själv i e-postmallar.
* Systemet lägger automatiskt till användarens signatur i varje e-postmeddelande som skickas. Om användaren använder en mall med det `{{my_signature}}` dynamiska fältet fyller systemet i signaturen där det `{{my_signature}}` dynamiska fältet har placerats. Det läggs bara till där för att undvika duplicering. Systemet hanterar `{{team_unsubscribe}}` på samma sätt när den globala inställningen för att avsluta prenumerationen är aktiverad.

>[!TIP]
>
>Om dina dynamiska fält inte fylls i går du till [den här artikeln](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
