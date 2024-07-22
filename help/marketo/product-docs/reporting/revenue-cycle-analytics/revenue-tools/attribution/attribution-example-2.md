---
unique-page-id: 7514146
description: Attribution Example 2 - Marketo Docs - Product Documentation
title: Attribut - exempel 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Attribut - exempel 2 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Bill förvärvas av (Tradeshow)
* 15 april | Joan förvärvas av (webbinarium)
* 22 april | (Möjlighet 1) skapad för $6 000
* 24 april | (Möjlighet 2) har skapats för $10 000
* 25 april | Bill och Joan är associerade med roller till **BÅDE** Optys
* 29 april | (Möjlighet 1) är stängd-Won

| Programnamn | (Varumärke) | (webbinarium) |
|---|---|---|
| (FT) Opty skapad | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Pipeline skapad | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Intäkter, vinst | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>Eftersom både Bill och Joan associerades med roller till **BTH**-affärsmöjligheter, delade systemet (enligt reglerna) krediten jämnt mellan dem.
>
>Pipeline som skapats för varje program ($8.000) är hälften av det totala beloppet ($16.000) som kan krediteras.

>[!NOTE]
>
>**Attribution Rules**
>
>1. Krediten delas jämnt
>1. Du kan inte ge mer beröm än du har fått
>1. Du kan inte tillgodoräkna dig något som hänt tidigare

Prova alla exempel så blir du ett attribueringsproffs!

>[!MORELIKETHIS]
>
>* [Attribution Example 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attribution Example 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attribution Example 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
