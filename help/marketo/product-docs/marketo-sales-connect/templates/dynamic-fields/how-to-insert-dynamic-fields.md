---
unique-page-id: 14352592
description: Infoga dynamiska fält - Marketo Docs - produktdokumentation
title: Infoga dynamiska fält
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Infoga dynamiska fält {#how-to-insert-dynamic-fields}

Du kan anpassa dina e-postmallar med fördefinierade attribut som `{{first_name}}` eller `{{company}}`. Dessa fält gör att du kan skicka e-post till flera kontakter och fylla i fälten automatiskt utan att behöva skriva ut dem separat för varje kontakt.

>[!TIP]
>
>Fälten&quot;first_name&quot; och&quot;company&quot; är de enda fälten som kommer att användas för både [!DNL Sales Connect] och [!DNL Salesforce]. Det innebär att om det inte finns någon kontakt i [webbprogrammet](https://toutapp.com/login), söker vi i [!DNL Salesforce] för att se om det går att hitta en kontakt-/lead-post med en matchande e-postadress. Vi använder sedan information från den posten för att fylla i fältet.

## Infoga ett dynamiskt fält i en mall {#insert-a-dynamic-field-into-a-template}

1. I **[!UICONTROL Templates & Campaigns]** letar du reda på mallen som du vill redigera och klickar på **[!UICONTROL Edit Template]**.

1. Klicka på **[!UICONTROL Tout Dynamic Fields]**.

   >[!NOTE]
   >
   >När du skickar e-post till kontakter som finns i [!DNL Sales Connect] kan du använda de grundläggande dynamiska fälten. De här kommer att dras direkt från kontakten.

Om du skickar e-post till kontakter som finns i [!DNL Salesforce] kan du dra nytta av de dynamiska fälten i [!DNL Salesforce]. De här börjar alla med &quot;sfdc&quot;. Så länge du har en anslutning till [!DNL Salesforce] anropar de här fälten direkt till lead/kontakt i [!DNL Salesforce] för att fylla i information i mallen.

## Infoga dynamiska fält i en ämnesrad {#insert-dynamic-fields-in-a-subject-line}

Kopiera dem manuellt och klistra in dem i ämnesfältet i ett e-postmeddelande. Se till att du har rätt formatering.
