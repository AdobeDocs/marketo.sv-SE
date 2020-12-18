---
unique-page-id: 14352602
description: Mina dynamiska fält fylls inte i - Marketo Docs - Produktdokumentation
title: Mina dynamiska fält fylls inte ut
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Mina dynamiska fält fylls inte ut {#my-dynamic-fields-arent-filling-out}

Dynamiska fält fungerar bara när du använder en mall. Enskilda e-postmeddelanden som du skriver fyller inte i dessa.

## Vad som ska kontrolleras {#what-to-check}

Det finns tre typer av dynamiska fält i Sales Connect: Basic, Custom och Salesforce. Grundläggande och Anpassad söker båda efter information från [webbprogrammet](http://toutapp.com/login). Om informationen inte finns i webbprogrammet är fälten tomma. Salesforce-fält hämtar information från [Salesforce.com](http://salesforce.com).

`**Troubleshooting Salesforce Fields**`

Salesforce-fält: t.ex. `{{sfdc_account_name}}`

* Se till att den är rätt ansluten med Sales Connect. Gå till sidan [Inställningar](http://toutapp.com/next#settings) och klicka på **Hantera** bredvid CRM.

**Felsöka grundläggande och anpassade fält**

Grundläggande flikar: t.ex. `{{company}}`

Visa anpassade fält: t.ex. `{{custom_field_favorite_movie}}`

* T `he corresponding field needs to be saved for your contact` på sidan [Personer](http://toutapp.com/next#relationships) för att referera till vårt dynamiska fält. Om du till exempel skickar ett e-postmeddelande till Mary och använder fältet `{{company}}`, men hennes kontaktpost inte listar något företag, kommer vi inte att kunna fylla i det.

## Varför skickade mitt e-postmeddelande utan att fylla i alla dynamiska fält? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect kommer att hindra att dina e-postmeddelanden skickas ut om vi inte kan fylla i alla dynamiska fält i e-postmeddelandet. **Det finns dock** några undantag från den här regeln. Vissa fält skickas ut tomma eller fyller i ett värde automatiskt om vi kan hitta ett. Dessa fält och hur de kommer att reagera om de inte kan fylla i fältet visas nedan.

`{{first_name}}` = TOM

`{{last_name}}` =TOM

`{{title}}` = TOM

`{{company}}` = &quot;ditt företag&quot;

`{{friendly_company}}` = &quot;ditt företag&quot;

>[!NOTE]
>
>Fältet `{{first_name}}` kommer att finnas i både Sales Connect och Salesforce för att försöka hämta information. Alla andra fält i den här listan söker bara i Sales Connect för att fylla i fältet.

