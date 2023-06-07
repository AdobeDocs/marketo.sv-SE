---
description: Varför fylls inte mina dynamiska fält i - Marketo Docs - produktdokumentation
title: Varför fylls inte mina dynamiska fält ut?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: b4773137bf21eccc58a6d975d50748e8ff2a57db
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Varför fylls inte mina dynamiska fält ut? {#why-arent-my-dynamic-fields-filling-out}

Dynamiska fält fungerar bara när du använder en mall. Enskilda e-postmeddelanden som du skriver fyller inte i dessa.

## Vad som ska kontrolleras {#what-to-check}

Det finns tre typer av dynamiska fält i Sales Insight Actions: Basic, Custom och Salesforce. Grundläggande och Anpassad ser båda ut att hämta information från [webbprogram](https://toutapp.com/login). Om informationen inte finns i webbprogrammet är fälten tomma. Salesforce-fält hämtar information från [Salesforce.com](https://salesforce.com).

**Felsöka Salesforce-fält**

Salesforce-fält: t.ex. `{{sfdc_account_name}}`

* Se till att den är korrekt ansluten med Sales Insight Actions. Gå till [Inställningar](https://toutapp.com/login) sida och klicka **Hantera** bredvid din CRM.

**Felsöka grundläggande och anpassade fält**

Marketo Sales Insight Actions Basic Fields: t.ex. `{{company}}`

Anpassade fält för Marketo Sales Insight-åtgärder: t.ex. `{{custom_field_favorite_movie}}`

* Motsvarande fält måste sparas för din kontakt i [Personsida](https://toutapp.com/next#relationships) för att hänvisa till vårt dynamiska fält. Om du till exempel skickar ett e-postmeddelande till Mary och använder `{{company}}` men hennes kontaktpost inte listar ett företag, vi kan inte fylla i det.

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
