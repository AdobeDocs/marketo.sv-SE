---
unique-page-id: 4719316
description: Använda personkonton - Marketo Docs - Produktdokumentation
title: Använda personkonton
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Använda personkonton {#using-person-accounts}

Personkonton kan konfigureras i Salesforce för att passa behoven i din organisation. Så här behandlar Marketo personkonton.

>[!NOTE]
>
>Salesforce-standardkonton är affärskonton. Din Salesforce-administratör måste konfigurera personkonton separat.

## Vad är ett personkonto? {#what-is-a-person-account}

Ett personkonto liknar kontoobjektet i Salesforce. Ett personkonto har dock åtkomst till både kontofält och kontaktfält.

## Vad händer när ett personkonto synkroniseras med Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ett personkonto synkroniseras med Marketo som ett företag och som en person.

>[!NOTE]
>
>De anpassade fälten för ett personkonto kopieras till både företag och person i Marketo.

## Hur skiljer jag på affärskonton och personkonton? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Använd filtret **Är personkonto** i den smarta listan för att separera personkonton från standardaffärskonton.

## Var visas min personkontoinformation i Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktiviteter som rör personkonton visas på panelen **Konto**.

>[!NOTE]
>
>Marketo Sales Insight-alternativen **Lägg till i Marketo Campaign** och **Skicka e-post** är för närvarande inte tillgängliga för personkonton.

## Hur kopplar jag affärsmöjligheter till ett personkonto? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo är beroende av säljprojektens kontaktroll för att avgöra vilken person som affärsmöjligheten ska kopplas till. Du måste lägga till kontaktrollen för affärsmöjligheten för varje personkonto för att kunna ansluta affärsmöjligheten till rätt person i Marketo. Vi rekommenderar att du skapar ett arbetsflöde för att lägga till kontaktrollen för affärsmöjligheten automatiskt.

## Vilket e-postfält ska jag använda för personkonton? {#which-email-field-should-i-use-for-person-accounts}

Det finns två e-postfält för ett personkonto. Använd fältet **E-postadress** i dina formulär (inte **Personens e-postadress**) för att säkerställa att Marketos borttagning av dubbletter och annan e-postbearbetning fungerar som den ska.
