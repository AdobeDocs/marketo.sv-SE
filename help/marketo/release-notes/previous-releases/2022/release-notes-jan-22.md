---
description: Versionsinformation - januari 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - januari 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# Versionsinformation: Januari 2022 {#release-notes-jan-22}

Följande funktioner finns i januari 22. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att lanseras den **21 januari 2022**, med en fasad utrullning av alla funktioner under de följande veckorna (om inget annat anges).

## Nästa generations upplevelse {#modern-ux}

* **Uppdaterade skärmar i nästa generation**: Vi levererar nya, uppdaterade skärmar i nästa generation av upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Information om landningssidans resurser i Design Studio
   * Information om landningssidans tillgångar i marknadsföringsaktiviteter

## Integrering med Microsoft Dynamics {#microsoft-dynamics-integration}

* **Synkronisering av fälttypen Multiselect OptionSet är vanligtvis tillgänglig**: Synkronisera fälttypen för flervalsalternativ från Microsoft Dynamics för att utnyttja Smart Lists och Smart Campaigns för mer detaljerad målgruppsanpassning. Exempel: ämnen/produkter av intresse, kommunikationslägen med mera. Den här nya synkroniseringen är tillgänglig för Microsoft Dynamics version 9.X (inklusive Dynamics 365 Online).

* **Server-till-server-autentisering för Microsoft Dynamics 365 Online**: För ökad säkerhet kommer vi nu att ha stöd för Server-till-server (S2S) som ett extra autentiseringssätt för Marketo Engage-synkroniseringsanvändaren på Azure Active Directory för icke-interaktiv åtkomst till Microsoft Dynamics 365 Online. Detta gör att du kan använda multifaktorautentisering, eftersom all autentisering och alla inloggningar baseras på OAuth (endast klient-ID och klienthemlighet).

>[!NOTE]
>
>S2S-läget baseras på Application User (Programanvändare) i stället för Licensed User (Licensierad användare), vilket sparar pengar på att använda ytterligare en licens.

## Administration {#administration}

* **[Formulärvalideringsregler](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Bevara databasens hälsotillstånd och blockera problematiska eller oönskade e-postdomäner från att skicka formulär i Marketo Engage. På panelen Valideringsregel för globala formulär kan administratörer definiera en blockeringslista eller aktivera en fördefinierad lista med kostnadsfria konsumentdomäner som ska blockeras från formulär.

* **[Säkerhet för landningssidhuvud](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Administratörer kan hantera rubrikerna Strict Transport Security och X-Frame Options på sina landningssiddomäner för att upprätthålla höga säkerhetskrav.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## AEP Marketo Engage Destination Connector - Skapa nya NetLeads {#aep-marketo-engage-destination-connector}

Marketo Engage-kunder som också använder Adobe Experience Platform (AEP) kan maximera sin databas genom att överföra nästa-nya personposter till Marketo Engage från AEP via AEP-destinationsanslutningen. När du skickar målgruppssegment från AEP till Marketo Engage, personer i segmentet som inte redan finns i din Marketo Engage-databas [kan läggas till automatiskt](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

**Försäljningsinsikter för Salesforce CRM**

* **Ny typkolumn för bästa val**: Säljarna får snabbare insikter med en ny kolumn som heter&quot;Typ&quot; för att skilja mellan leads och kontakter på sidan Bästa val.

* **Uppdatering för Salesforce Platform API**: Som svar på att Salesforce upphör med Salesforce Platform API-versionerna 21.0 till 30.0 har Sales Insight-paketet uppdaterats med de senaste API:erna.

* **Uppdaterad profilering**: Alla Sales Insight-sidor uppdateras för att passa Adobe.

**Sales Insight for Microsoft Dynamics**

* **Uppdaterad kontolayout**: Säljarna kan få en samlad bild av de viktigaste aktiviteterna som: e-postaktiviteter, webbaktiviteter, intressanta ögonblick och poängändringar för alla kontakter i ett konto.

## Sales Connect {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Utfall och orsaker**: Förstå och spåra säljteamets utgående satsningar mer i detalj med nya, fullt anpassningsbara samtalsresultat och alternativ för samtalsorsaker. Förutom dessa nya fält introducerar vi nya styrfunktioner för att framtvinga val av anropsorsak och -utfall medan säljarna gör samtal, ny styrning för att aktivera eller inaktivera samtalsorsaker och -utfall samt ett nytt anpassat fält för Salesforce-aktivitet för samtalsorsak och samtalsutfall för att logga data till Salesforce. [Klicka här](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) om du vill veta mer.

* **Detaljanpassning av Salesforce-aktivitet**: Samla in fler data om försäljningsaktivitet och uppgifter i Salesforce genom att anpassa vilken information som läggs till i Salesforce-aktivitetens ämnesfält när en försäljningsaktivitet loggas till Salesforce från Sales Connect. [Klicka här](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) om du vill veta mer.

## Meddelanden {#announcements}

* **Borttagning av Marketo Sky**: I mars kommer Marketo Sky inte längre att vara tillgänglig eftersom vi fokuserar på att leverera nästa generations användarupplevelser. I ett försök att behålla åtkomst till funktioner som är exklusiva för Marketo Skyn idag, tar vi med åsidosättande av förfallodatum och prioritet för smarta kampanjer i den vanliga upplevelsen i mars. [Klicka här](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) om du vill veta mer.

* **Borttagning av formulärslutpunkter**: POST:er för programmatiska formulär till leadCapture/save2-slutpunkten stöds inte av Marketo Engage-formulär. [Klicka här](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) om du vill veta mer.

**Marketo Engage-domäner - konfiguration för Sales Insight**: För Marketo Engage-domäner som inte har SSL-certifikat aktiverat och https://, misslyckas anrop med ett SSL-handskakningsfel. Därför kommer dessa domäner att upphöra. Detta innebär att användare av Sales Insight med en äldre konfiguration som pekar på någon av dessa domäner kan råka ut för bildtextsfel på sin Lead-, Contact-, Account-, Opportunity Panels- eller Marketo Global-sida. Vi rekommenderar att du uppdaterar din [Marketo Engage-konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) i Salesforce om det här felet inträffar. Du behöver bara uppdatera inloggningsuppgifterna för Marketo Engage som är markerade i avsnittet&quot;Marketo Sales Insight Config&quot; i dokumentet.

**_Product Release Webinar_**

[Webbinariet Marketo Engage från januari 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
