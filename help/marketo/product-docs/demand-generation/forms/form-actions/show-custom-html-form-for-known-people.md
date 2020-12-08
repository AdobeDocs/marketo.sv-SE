---
unique-page-id: 2359644
description: Visa anpassat HTML-formulär för kända personer - Marketo-dokument - Produktdokumentation
title: Visa anpassat HTML-formulär för kända personer
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Visa anpassat HTML-formulär för kända personer {#show-custom-html-form-for-known-people}

Om en besökare är cookie (en känd person som tidigare har angett en e-postadress), varför behöver du då bekymra dig om formuläret? Ge dem bara nedladdningsknappen. Så här gör du.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. Gå till **Marknadsföringsaktiviteter** och **aktiviteter**.

   ![](assets/login-marketing-activities-5.png)

1. Under **Marknadsföringsaktiviteter** **väljer du formuläret och klickar på** Redigera **** formulär ****.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Klicka på **Inställningar** under **Formulärinställningar******.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Ange om **du känner** till **besökare, visa**: till **anpassad** **HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Klicka på ![—](assets/image2014-9-25-14-3a1-3a26.png) för att redigera den **anpassade** **HTML** som ska visas för kända personer.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Det finns visst standardinnehåll, men du kan ändra det.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tillgängliga tokens:

   | Token | Beskrivning |
   |---|---|
   | `{{lead.FirstName}}` | Då visas personens förnamn. |
   | `{{lead.LastName}}` | Då visas personens efternamn. |
   | `{{form.Button:default=Download}}` | Då visas formulärknappen. Ersätt området efter `=` knappen för att ändra knapptexten. |
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
   >**Påminnelse**
   >
   >
   >Kom ihåg att [godkänna landningssidans utkast](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) som har skapats av formulärändringarna.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Du kan dirigera klickningen på knappen till resursen genom att ställa in formuläruppföljningssidan till filens URL.

Kakbit! Ta en titt på vad en person skulle se om de kom tillbaka till samma form: