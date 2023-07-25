---
unique-page-id: 7514149
description: Attribution Example 3 - Marketo Docs - Product Documentation
title: Attribut - exempel 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# Attribut - exempel 3 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Steve Downloads (Content) - success
* 22 april | Affärsmöjlighet skapas för 3 000 USD (både Steve och Jason har roller)
* 25 april | Jason Attends (Webinar) - success
* 30 april | Affärsmöjligheten är avbruten

| Attributionsmått | (Innehåll) | (webbinarium) |
|---|---|---|
| (MT) Opty har skapats | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline skapad | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Intäkter, vinst | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>Kom ihåg attribueringsregel nr 3. Jason lyckades med programmet EFTER att optyn skapades. Det innebär att webbinariet inte kan få något erkännande för skapandet av affärsmöjligheten. Endast tillgodoräknande för Opty vann.
>
>(Innehåll) har därför 100 % av äran för Opty-projektet och rörledningen, men bara 50 % rabatt på optyt.

>[!NOTE]
>
>**Attributionsregler**
>
>1. Krediten delas jämnt
>1. Du kan inte ge mer beröm än du har fått
>1. Du kan inte tillgodoräkna dig något som hänt tidigare

Prova alla exempel så blir du ett attribueringsproffs!

>[!MORELIKETHIS]
>
>* [Attribut - exempel 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attribut - exempel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attribut - exempel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
