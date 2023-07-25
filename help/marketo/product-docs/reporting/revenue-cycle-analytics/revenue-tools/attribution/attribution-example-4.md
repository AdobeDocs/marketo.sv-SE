---
unique-page-id: 7514151
description: Attribution Example 4 - Marketo Docs - Product Documentation
title: Attribut - exempel 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Attribut - exempel 4 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Michelle laddar ned e-bok (innehåll) - Klart
* 15 april | John deltar (webbinarium) - Klart
* 22 april | (möjlighet 1) skapad för $3 000
* 24 april | (möjlighet 2) skapat för 5 000 USD
* 25 april | John och Michelle är associerade med **båda** Optyer
* 29 april | [Optisk 1] is Closed-Won

| Programnamn | (Innehåll) | (webbinarium) |
|---|---|---|
|   | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Opty har skapats | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline skapad | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Intäkter, vinst | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>När ni har flera möjligheter och flera personer med programframgångar måste ni dela upp krediterna mellan människor och program. Observera dock att krediteringen för affärsmöjligheten 1 och 2 inte kombineras. De utgör en tydlig kreditbedömning.
>
>När många är inblandade beräknar Marketo automatiskt de bråkdelar av en affärsmöjlighet som man kan tillgodoräkna sig.

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
>* [Attribut - exempel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
