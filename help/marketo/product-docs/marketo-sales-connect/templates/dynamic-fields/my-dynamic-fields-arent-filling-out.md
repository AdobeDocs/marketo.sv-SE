---
unique-page-id: 14352602
description: Mina dynamiska fält fylls inte i - Marketo Docs - produktdokumentation
title: Mina dynamiska fält fylls inte ut
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Mina dynamiska fält fylls inte ut {#my-dynamic-fields-arent-filling-out}

Dynamiska fält fungerar bara när du använder en mall. Enskilda e-postmeddelanden som du skriver fyller inte i dessa.

## Vad som ska kontrolleras {#what-to-check}

Det finns tre typer av dynamiska fält i [!DNL Sales Connect]: Basic, Custom och [!DNL Salesforce]. Grundläggande och Anpassad ser båda ut att hämta information från [webbprogrammet](https://toutapp.com/login). Om informationen inte finns i webbprogrammet är fälten tomma. [!DNL Salesforce] fält hämtar information från [Salesforce.com](https://salesforce.com).

**Felsökning av [!DNL Salesforce] fält**

[!DNL Salesforce] fält: t.ex. `{{sfdc_account_name}}`

* Kontrollera att den är korrekt ansluten med [!DNL Sales Connect]. Gå till sidan [Inställningar](https://toutapp.com/login) och klicka på **[!UICONTROL Manage]** bredvid CRM.

**Felsökning av grundläggande och anpassade fält**

Grundläggande flikar: t.ex. `{{company}}`

Tout-anpassade fält: t.ex. `{{custom_field_favorite_movie}}`

* Motsvarande fält måste sparas för din kontakt på sidan [Personer](https://toutapp.com/next#relationships) för att det dynamiska fältet ska referera till. Om du till exempel skickar ett e-postmeddelande till Mary och använder fältet `{{company}}`, men hennes kontaktpost inte listar något företag, kommer vi inte att kunna fylla i det.

## Varför skickade mitt e-postmeddelande utan att fylla i alla dynamiska fält? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Connect] kommer att hindra att dina e-postmeddelanden skickas ut om vi inte kan fylla i alla dynamiska fält i e-postmeddelandet. **Men**, det finns några undantag för den här regeln. Vissa fält skickas ut tomma eller fyller i ett värde automatiskt om vi kan hitta ett. Dessa fält och hur de kommer att reagera om de inte kan fylla i fältet visas nedan.

`{{first_name}}` = TOMT

`{{last_name}}` =TOM

`{{title}}` = TOMT

`{{company}}` = &quot;ditt företag&quot;

`{{friendly_company}}` = &quot;ditt företag&quot;

>[!NOTE]
>
>Fältet `{{first_name}}` kommer att söka i både [!DNL Sales Connect] och [!DNL Salesforce] för att försöka hämta information. Alla andra fält i den här listan söker bara i [!DNL Sales Connect] för att fylla i fältet.
