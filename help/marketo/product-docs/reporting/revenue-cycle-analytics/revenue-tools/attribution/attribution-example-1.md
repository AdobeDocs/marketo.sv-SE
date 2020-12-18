---
unique-page-id: 7514126
description: Attribution Example 1 - Marketo Docs - produktdokumentation
title: Attribut - exempel 1
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Attributionsexempel 1 {#attribution-example}

Läs följande scenario och försök fastställa vilka tal som ska finnas i rutnätet.

* 11 april | Fred förvärvas av (Tradeshow)
* 15 april | Margo-deltagare (webbinarium) - klar
* 22 april | Fred är associerad (roll) med affärsmöjligheten
* 22 april | Affärsmöjlighet skapas för $3 000

| Programnamn | (Varumärke) | (webbinarium) |
|---|---|---|
| (FT) Opty skapad | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline skapad | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Vinstintäkter | `<pre>0</pre>` | `<pre>0</pre>` |

**Visa svar**

>[!NOTE]
>
>**Förklaring**
>
>För det första är att förstå att vissa typer är COUNTS och andra är VALUTA. Opty Created är ett antal, ett heltal. Pipeline är en valuta. I Marketo anpassas valutan efter inställningarna för administratörens språkområde.
>
>Orsaken till att Tradeshow fick all kredit är att Margo inte var associerad med en roll i affärsmöjligheten. Ingen roll, ingen kredit.

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
>* [Attribut - exempel 2](attribution-example-2.md)
>* [Attribut - exempel 3](attribution-example-3.md)
>* [Attribut - exempel 4](attribution-example-4.md)

