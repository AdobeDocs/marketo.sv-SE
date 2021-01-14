---
unique-page-id: 2951259
description: Anpassad fälttypsordlista - Marketo Docs - Produktdokumentation
title: Ordlista för anpassad fälttyp
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---


# Ordlista för anpassad fälttyp {#custom-field-type-glossary}

När du skapar ett anpassat fält i Marketo finns det en lista med typer att välja mellan.

>[!PREREQUISITES]
>
>[Skapa ett anpassat fält i Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Beroende på fälttyp kommer filter/trigger [operatorer](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) att vara olika.

>[!NOTE]
>
>De flesta fält får inte innehålla maximalt antal tecken, utan i stället en mängd byte. Därför kan vi inte ange en definitiv teckengräns för varje fält. Undantaget är **String**, som är högst vid 255 tecken.

## Boolean {#boolean}

**Exempelnamn:** Är kund - tagga dina personer som kunder

**Exempelvärden:** Sant (markerat) / Falskt (omarkerat)

**Operatorer**: Ingen

## Valuta {#currency}

**Exempelnamn:** Budget - Lagra ett nummervärde för ett företags budget

**Exempelvärden:** 100

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Datum {#date}

**Exempelnamn:** Förnyelsedatum - Lagra dina kunders förnyelsedatum

**Exempelvärden:** 8/19/14

**Operatorer**: är, inte, mellan, tidigare, tidigare, tidigare, i framtiden, efter, i tidsramen, efter, före, på eller efter, är tom, är inte tom

## Datum/tid {#datetime}

**Exempelnamn:** Skapad - Lagra datum och tid då en person skapades

**Exempelvärden:** 8/19/14 2:00

**Operatorer**: är, inte, mellan, tidigare, tidigare, tidigare, i framtiden, efter, i tidsramen, efter, före, på eller efter, är tom, är inte tom

## E-post {#email}

**Exempelnamn:** Alternativ e-postadress - Behåll en alternativ e-postadress för dina personer (det går inte att skicka e-post till det här fältet, t.ex. standardfältet för e-postadress, det är en speciell adress)

**Exempelvärden:** name@company.com

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Float {#float}

**Exempelnamn:** Grad-punktsmedel - Behåll en persons medelpoäng eller något annat numeriskt värde med decimaler

**Exempelvärden:** 2.47

**Operatorer**: mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Formel {#formula}

**Exempelnamn:** Hälsningar - använd det här specialfältet i en  [lösning för att få rätt ](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) lösning baserat på kön

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

**Exempelnamn:** Alternativ telefon - lagra ytterligare ett telefonnummer för dina personer

**Exempelvärde:** 650-555-5555

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Poäng {#score}

**Exempelnamn:** Beteendepoäng/Demografisk poäng - skapa flera poängfält för att hålla reda på olika attribut.

**Exempelvärde:** 14

**Operatorer**: är, inte, mellan, större än, mindre än, åtminstone, är tom, är inte tom

## Sträng {#string}

**Exempelnamn:** Mellannamn - lagra ytterligare ett textattribut

**exempelvärde:** ros

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## Textområde {#text-area}

**Exempelnamn:** Kommentarer - lägg till ett kommentarsfält i formulären så att du kan skriva text på flera rader

**Exempelvärde:** Den här artikeln är fantastisk!

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom

## URL {#url}

**Exempelnamn:** Blogg - skapa ett fält för lagring av personbloggar-URL:er

**Exempelvärde:** www.myblog.com

**Operatorer**: is, is not, startar med, inte börjar med, innehåller, inte innehåller, är tom, är inte tom
