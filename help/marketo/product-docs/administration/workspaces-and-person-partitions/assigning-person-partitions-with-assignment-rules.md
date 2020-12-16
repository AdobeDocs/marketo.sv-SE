---
unique-page-id: 2360327
description: Tilldela personpartitioner med tilldelningsregler - Marketo-dokument - Produktdokumentation
title: Tilldela personpartitioner med tilldelningsregler
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
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
>* [Skapa en personpartition](create-a-person-partition.md)

>



När du använder personpartitioner ska du ställa in tilldelningsregler för att dirigera personer som skapats från CRM till sina respektive partitioner.

>[!NOTE]
>
>Endast personer som har skapats i Marketo från din CRM och via SOAP API kommer att ha tilldelningsregler tillämpade på dem.

1. Klicka på Arbetsytor och partitioner under Admin.

![](assets/image2014-9-17-10-3a32-3a55.png)

1. Under fliken **Personpartitioner **klickar du på **Uppdragsregler**.

   ![](assets/two-6.png)

1. Klicka på **Add Choice **för att lägga till villkor för att dirigera personer till personpartitioner.

   ![](assets/three-6.png)

1. Markera fältet som villkoret ska byggas på.

   ![](assets/four-5.png)

1. Välj önskad operator och ange ett värde.
1. ![](assets/five-1.png)

1. Markera den personpartition som du vill att de personer som uppfyller villkoren ska ingå i.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >
   >Du kan lägga till så många alternativ du vill.

   Klicka på Spara.
   ![](assets/seven.png)

Och där har du den! Du har tilldelat regler för att fylla dina personpartitioner med personer!

>[!NOTE]
>
>Standardalternativet används om inget av de föregående villkoren uppfylls.

