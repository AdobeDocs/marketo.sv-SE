---
unique-page-id: 2360327
description: Tilldela personpartitioner med tilldelningsregler - Marketo Docs - produktdokumentation
title: Tilldela personpartitioner med tilldelningsregler
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

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
>Endast personer som har skapats i Marketo från din CRM och via SOAP API:t kommer att ha tilldelningsregler tillämpade på dem.

1. Klicka på Arbetsytor och partitioner under Admin.

   ![](assets/image2014-9-17-10-3a32-3a55.png)

1. Under **Personpartitioner** flik, klicka på **Uppdragsregler**.

   ![](assets/two-6.png)

1. Klicka **Lägg till alternativ** för att lägga till villkor för att dirigera personer till personpartitioner.

   ![](assets/three-6.png)

1. Markera fältet som villkoret ska byggas på.

   ![](assets/four-5.png)

1. Välj önskad operator och ange ett värde.

   ![](assets/five-1.png)

1. Markera den personpartition som du vill att de personer som uppfyller villkoren ska ingå i.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Du kan lägga till så många alternativ du vill.

1. Klicka **Spara**.

   ![](assets/seven.png)

Och där har du den! Du har tilldelat regler för att fylla dina personpartitioner med personer!

>[!NOTE]
>
>Standardalternativet används om inget av de föregående villkoren uppfylls.
