---
unique-page-id: 7514126
description: Attribution Example 1 - Marketo Docs - Product Documentation
title: Attribut - exempel 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Attribut - exempel 1 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Fred förvärvas av (Tradeshow)
* 15 april | Margo Attends (Webinar) - success
* 22 april | Fred är associerad (roll) med affärsmöjligheten
* 22 april | Affärsmöjligheten har skapats för $3 000

| Programnamn | (Varumärke) | (webbinarium) |
|---|---|---|
| (FT) Opty skapad | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline skapad | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Intäkter, vinst | `<pre>0</pre>` | `<pre>0</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>För det första är att förstå att vissa typer är COUNTS och andra är VALUTA. Opty Created är ett antal, ett heltal. Pipeline är en valuta. I Marketo anpassas valutan efter dina inställningar för administratörens språkområde.
>
>Orsaken till att Tradeshow fick all kredit är att Margo inte var associerad med en roll i affärsmöjligheten. Ingen roll, ingen kredit.

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
>* [Attribution Example 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attribution Example 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attribution Example 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
