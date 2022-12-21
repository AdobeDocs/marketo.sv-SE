---
unique-page-id: 7514146
description: Attribution Example 2 - Marketo Docs - Product Documentation
title: Attribut - exempel 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Attribut - exempel 2 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Fakturan förvärvas av (Tradeshow)
* 15 april | Joan förvärvas av (webbinarium)
* 22 april | (möjlighet 1) skapad för 6 000 USD
* 24 april | (möjlighet 2) skapat för 10 000 USD
* 25 april | Bill och Joan är associerade med roller till **BÅDA** Optyer
* 29 april | (möjlighet 1) är stängd

| Programnamn | (Varumärke) | (webbinarium) |
|---|---|---|
| (FT) Opty skapad | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Pipeline skapad | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Vinstintäkter | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>Eftersom både Bill och Joan var associerade med roller till **BÅDA** affärsmöjligheter, så att systemet (enligt reglerna) fördelar krediten jämnt mellan dem.
>
>Pipeline som skapats för varje program ($8.000) är hälften av det totala beloppet ($16.000) som kan krediteras.

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
>* [Attribut - exempel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attribut - exempel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

