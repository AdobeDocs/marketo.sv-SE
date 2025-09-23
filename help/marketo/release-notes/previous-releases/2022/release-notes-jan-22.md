---
description: Versionsinformation - januari 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - januari 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Versionsinformation: januari 2022 {#release-notes-jan-22}

Följande funktioner finns i januari 22. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att börja släppas den **21 januari 2022**, med en fasad utrullning av alla funktioner under de följande veckorna (om inget annat anges).

## Nästa generations upplevelse {#modern-ux}

* **Uppdaterade Screens i nästa generations upplevelse**: Vi levererar nya, uppdaterade skärmar i nästa generations upplevelser som erbjuder uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion:

   * Information om landningssidans tillgångar i [!UICONTROL Design Studio]
   * Information om landningssidans tillgångar i [!UICONTROL Marketing Activities]

## Integrering av [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Synkronisering av fälttypen Multiselect OptionSet är vanligtvis tillgänglig**: Synkronisera fälttypen multiselect optionset från [!DNL Microsoft Dynamics] för användning i smarta listor och smarta kampanjer för mer detaljerad målgruppsanpassning. Exempel: ämnen/produkter av intresse, kommunikationslägen med mera. Den här nya synkroniseringen är tillgänglig för [!DNL Microsoft Dynamics] version 9.X (inklusive Dynamics 365 Online).

* **Server-till-server-autentisering för[!DNL Microsoft Dynamics 365 Online]**: För ökad säkerhet kommer vi nu att ha stöd för Server till Server (S2S) som ett extra autentiseringsläge för Marketo Engage synkroniseringsanvändare på Azure Active Directory för icke-interaktiv åtkomst till [!DNL Microsoft Dynamics 365 Online]. Detta gör att du kan använda multifaktorautentisering, eftersom all autentisering och alla inloggningar baseras på OAuth (endast klient-ID och klienthemlighet).

>[!NOTE]
>
>S2S-läget baseras på Application User (Programanvändare) i stället för Licensed User (Licensierad användare), vilket sparar pengar på att använda ytterligare en licens.

## Administrering {#administration}

* **[Formulärvalideringsregler](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Behåll databasens hälsotillstånd och blockera problematiska eller oönskade e-postdomäner från att skicka Marketo Engage-formulär. På panelen Valideringsregel för globala formulär kan administratörer definiera en blockeringslista eller aktivera en fördefinierad lista med kostnadsfria konsumentdomäner som ska blockeras från formulär.

* **[Landing Page Header Security](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Administratörer kan hantera rubrikerna Strict Transport Security och X-Frame Options på sina landningssiddomäner för att upprätthålla höga säkerhetskrav.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## AEP Marketo Engage Destination Connector - Skapa nya leads {#aep-marketo-engage-destination-connector}

Marketo Engage-kunder som också använder Adobe Experience Platform (AEP) kan maximera sin databas genom att överföra nya personposter till Marketo Engage från AEP via AEP målanslutning. När du skickar målgruppssegment från AEP till Marketo Engage kan personer i segmentet som inte redan finns i din Marketo Engage-databas [automatiskt läggas till i det](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

**[!DNL Sales Insight]för [!DNL Salesforce] CRM**

* **Ny typkolumn för[!UICONTROL Best Bets]**: Säljarna får snabbare insikter med en ny kolumn med namnet&quot;Typ&quot; för att skilja mellan leads och kontakter på sidan [!UICONTROL Best Bets].

* **[!DNL Salesforce]API-uppdatering för plattform**: Som svar på [!DNL Salesforce] att [!DNL Salesforce] API-version 21.0 till 30.0 tagits bort har [!DNL Sales Insight]-paketet uppdaterats med de senaste API:erna.

* **Uppdaterad profilering**: Alla [!DNL Sales Insight] sidor uppdateras för att passa Adobe branding.

**[!DNL Sales Insight]för[!DNL Microsoft Dynamics]**

* **Uppdaterad kontolayout**: Säljarna kan få en samlad vy över de viktigaste aktiviteterna, till exempel e-postaktiviteter, webbaktiviteter, intressanta ögonblick och poängändringar för alla kontakter i ett konto.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Anropsresultat och orsaker**: Förstå och spåra säljteamets utgående satsningar mer i detalj med nya, helt anpassningsbara alternativ för samtalsresultat och samtalsorsaker. Förutom dessa nya fält introducerar vi nya styrfunktioner för att framtvinga val av anropsorsak och -resultat medan säljarna gör samtal, ny styrning för att aktivera eller inaktivera samtalsorsaker och -resultat samt ett nytt anpassat aktivitetsfält för Anropsorsak och samtalsresultat [!DNL Salesforce] för att logga data på [!DNL Salesforce]. [Klicka här](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) om du vill veta mer.

* **[!DNL Salesforce]Anpassning av aktivitetsdetalj**: Hämta fler försäljningsaktivitets- och aktivitetsdata i [!DNL Salesforce] genom att anpassa vilken information som läggs till i [!DNL Salesforce]-aktivitetens ämnesfält när en försäljningsaktivitet loggas till [!DNL Salesforce] från [!DNL Sales Connect]. [Klicka här](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) om du vill veta mer.

## Meddelanden {#announcements}

* **Borttagning av Marketo Sky**: I mars kommer Marketo Sky inte längre att vara tillgängligt eftersom vi fokuserar våra resurser på att leverera nästa generations användarupplevelser. I ett försök att behålla åtkomsten till funktioner som är exklusiva för Marketo Sky idag kommer vi att ta med Åsidosättning av förfallodatum och prioritet för smarta kampanjer i den vanliga upplevelsen i mars. [Klicka här](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) om du vill veta mer.

* **Borttagning av formulärslutpunkter**: Programatiska POST-värden för leadCapture/save2-slutpunkten stöds inte av Marketo Engage-formulär. [Klicka här](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) om du vill veta mer.

* **Inloggning i dialogrutan Bjud in användare**: I mars kommer den befintliga valfria funktionen Inbjudan till användare att bli inaktuell. Funktionen [!UICONTROL Login in Invite User Dialog] åsidosätts av funktionen Universal ID, som krävs för den kommande systemintegrationen i Adobe Identity Management och som aktiverades i augusti 2021 för alla prenumerationer. Som ett resultat av borttagningen tvingar Marketo Engage endast en användare att kopplas per e-postadress inom en prenumeration.

**Marketo Engage-domäner - [!DNL Sales Insight] Konfiguration**: För Marketo Engage-domäner som inte har ett SSL-certifikat aktiverat och https://, misslyckas anropen med ett SSL-handskakningsfel. Därför kommer dessa domäner att upphöra. Därför kan [!DNL Sales Insight] användare med en äldre konfiguration som pekar på någon av dessa domäner råka ut för bildtextfel på sin Lead-, Kontakt-, Konto-, Affärsmöjlighetspaneler- eller Marketo Global-sida. Vi rekommenderar att du uppdaterar din [Marketo Engage-konfiguration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) i [!DNL Salesforce] om det här felet inträffar. Du behöver bara uppdatera Marketo Engage-autentiseringsuppgifter som är markerade i avsnittet [!DNL Marketo Sales Insight]-konfiguration i dokumentet.

**_Webbseminarium om produktreleaser_**

[Januari 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
