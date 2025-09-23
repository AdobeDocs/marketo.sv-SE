---
unique-page-id: 2360327
description: Tilldela personpartitioner med tilldelningsregler - Marketo Docs - produktdokumentation
title: Tilldela personpartitioner med tilldelningsregler
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%

---

# Tilldela personpartitioner med tilldelningsregler {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>[Skapa en personpartition](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

När du använder personpartitioner ska du ställa in tilldelningsregler för att dirigera personer som skapats från CRM till sina respektive partitioner.

>[!NOTE]
>
>Endast personer som har skapats i Marketo från din CRM och via SOAP API får tilldelningsregler tillämpade på dem.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Klicka på **[!UICONTROL Workspaces & Partitions]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Klicka på **[!UICONTROL Person Partitions]** på fliken **[!UICONTROL Assignment Rules]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Klicka på **[!UICONTROL Add Choice]** om du vill lägga till villkor för att dirigera personer till personpartitioner.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Markera fältet som villkoret ska byggas på.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Välj önskad operator och ange ett värde.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Markera den personpartition som du vill att de personer som uppfyller villkoren ska ingå i.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Du kan lägga till så många alternativ du vill.

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

Och där har du den! Du har tilldelat regler för att fylla dina personpartitioner med personer!

>[!NOTE]
>
>Standardalternativet används om inget av de föregående villkoren uppfylls.
