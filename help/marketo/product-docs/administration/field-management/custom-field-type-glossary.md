---
unique-page-id: 2951259
description: Anpassad fälttypsordlista - Marketo Docs - produktdokumentation
title: Ordlista för anpassad fälttyp
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Ordlista för anpassad fälttyp {#custom-field-type-glossary}

När du skapar ett anpassat fält i Marketo har du en lista med typer att välja mellan.

>[!PREREQUISITES]
>
>[Skapa ett anpassat fält i Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Beroende på fälttyp kommer filter/utlösare [operatorer](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) att vara olika.

>[!NOTE]
>
>De flesta fält får inte innehålla maximalt antal tecken, utan i stället en mängd byte. Därför kan vi inte ange en definitiv teckengräns för varje fält. Undantaget är **String**, som är högst 255 tecken långt.

## Boolean {#boolean}

**Exempelnamn:** är kund - tagga dina personer som kunder

**Exempelvärden:** Sant (markerad)/Falskt (avmarkerad)

**Operatorer**: Inga

## Valuta {#currency}

**Exempelnamn:** Budget - Lagra ett talvärde för ett företags budget

**Exempelvärden:** 100

**Operatorer**: är, inte, mellan, större än, mindre än, minst, är tom, är inte tom

## Datum {#date}

**Exempelnamn:** Förnyelsedatum - Lagra dina kunders förnyelsedatum

**Exempelvärden:** 8/19/14

**Operatorer**: är, inte, mellan, tidigare, tidigare, i framtiden, efter, i tidsram, efter, före, på eller efter, på eller före, är tom, är inte tomma

## Datetime {#datetime}

**Exempelnamn:** Skapad - Lagra datum och tid då en person skapades

**Exempelvärden:** 8/19/14 2:00

**Operatorer**: är, inte, mellan, tidigare, tidigare, i framtiden, efter, i tidsram, efter, före, på eller efter, på eller före, är tom, är inte tomma

## E-post {#email}

**Exempelnamn:** Alternativ e-postadress - Behåll en alternativ e-postadress för dina personer (det går inte att skicka e-post till det här fältet, t.ex. standardfältet för e-postadress, det är en speciell adress)

**Exempelvärden:** <name@company.com>

**Operatorer**: är, inte, börjar med, inte med, innehåller, inte innehåller, är tom, är inte tom

## Float {#float}

**Exempelnamn:** Grad-punktsmedel - Behåll en persons medelvärde för poäng eller något annat numeriskt värde med decimaler

**Exempelvärden:** 2.47

**Operatorer**: mellan, större än, mindre än, åtminstone, är tomma, är inte tomma

## Formel {#formula}

**Exempelnamn:** Hälsningar - använd det här specialfältet i en [lösning för att få rätt hälsning](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) baserat på kön

**Exempelvärden:** Kontrollera den länkade lösningen

## Heltal {#integer}

**Exempelnamn:** Antal anställda - lagra ett talvärde som inte kräver decimaler

**Exempelvärden:** 600

**Operatorer**: är, inte, mellan, större än, mindre än, minst, är tom, är inte tom

## Procent {#percent}

**Exempelnamn:** Sannolikt att köpa - lagra ett procentvärde (kanske beräknat på CRM-sidan)

**Exempelvärden:** 85 %

**Operatorer**: är, inte, mellan, större än, mindre än, minst, är tom, är inte tom

## Tel. {#phone}

**Exempelnamn:** Alternativ telefon - lagra ytterligare ett telefonnummer för dina personer

**Exempelvärde:** 650-555-5555

**Operatorer**: är, inte, börjar med, inte med, innehåller, inte innehåller, är tom, är inte tom

## Poäng {#score}

**Exempelnamn:** Beteendepoäng/Demografisk poäng - skapa flera poängfält för att hålla reda på olika attribut

**Exempelvärde:** 14

**Operatorer**: är, inte, mellan, större än, mindre än, minst, är tom, är inte tom

## Sträng {#string}

**Exempelnamn:** Mellannamn - lagra ytterligare ett textattribut

**Exempelvärde:** ros

**Operatorer**: är, inte, börjar med, inte med, innehåller, inte innehåller, är tom, är inte tom

## Textområde {#text-area}

**Exempelnamn:** Kommentarer - lägg till ett kommentarsfält i formulären för att tillåta flerradig text

**Exempelvärde:** Den här artikeln är fantastisk!

**Operatorer**: är, inte, börjar med, inte med, innehåller, inte innehåller, är tom, är inte tom

## URL {#url}

**Exempelnamn:** Blogg - skapa ett fält för lagring av personbloggens URL

**Exempelvärde:** &lt;www.myblog.com>

**Operatorer**: är, inte, börjar med, inte med, innehåller, inte innehåller, är tom, är inte tom
