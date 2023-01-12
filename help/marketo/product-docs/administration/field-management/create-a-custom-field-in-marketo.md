---
unique-page-id: 2360287
description: Skapa ett anpassat fält i Marketo - Marketo Docs - produktdokumentation
title: Skapa ett anpassat fält i Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
source-git-commit: cd742b3c4ff464a7efeb6490b88fe78e6b3f4ae8
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Skapa ett anpassat fält i Marketo {#create-a-custom-field-in-marketo}

Så här skapar du ett nytt anpassat fält i Marketo för att lagra/hämta in data.

1. Gå till **Administratör** område.

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. Klicka **Fälthantering**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >Om du vill att fälten ska synkroniseras med CRM skapar du dem i CRM så skapas de automatiskt i Marketo.

1. Klicka **Nytt anpassat fält**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. Välj fälttyp. Detta ändrar hur det återges i smarta listor och formulär i Marketo.

   >[!TIP]
   >
   >Kolla in [Ordlista för anpassade fälttyper](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/create-a-custom-field-in-marketo-4.png)

1. Ange namnet som du vill att det ska visas i Marketo. API-namnet genereras automatiskt. Du kan ändra den, men du kan inte byta namn på den när den har angetts. Klicka **Skapa** när det är klart.

>[!CAUTION]
>
>Fältnamn får inte börja med följande tecken: **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-5.png)

>[!NOTE]
>
>API-namnet används av SOAP API och andra serverdelsprocesser.

Du kan nu använda det här anpassade fältet i formulär, flödessteg och smarta listor.
