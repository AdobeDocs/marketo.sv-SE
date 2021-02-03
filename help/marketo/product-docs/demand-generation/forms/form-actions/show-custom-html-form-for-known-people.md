---
unique-page-id: 2359644
description: Visa anpassat HTML-formulär för kända personer - Marketo-dokument - Produktdokumentation
title: Visa anpassat HTML-formulär för kända personer
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Visa anpassat HTML-formulär för kända personer {#show-custom-html-form-for-known-people}

Om en besökare är cookie (en känd person som tidigare har angett en e-postadress), varför behöver du då bekymra dig om formuläret? Ge dem bara nedladdningsknappen. Så här gör du.

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-5.png)

1. Under **Marknadsföringsaktiviteter** markerar du formuläret och klickar på **Redigera formulär**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Klicka på **Inställningar** under **Formulärinställningar**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Ange om **Känd besökare, visa**: till **Anpassad HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Klicka på ![—](assets/image2014-9-25-14-3a1-3a26.png) för att redigera den **anpassade HTML** som ska visas för kända personer.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Det finns visst standardinnehåll, men du kan ändra det.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tillgängliga tokens:

   | Token | Beskrivning |
   |---|---|
   | `{{lead.FirstName}}` | Då visas personens förnamn. |
   | `{{lead.LastName}}` | Då visas personens efternamn. |
   | `{{form.Button:default=Download}}` | Då visas formulärknappen. Ersätt området efter `=` om du vill ändra knapptexten. |
   | `{{form.NotYou:default=Not you?}}` | Då visas en länk om personen är någon annan. Ersätt området efter `=` för att ändra länktexten. |

   >[!CAUTION]
   >
   >Endast de fyra variablerna ovan kan användas. Alla andra token fungerar inte här.

1. Klicka på **Slutför**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Klicka på **Godkänn och stäng**.

   >[!NOTE]
   >
   >Formuläret ska vara godkänt för användning på landningssidor.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Kom ihåg att [godkänna landningssidans utkast](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) som skapats av formulärändringarna.

   Kakbit! Ta en titt på vad en person skulle se om de kom tillbaka till samma form:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Du kan dirigera klickningen på knappen till resursen genom att ställa in formuläruppföljningssidan till filens URL.
