---
unique-page-id: 2360287
description: Skapa ett anpassat fält i Marketo - Marketo Docs - produktdokumentation
title: Skapa ett anpassat fält i Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Skapa ett anpassat fält i Marketo {#create-a-custom-field-in-marketo}

Så här skapar du ett nytt anpassat fält i Marketo för att lagra/hämta in data.

1. Gå till Admin och klicka på **Fälthantering**.

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >Om du vill att fälten ska synkroniseras med CRM skapar du dem i CRM så skapas de automatiskt i Marketo.

1. Klicka på **Nytt anpassat fält**.

   ![](assets/two.png)

1. Välj fälttyp. Detta ändrar hur det återges i smarta listor och formulär i Marketo.

   >[!TIP]
   >
   >Ta en titt på ordlistan [Egna fälttyper](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. Ange namnet som du vill att det ska visas i Marketo. API-namnet genereras automatiskt. Du kan ändra den, men du kan inte byta namn på den när den har angetts. Klicka på **Skapa** när du är klar.

>[!CAUTION]
>
>Fältnamn får inte börja med följande tecken: **. &amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>API-namnet används av SOAP API och andra serverdelsprocesser.

Du kan nu använda det här anpassade fältet i formulär, flödessteg och smarta listor.
