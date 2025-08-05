---
description: Varför fylls inte mina dynamiska fält ut? - Marketo Docs - produktdokumentation
title: Varför fylls inte mina dynamiska fält ut?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Varför fylls inte mina dynamiska fält ut? {#why-arent-my-dynamic-fields-filling-out}

Dynamiska fält fungerar bara när du använder en mall. Enskilda e-postmeddelanden som du skriver fyller inte i dessa.

## Vad som ska kontrolleras {#what-to-check}

Det finns tre typer av dynamiska fält i Sales Insight Actions: Basic, Custom och Salesforce. Grundläggande och Anpassad ser båda ut att hämta information från [webbprogrammet](https://toutapp.com/login){target="_blank"}. Om informationen inte finns i webbprogrammet är fälten tomma. Salesforce-fält hämtar information från [Salesforce.com](https://salesforce.com){target="_blank"}.

**Felsökning av [!DNL Salesforce] fält**

[!DNL Salesforce] fält: t.ex. `{{sfdc_account_name}}`

* Se till att den är korrekt ansluten med Sales Insight Actions. Gå till sidan [Inställningar]&#x200B;(<https://toutapp.com/login{target="_blank"}> och klicka på **Hantera** bredvid CRM.

**Felsökning av grundläggande och anpassade fält**

Marketo Sales Insight Actions Basic Fields: e.g., `{{company}}`

Anpassade fält för Marketo Sales Insight-åtgärder: t.ex. `{{custom_field_favorite_movie}}`

* Motsvarande fält måste sparas för din kontakt på sidan [Personer](https://toutapp.com/next#relationships){target="_blank"} för att det dynamiska fältet ska referera till. Om du till exempel skickar ett e-postmeddelande till Mary och använder fältet `{{company}}`, men hennes kontaktpost inte listar något företag, kommer vi inte att kunna fylla i det.

## Varför skickade mitt e-postmeddelande utan att fylla i alla dynamiska fält? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Insight Actions] kommer att hindra att dina e-postmeddelanden skickas ut om vi inte kan fylla i alla dynamiska fält i e-postmeddelandet. **Men**, det finns några undantag för den här regeln. Vissa fält skickas ut tomma eller fyller i ett värde automatiskt om vi kan hitta ett. Dessa fält och hur de kommer att reagera om de inte kan fylla i fältet visas nedan.

`{{first_name}}` = TOMT

`{{last_name}}` =TOM

`{{title}}` = TOMT

`{{company}}` = &quot;ditt företag&quot;

`{{friendly_company}}` = &quot;ditt företag&quot;

>[!NOTE]
>
>Fältet `{{first_name}}` kommer att söka i både [!DNL Sales Insight Actions] och [!DNL Salesforce] för att försöka hämta information. Alla andra fält i den här listan söker bara i [!DNL Sales Insight Actions] för att fylla i fältet.
