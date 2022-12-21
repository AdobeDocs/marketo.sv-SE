---
unique-page-id: 10095554
description: Bädda in ett formulär i en webbkampanj - Marketo Docs - produktdokumentation
title: Bädda in ett formulär i en webbkampanj
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Bädda in ett formulär i en webbkampanj {#embed-a-form-into-a-web-campaign}

Se hur du kan bädda in ett Marketo-formulär i en webbkampanj (Dialog, In Zone eller Widget).

1. Högerklicka på ett godkänt formulär. Välj **Bädda in kod**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Kopiera koden.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Gå till Webbanpassning **Webbkampanjer**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Klicka **Skapa ny kampanj**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Klicka på ikonen HTML i textredigeraren.

   ![](assets/five-1.png)

1. Klistra in formulärinbäddningskoden i HTML källredigeraren. Klicka **Uppdatera**.

   ![](assets/six-1.png)

1. Formuläret visas inte i redigeringsvyn, men du kan förhandsgranska det för att se hur det kommer att visas i en kampanj.

1. Klicka **Starta** för att starta kampanjen.

   >[!NOTE]
   >
   >Ändringar i formulärfälten måste göras i Marketo marknadsföringsaktiviteter i Redigera utkast till formuläret.

## Tre sätt att lägga till en bakgrundsbild i ett formulär {#three-ways-to-add-a-background-image-to-a-form}

Om du vill lägga till en bakgrundsbild i formuläret kan du:

* Redigera CSS för ett formulärtema
* Ändra dialogrute- eller widgetfärger i Ange kampanj
* Lägg till CSS-kod i skriptet

Information om hur du redigerar CSS för ett formulärtema finns i [den här artikeln](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Så här ändrar du dialogrute- eller widgetfärger i Ange kampanj:

1. Välj en kampanjtyp för dialog och en dialogstil, rubrikfärg och bakgrundsfärg i Rich Text Editor för att anpassa formulärets bakgrundsfärger. Klicka **Spara**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Här är ett exempel på hur en dialogstil för modern trimning ser ut med en ljuslila rubrik- och bakgrundsfärg.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Så här lägger du till CSS-kod i skriptet:

1. Klicka på ikonen HTML i textredigeraren.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Klistra in formulärinbäddningskoden med bakgrundsformatkoden i källredigeraren i HTML. Klicka **Uppdatera**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Klicka **Förhandsgranska** för att se hur det kommer att återges i en kampanj (formuläret visas inte i redigeringsvyn). Här är ett exempel på hur formulärkoden ovan återges i en kampanj med en bakgrundsbild.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Redigera CSS för ett formulärtema](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Visa tackmeddelande utan en uppföljningsstartsida](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://developers.marketo.com/documentation/websites/forms-2-0/)

