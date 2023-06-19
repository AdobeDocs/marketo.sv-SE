---
description: Varför fylls inte mina dynamiska fält ut? - Marketo Docs - produktdokumentation
title: Varför fylls inte mina dynamiska fält ut?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Varför fylls inte mina dynamiska fält ut? {#why-arent-my-dynamic-fields-filling-out}

Dynamiska fält fungerar bara när du använder en mall. Enskilda e-postmeddelanden som du skriver fyller inte i dessa.

## Vad som ska kontrolleras {#what-to-check}

Det finns tre typer av dynamiska fält i Sales Insight Actions: Basic, Custom och Salesforce. Grundläggande och Anpassad ser båda ut att hämta information från [webbprogram](https://toutapp.com/login){target="_blank"}. If the information does not exist in the web application, the fields will be blank. Salesforce fields pull information from [Salesforce.com](https://salesforce.com){target="_blank"}.

**Felsöka Salesforce-fält**

Salesforce-fält: t.ex. `{{sfdc_account_name}}`

* Se till att den är korrekt ansluten med Sales Insight Actions. Gå till [Inställningar](https://toutapp.com/login{target="_blank"} sida och klicka **Hantera** bredvid din CRM.

**Felsöka grundläggande och anpassade fält**

Marketo Sales Insight Actions Basic Fields: t.ex. `{{company}}`

Anpassade fält för Marketo Sales Insight-åtgärder: t.ex. `{{custom_field_favorite_movie}}`

* Motsvarande fält måste sparas för din kontakt i [Personsida](https://toutapp.com/next#relationships){target="_blank"} för att hänvisa till vårt dynamiska fält. Om du till exempel skickar ett e-postmeddelande till Mary och använder `{{company}}` men hennes kontaktpost inte listar ett företag, vi kan inte fylla i det.

## Varför skickade mitt e-postmeddelande utan att fylla i alla dynamiska fält? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Insight Actions förhindrar att e-postmeddelanden skickas ut om vi inte kan fylla i alla dynamiska fält i e-postmeddelandet. **Men**, finns det några undantag från den här regeln. Vissa fält skickas ut tomma eller fyller i ett värde automatiskt om vi kan hitta ett. Dessa fält och hur de kommer att reagera om de inte kan fylla i fältet visas nedan.

`{{first_name}}` = TOM

`{{last_name}}` =TOM

`{{title}}` = TOM

`{{company}}` = &quot;ditt företag&quot;

`{{friendly_company}}` = &quot;ditt företag&quot;

>[!NOTE]
>
>The `{{first_name}}` ska det finnas både Sales Insight Actions och Salesforce för att försöka hämta information. Alla andra fält i den här listan söker bara i Sales Insight Actions för att fylla i fältet.
