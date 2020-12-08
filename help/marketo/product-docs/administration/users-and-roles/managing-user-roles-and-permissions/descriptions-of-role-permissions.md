---
unique-page-id: 6848747
description: Beskrivningar av rollbehörigheter - Marketo Docs - Produktdokumentation
title: Beskrivningar av rollbehörigheter
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Beskrivningar av rollbehörigheter {#descriptions-of-role-permissions}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Nedan visas en lista med alla tillgängliga behörigheter som du kan tilldela dina roller. Behörigheter är vanligtvis kopplade till specifika funktionsområden i Marketo och kan hjälpa dig att styra vilka områden och funktioner olika användare har tillgång till.

Ytterligare information om behörigheter:

* Behörigheten&quot;Åtkomst&quot; ger en roll behörighet att visa och ibland redigera den delen av programmet.
* För att en roll ska ha åtkomst till underbehörigheterna (&quot;Skapa&quot;,&quot;Ta bort&quot;, osv.) måste den rollen ha&quot;Åtkomst&quot;-behörighet till den delen av programmet. Om du till exempel vill ge någon behörighet att redigera kampanjer måste de ha övergripande behörighet att få åtkomst till marknadsföringsaktiviteter.
* Du kanske kan se åtgärder eller resurser som du inte har behörighet att använda. Om du försöker få åtkomst till dem visas ett varningsmeddelande om din begränsade åtkomst.

## Tillgängliga behörigheter {#available-permissions}

När du [skapar eller redigerar en roll](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)kan du välja vilken av följande behörigheter som ska tillåtas för den rollen genom att markera lämpliga rutor.

![](assets/createnewrole.png)

## Åtkomstadministratör  {#access-admin}

Visa och gör ändringar i inställningarna under Mitt konto i Admin.

* Åtkomst till granskningsspår - Ger användare åtkomst till både resursgranskningsspår och administratörsgranskningsspår
* Åtkomstkanaler - Ger användarna åtkomst endast för att ändra kanaltaggen, inte andra anpassade taggar
* Kommunikationsgräns för åtkomst - Ger användarna åtkomst för att aktivera en kommunikationsgräns i Admin
* Access CRM - Ger användare åtkomst till CRM, som Salesforce eller Microsoft Dynamics, i Admin
* Access [Data.com](http://Data.com) - ger användarna åtkomst till flödesåtgärden Data.com
* Åtkomst till e-postadministratör - Ger användare behörighet att ändra standardinställningar, som att avbeställa prenumerationer och ange varumärke
* Åtkomst till händelsepartners - Ger användarna åtkomst till LaunchPoint i Admin
* Fälthantering för åtkomst - ger användarna åtkomst till fälthantering i Admin
* Access File Upload - Ger användarna möjlighet att överföra bilder och filer till Design Studio
* Åtkomst till landningssidor - ger användarna åtkomst till landningssidor i administratören
* Åtkomstplats - Ger användare åtkomst till plats i Admin för att ange standardspråk, nationella inställningar, tidszon och valuta
* Åtkomst till inloggningshistorik - Ger användare åtkomst till användarens inloggningshistorik i granskningsspår
* Åtkomst till inloggningsinställningar - Ger användarna åtkomst till inloggningsinställningar i Admin för inställningar av säkerhet, IP-begränsningar och Smart List-rapporter
* Access Marketo Custom Activity (Anpassad aktivitet för Access Marketo) - ger användarna åtkomst till anpassade aktiviteter i Admin
* Anpassat objekt för Access Marketo - Ger användare åtkomst till anpassade objekt i Marketo i Admin
* Access Munchkin - glittrar användare tillgång till Munchkin i Admin för att ställa in spårningskod, personspårning och aktivera API-konfiguration
* Access Revenue Cycle Analytics (Åtkomstcykelanalys) - Ger användarna tillgång till Intäktscykelanalys i Admin, för inställning av Synkroniseringssammanfattning och Attribution
* Åtkomstroller - Ger användare åtkomst till att hantera och redigera roller, men inte användare
* Access Sales Insight - Ger användare åtkomst till att hantera Sales Insight i Admin för att ange status, API-konfiguration, personbedömning och andra inställningar
* Åtkomst till enkel inloggning - Ger användarna åtkomst till att hantera enkel inloggning i Admin, för att aktivera SAML och arbeta med SAML-inställningar och URL:er för omdirigeringssida
* Access Smart Campaign - Ger användarna tillgång till Smart Campaign i Admin, för att begränsa begränsningarna för kvalificerade personer
* Åtkomst till SOAP API - ger användarna åtkomst till att hantera SOAP API:er i webbtjänster i Admin
* Åtkomsttaggar - Ger användarna åtkomst till alla anpassade taggar utom kanaltaggen
* Access Treasure Chest - Ger användarna tillgång till de experimentella funktionerna i Resurs Chest i Admin
* Åtkomstanvändare - Ger användare åtkomst till att redigera och hantera användare (men inte roller) i Admin
* Åtkomst till webbhooks - Ger användare tillgång till webbhooks i Admin för att ställa in information och svarsmappningar
* Åtkomst till arbetsytor och partitioner - Ger användarna tillgång till arbetsytor och partitioner i administratören för att skapa, redigera och ta bort

## Åtkomst-API  {#access-api}

Ger användare åtkomst till de enskilda API:erna som anges nedan med enbart **** API- **rollen** .

* Godkänn resurser
* Kör kampanj
* Skrivskyddad aktivitet
* Metadata för skrivskyddad aktivitet
* Skrivskyddade resurser
* Skrivskyddad kampanj
* Skrivskyddat företag
* Skrivskyddat anpassat objekt
* Skrivskyddad person
* Skrivskyddat namngivet konto
* Skrivskyddad möjlighet
* Skrivskyddad säljare
* Aktivitet för läsning/skrivning
* Metadata för aktiviteten Read-Write
* Skrivskyddade resurser
* Read-Write Campaign
* Läs/skriv företag
* Anpassat objekt för läsning/skrivning
* Skrivskyddad person
* Läs/skriv namngivet konto
* Möjligheter att läsa och skriva
* Skrivskyddad säljare

Åtkomstanalys

Ger användarna åtkomst till Analytics-flikarna, e-postinsikter, rapporter och de tre objekten nedan, om de inte är avmarkerade.

* Access Revenue Explorer (Handkomstutforskaren) - Avmarkering tar bort användarens åtkomst till Intresseutforskaren
* Ta bort rapport - Avmarkera tar bort användarens möjlighet att ta bort rapporter
* Exportera analysdata - Avmarkering tar bort användarens möjlighet att exportera analysdata

## Öppna Kalender för Presentations {#access-calendar-presentations}

Ger användare åtkomst till kalenderpresentationer ??- aktiverar visning av Presentations-knappen längst ned?

* Redigera kalender i Presentations - Gör att användare kan redigera presentationer i kalendern

## Access Design Studio {#access-design-studio}

Ger användarna tillgång till fliken Design Studio och trädvyn, men inte till detaljer.

* Åtkomst till e-post

   * Redigera e-post - Ger användare behörighet att redigera, skapa och klona e-postmeddelanden

      * Använd e-post - Ger användare behörighet att göra e-postmeddelanden operativa. Se: [Låt e-postmeddelanden fungera](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)
   * Godkänn e-post - Låter användarna godkänna e-postmeddelanden.
   * Ta bort e-post - Gör det möjligt för användare att ta bort e-postmeddelanden.
   * Ange profilerad domän - Gör att användare kan arbeta med profileringsdomäner. Se: [Lägg till flera varumärkesdomäner](http://docs.marketo.com/display/docs/add+multiple+branding+domains)


* E-postmall för åtkomst

   * Godkänn e-postmall
   * Ta bort e-postmall
   * Redigera e-postmall - Redigera, skapa och klona e-postmallar

* Åtkomstformulär

   * Ta bort formulär
   * Redigera formulär - Redigera, skapa och klona formulär

* Åtkomstbild

   * Ta bort bild
   * Överför bild

* Åtkomst till landningssida

   * Godkänn landningssida
   * Ta bort landningssida
   * Redigera landningssida - Redigera, skapa och klona landningssidor

* Access Landing Page Template

   * Godkänn mall för landningssida
   * Ta bort mall för landningssida
   * Redigera mall för landningssida - Redigera, skapa och klona mallar för landningssidor

* Åtkomstfragment

   * Godkänn fragment
   * Ta bort fragment
   * Redigera fragment

* Access Social App

   * Godkänn social app
   * Ta bort social app
   * Redigera social app

## Åtkomstdatabas {#access-database}

Visa databasen samt visa och redigera smarta/statiska listor.

* Åtkomstsegmentering

   * Godkänn segmentering
   * Ta bort segmentering
   * Redigera segmentering

* Import av avancerad lista
* Ta bort person
* Ta bort lista
* Redigera person - Förhindrar manuell redigering och att enstaka flödessteg körs. kan du fortfarande redigera människor genom att köra kampanjer mot dem
* Exportera person - Exportera kalkylblad med från databaslistor
* Importera anpassat objekt
* Importera lista
* Sammanfoga personer
* Kör enkelflödesåtgärder - Gör det möjligt för användare att köra flödessteget **Ändra datavärde** på personer från databasen

* Visa affärsmöjlighetsdata - Döljer affärsmöjlighetsinformationen på personinformationssidan

## Access Marketing Activities {#access-marketing-activities}

Visa fliken Marknadsföringsaktiviteter, kampanjer och kampanjmappar.

* Åtkomst till SMS-meddelande

   * Godkänn SMS-meddelande
   * Ta bort SMS-meddelande
   * Redigera SMS-meddelande

* Åtkomstpush-meddelande

   * Godkänn push-meddelande
   * Ta bort push-meddelande
   * Redigera push-meddelande

* Access Awards
* Aktivera utlösarkampanj
* Godkänn e-postprogram
* Klona marknadsföringsresurs
* Ta bort marknadsföringsresurs
* Redigera kampanjbegränsningar
* Redigera marknadsföringsmaterial
* Importprogram
* Importera lista
* Schemalägg batchkampanj

Åtkomst-SEO

* Administrera SEO
* Standard SEO

## Målinriktning och personalisering {#targeting-and-personalization}

* Administrera webbanpassning
* CRE Campaign Editor
* CRE Campaign Launcher
* Webbkampanjredigerare
* Web Campaign Launcher

Administration av arbetsytan

* Administratörsåtkomst för en viss arbetsyta (endast om du har aktiverat Arbetsytor)
* Flytta resurser mellan arbetsytor (endast om du har aktiverat arbetsytor)

Access Mobile Application
