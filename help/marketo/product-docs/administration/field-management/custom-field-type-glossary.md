---
unique-page-id: 2951259
description: Anpassad fälttypsordlista - Marketo Docs - Produktdokumentation
title: Ordlista för anpassad fälttyp
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Ordlista för anpassad fälttyp {#custom-field-type-glossary}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

När du skapar ett anpassat fält i Marketo finns det en lista med typer att välja mellan.

>[!NOTE]
>
>**Förutsättningar**
>
>* [Skapa ett anpassat fält i Marketo](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>Beroende på fälttyp kommer filter-/ [utlösaroperatorer](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) att vara olika.

>[!NOTE]
>
>De flesta fält får inte innehålla maximalt antal tecken, utan i stället en mängd byte. Därför kan vi inte ange en definitiv teckengräns för varje fält. Undantaget är **String**, som är högst 255 tecken långt.

## Boolean {#boolean}

**Exempelnamn:** Är kund - tagga dina medarbetare som kunder

**Exempelvärden:** True (checked) / False (unchecked)

**Operatorer**: Ingen

## Valuta {#currency}

**Exempelnamn:** Budget - Lagra ett nummervärde för ett företags budget

**Exempelvärden:** 100

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Datum {#date}

**Exempelnamn:** Förnyelsedatum - Lagra dina kunders förnyelsedatum

**Exempelvärden:** 8/19/14

**Operatorer**: är, inte, mellan, tidigare, tidigare, tidigare, i framtiden, efter, i tidsramen, efter, före, på eller efter, är tom, är inte tom

## Datetime {#datetime}

**Exempelnamn:** Skapad - Lagra datum och tid då en person skapades

**Exempelvärden:** 8/19/14 2:00

**Operatorer**: är, inte, mellan, tidigare, tidigare, tidigare, i framtiden, efter, i tidsramen, efter, före, på eller efter, är tom, är inte tom

## E-post {#email}

**Exempelnamn:** Alternativ e-postadress - Behåll en alternativ e-postadress för dina personer (det går inte att skicka e-post till det här fältet, t.ex. standardfältet för e-postadress, det är en speciell adress)

**Exempelvärden:** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Float {#float}

**Exempelnamn:** Grad - Behåll en persons medelvärde för poäng eller något annat numeriskt värde med decimaler

**Exempelvärden:** 2,47

**Operatorer**: mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Formel {#formula}

**Exempelnamn:** Hälsningar - använd det här speciella fältet i en [lösning för att få rätt hälsning](create-and-use-a-concatenated-string-formula-field.md) baserat på kön

**Exempelvärden:** kontrollera den länkade lösningen

## Heltal {#integer}

**Exempelnamn:** Antal anställda - lagra ett talvärde som inte kräver decimaler

**Exempelvärden:** 600

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Procent {#percent}

**Exempelnamn:** Sannolikt att köpa - lagra ett procentvärde (kanske beräknat på CRM-sidan)

**Exempelvärden:** 85 %

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Telefon {#phone}

**Exempelnamn:** Alternativ telefon - lagra ytterligare ett telefonnummer åt dina medarbetare

**Exempelvärde:** 650-555-5555

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Poäng {#score}

**Exempelnamn:** Beteendepoäng/Demografisk poäng - skapa flera poängfält för att hålla reda på olika attribut.

**Exempelvärde:** 14

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Sträng {#string}

**Exempelnamn:** Mellannamn - lagra ytterligare ett textattribut

**Exempelvärde:** ros

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Textområde {#text-area}

**Exempelnamn:** Kommentarer - lägg till ett kommentarsfält i formulären så att du kan skriva text på flera rader

**Exempelvärde:** Den här artikeln är fantastisk!

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## URL {#url}

**Exempelnamn:** Blogg - skapa ett fält för lagring av personblogg-URL:er

**Exempelvärde:** www.myblog.com

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom
