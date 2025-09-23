---
unique-page-id: 2360287
description: Skapa ett anpassat fält i Marketo - Marketo Docs - produktdokumentation
title: Skapa ett anpassat fält i Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 1%

---

# Skapa ett anpassat fält i Marketo {#create-a-custom-field-in-marketo}

Så här skapar du ett nytt anpassat fält i Marketo Engage för att lagra/hämta in data.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. Klicka på **[!UICONTROL Field Management]**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >Om du vill att fälten ska synkroniseras med CRM skapar du dem i CRM så skapas de automatiskt i Marketo.

1. Klicka på **[!UICONTROL New Custom Field]**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. Välj _[!UICONTROL Object]_.

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >Du kan inte välja _Company_-objektet själv, men du kan begära det genom att kontakta [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

1. Välj fältet _[!UICONTROL Type]_. Detta ändrar hur det återges i smarta listor och formulär i Marketo.

   >[!TIP]
   >
   >Ta en titt på ordlistan [Anpassade fälttyper](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. Ange _[!UICONTROL Name]_så som du vill att den ska visas i Marketo (_[!UICONTROL API Name]_ genereras automatiskt). Välj noggrant eftersom namnet inte kan ändras när du har sparat. Klicka på **[!UICONTROL Create]** när du är klar.

>[!CAUTION]
>
>Fältnamn får inte börja med följande tecken: **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>API-namnet används av SOAP API och andra serverdelsprocesser.

Nu kan du använda det här anpassade fältet i formulär, flödessteg och smarta listor!
