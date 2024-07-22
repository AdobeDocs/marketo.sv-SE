---
unique-page-id: 4719316
description: Använda personkonton - Marketo Docs - produktdokumentation
title: Använda personkonton
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Använda personkonton {#using-person-accounts}

Personkonton kan konfigureras i Salesforce för att passa behoven i din organisation. Så här behandlar Marketo Engage personkonton.

>[!NOTE]
>
>Salesforce-standardkonton är affärskonton. Din Salesforce-administratör måste konfigurera personkonton separat.

## Vad är ett personkonto? {#what-is-a-person-account}

Ett personkonto liknar kontoobjektet i Salesforce. Ett personkonto har dock åtkomst till både kontofält och kontaktfält.

## Vad händer när ett personkonto synkroniseras med Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Ett personkonto synkroniseras till Marketo som ett företag och som en person.

>[!NOTE]
>
>De anpassade fälten för ett personkonto kopieras till både företag och person i Marketo.

## Hur skiljer jag på affärskonton och personkonton? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Använd filtret Är personkonto i din smarta lista för att skilja personkonton från vanliga affärskonton.

## Var visas informationen om mitt personkonto i Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Aktiviteter som rör personkonton visas på panelen **[!UICONTROL Account]**.

>[!NOTE]
>
>Marketo Sales Insight-alternativen **[!UICONTROL Add to Marketo Campaign]** och **[!UICONTROL Send Email]** är för närvarande inte tillgängliga för personkonton.

## Hur kopplar jag affärsmöjligheter till ett personkonto? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo är beroende av kontaktrollen för affärsmöjligheten för att avgöra vilken person som affärsmöjligheten ska kopplas till. Du måste lägga till kontaktrollen för affärsmöjligheten för varje personkonto för att kunna ansluta affärsmöjligheten till rätt person i Marketo. Vi rekommenderar att du skapar ett arbetsflöde för att lägga till kontaktrollen för affärsmöjligheten automatiskt.

## Vilket e-postfält ska jag använda för personkonton? {#which-email-field-should-i-use-for-person-accounts}

Det finns två e-postfält för ett personkonto. Använd fältet **E-postadress** i dina formulär (inte **Personens e-postadress**) för att se till att Marketo deduplicering och annan e-postbearbetning fungerar som de ska.
