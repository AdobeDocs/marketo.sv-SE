---
unique-page-id: 14352592
description: Infoga dynamiska fält - Marketo Docs - Produktdokumentation
title: Infoga dynamiska fält
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Infoga dynamiska fält {#how-to-insert-dynamic-fields}

Vi låter dig anpassa dina e-postmallar med fördefinierade attribut som `{{first_name}}` eller `{{company}}`. Dessa fält gör att du kan skicka e-post till flera kontakter och fylla i fälten automatiskt utan att behöva skriva ut dem separat för varje kontakt.

>[!TIP]
>
>Fälten&quot;first_name&quot; och&quot;company&quot; är `only fields that will look to both Sales Connect and Salesforce.` &quot;Det innebär att om en kontakt inte finns i [webbprogrammet](http://toutapp.com/login), söker vi i Salesforce för att se om vi kan hitta en kontakt-/lead-post med en matchande e-postadress. Vi använder sedan information från den posten för att fylla i fältet.

## Infoga ett dynamiskt fält i en mall {#insert-a-dynamic-field-into-a-template}

1. I **Mallar och kampanjer** letar du reda på mallen som du vill redigera och klickar på **Redigera mall**.
1. Klicka på **Tout Dynamic Fields**.

   >[!NOTE]
   >
   >När du skickar e-postkontakter som finns i Sales Connect kan du använda de grundläggande dynamiska fälten. De här kommer att dras direkt från kontakten.

Om du skickar e-post till kontakter som finns i Salesforce kan du dra nytta av de dynamiska fälten i Salesforce. De här börjar alla med &quot;sfdc&quot;. Så länge du har en anslutning till Salesforce kommer dessa fält att anropa direkt till leadet/kontakten i Salesforce för att fylla i information i mallen.

## Infoga dynamiska fält i en ämnesrad {#insert-dynamic-fields-in-a-subject-line}

Kopiera dem manuellt och klistra in dem i ämnesfältet i ett e-postmeddelande. Se till att du har rätt formatering.
