---
unique-page-id: 2360327
description: Tilldela personpartitioner med tilldelningsregler - Marketo-dokument - Produktdokumentation
title: Tilldela personpartitioner med tilldelningsregler
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Tilldela personpartitioner med tilldelningsregler {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Förutsättningar**
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

