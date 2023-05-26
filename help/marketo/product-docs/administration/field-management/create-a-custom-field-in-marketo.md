---
unique-page-id: 2360287
description: Skapa ett anpassat fält i Marketo - Marketo Docs - produktdokumentation
title: Skapa ett anpassat fält i Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 1%

---

# Skapa ett anpassat fält i Marketo {#create-a-custom-field-in-marketo}

Om du behöver ett nytt anpassat fält i Marketo Engage för att lagra/hämta in data, så här skapar du ett.

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >Om du vill att fälten ska synkroniseras med CRM skapar du dem i CRM så skapas de automatiskt i Marketo.

1. Klicka på **[!UICONTROL New Custom Field]**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. Välj fälttyp. Detta ändrar hur det återges i smarta listor och formulär i Marketo.

   >[!TIP]
   >
   >Kolla in [Ordlista för anpassade fälttyper](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/create-a-custom-field-in-marketo-4.png)

1. Ange [!UICONTROL Name] som du vill att den ska visas i Marketo. The [!UICONTROL API Name] genereras automatiskt. Du kan ändra den, men du kan inte byta namn på den när den har angetts. Klicka **[!UICONTROL Create]** när det är klart.

>[!CAUTION]
>
>Fältnamn får inte börja med följande tecken: **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-5.png)

>[!NOTE]
>
>API-namnet används av SOAP API och andra serverdelsprocesser.

Nu kan du använda det här anpassade fältet i formulär, flödessteg och smarta listor!
