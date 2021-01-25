---
unique-page-id: 7504676
description: Förstå periodkostnader - Marketo Docs - Produktdokumentation
title: Förstå periodkostnader
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Förstå periodkostnader {#understanding-period-costs}

## Översikt {#overview}

Periodkostnader avser de pengar du spenderar under en viss månad på ett program.

>[!NOTE]
>
>**Exempel**
>
>Om du spenderar 1 000 dollar på att anställa en illustratör till en e-bok som lanseras i juli, skulle e-boksprogrammet ha en periodkostnad på 1 000 dollar i juli.
>
>Om du spenderar 200 USD per månad på Google Adwords har Google Adwords-programmet en periodkostnad på 200 **varje månad**.

>[!NOTE]
>
>[Förstå program](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Förstå programmedlemskap](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Hur periodkostnader beräknas {#how-period-costs-are-calculated}

Tänk dig en händelse, som ett webbinarium, som inträffar i mars. Nya människor köps i förväg från reklam i januari och februari. Nya kontakter hämtas också efter evenemanget, när andra laddar ned webbinariet under april och maj.

1. Med en enda periodkostnad som tillskrivs mars...

   ![](assets/graph1.png)

   ...kontakter som lagts till under månaderna före och efter kommer att *endast* räknas från mars.

   ![](assets/graph2.png)

1. Med periodkostnader i januari, februari och mars ...

   ![](assets/graph3.png)

   ...Kontakter som läggs till endast under månaderna efter mars räknas till mars.

   ![](assets/graph4.png)

1. Med periodkostnader som tillskrivs januari och april ...

   ![](assets/graph5.png)

   ...Kontakter som läggs till under månaderna januari till mars räknas till januari. Kontakter som lagts till under månaderna april och maj räknas till april.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >Sammanfattningsvis - månader utan definierade periodkostnader kommer att gå bakåt till den sista som definierats. Om det inte finns någon kostnad för föregående period kommer månaderna att flyttas fram till nästa som har definierats. Om en periodkostnad inte har definierats för _några_ månader kommer rapportering i RCE inte att vara tillgänglig för programmet.

   >[!MORELIKETHIS]
   >
   >* [Använda periodkostnader i ett program](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrera en programrapport efter periodkostnad](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

