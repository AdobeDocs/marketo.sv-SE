---
description: Versionsinformation - augusti 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - augusti 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 7a062683a3c38d8765eb966041bf7ee3db665f5a
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Versionsinformation: Augusti 2021 {#release-notes-aug-21}

Följande funktioner finns i versionen från 21 augusti. Se om det finns funktioner i Marketo Engage.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta Adobe Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den **20 augusti 2021**.

## Experience Automation {#experience-automation}

* **Autentisering av Marketo Engage via Adobe-identitet**: Snart kommer nya Marketo Engage-användare med Enterprise-paket att anställas med Adobe ID inloggningsuppgifter. Migrering av nuvarande användare till det integrerade identitetssystemet kommer inte att ske förrän i mitten av 2022 och inga åtgärder krävs förrän ytterligare varningar skickas. Autentisering av användare med Adobe-identitet gör det möjligt för IT-/säkerhetsadministratörer att hantera flera produktinstanser av Marketo Engage tillsammans med andra Experience Cloud-lösningar samt konfigurera enkel inloggning via en gemensam konsol. Administratörer kan enkelt hantera användargrupper och användarrättigheter på ett och samma ställe.

* **Körbar kampanjkapsling**: Körbara kampanjer kan nu även anropa andra körbara kampanjer så att ni kan kapsla dem på upp till tre nivåer. Detta möjliggör ytterligare konsolidering av vanliga driftsflöden och förbättrar hanteringen av smarta kampanjer.

* **Enkelflödesåtgärd på personinformationssidan** (Tillgänglig den 9 september): Kör flödesåtgärder som att skicka e-post, ändra ägare eller någon annan smart kampanjåtgärd för enskilda personer från sidan med personinformation med hjälp av flödesåtgärdsmenyn utan att växla till databasrutnätsvyn.

* **[Exportera anpassade aktiviteter](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Export av metadata har nu stöd för alla objekt och metadata som kan användas för att dela, analysera och utforma din prenumerationsdatamodell.

## API-förbättringar {#api-enhancements}

* **Skicka formulär-API**: När en e-postadress dupliceras i två eller flera Lead-poster uppdaterar vi posten&quot;senast uppdaterad&quot; i stället för att hoppa över helt. Ger paritet med Forms 2.0 API.

* **E-post-API**: Hämta e-postresurser för mästare eller utmanare. Hämta e-postresurser med datumintervallfilter.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **Förbättrad synlighet för Salesforce CRM-användare vad gäller lead-, kontakt-, konto- och säljprojektsaktiviteter**: Engagemang med potentiella kunder under långa säljcykler blir mer välinformerat på grund av ett ökat antal engagemangsposter i Sales Insight. Intressanta ögonblick, webbaktivitet, e-post och poängflikar visar upp till 400 aktiviteter i objekten Lead, Kontakt, Konto och säljprojekt.

## Sales Connect {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Begränsning av e-postanslutning (beta)**: Förbättra e-postleveransen och skräddarsy skräddarsydd säljkommunikation med e-postanslutningsbegränsning för Sales Connect. Den nya tekniken hanterar automatiskt e-posttajmning för att skapa sömlösa upplevelser för Exchange- och Gmail-användare. Minska eller eliminera användningen av massutskick av e-postprogram från tredje part och skicka alla e-postmeddelanden från Sales Connect utan problem.

>[!NOTE]
>
>E-postbegränsning finns nu i Beta. [Läs mer](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Förbättrade insikter om försäljningsaktivitet**: Hämta in och aktivera personaliserat engagemang baserat på säljteamets tidigare aktiviteter. Nya attribut som länken Försäljningssamtalsinspelning, Försäljningskampanjnamn och E-postärende kan användas i smarta listor i Marketo Engage.  Dessa aktiviteter kan exporteras och rapporteras via Marketo Engage REST API eller gruppexport och är tillgängliga för filter och utlösare som ytterligare begränsningar för smarta listor.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms Integration**: Nu kan marknadsförarna lägga in intäkter på konverteringar som görs när LinkedIn hämtar blanketter genom sina Lead Gen Forms-annonsenheter. Dessa insikter kan sedan användas för att optimera formulärprestanda och investeringar i betalda medier. linkedIn Lead Gen Forms är ett av LinkedIn snabbast växande betalmediepresentationer och denna nya funktion ingår i vår befintliga LinkedIn Ads-integrering med Bizible.

* **Snabbare instrumentpanel**: Vi har lagt till ett nytt snabbmätningsfilter och kontrollpanelsfilter för djupare insikter. Den här instrumentpanelen används av marknadsförare för att förstå hur snabbt leads och affärstillfällen kan komma i fas för steg och hur effektiva olika former av marknadsföring och säljengagemang är.

* **New Cohort Waterfall Journey Dashboard**: På så sätt kan marknadsförarna se utvecklingen i en utvald kohort genom en klassisk&quot;demand waterfall&quot;-uppsättning stadier, vilket ger en snabb förståelse för konverteringsgrader och underförstådda konverteringsfaktorer steg för steg.

## Bizibel-integrering med Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Det här avsnittet innehåller nya funktioner för användare av Bizible som har slutfört migreringen av Adobe Identity Management System (IMS). Om du har migrerats visas din nya Adobe ID i Bizible Settings under fliken Adobe ID. Alla konton bör migreras före slutet av 2021.

* **Bizibel-integrering med Adobe Privacy Service** (tillgängligt i september 2021): Bizibelns integrering med Privacy Servicen Adobe centraliserar efterlevnaden av viktiga sekretessbestämmelser (som GDPR) för Adobe Experience Cloud-program. Du kan nu utnyttja den här tjänsten och hantera alla sekretessförfrågningar centralt så att ändringsförfrågningar som kommer in i Bizible och andra Adobe-produkter återspeglas i alla program.

* **Bizible on Adobe Experience Cloud Interface**: Bizibles användning av Adobe Experience Cloud Interface ger användarna nya funktioner som kommer att visas i det Bizible-baserade programrubrikfältet och ger bättre åtkomst till supportresurser och programväxling. Gränssnittet Experience Cloud hjälper till att skapa en enhetlig upplevelse mellan Bizible och andra Adobe Experience Cloud-program.

* **Bizible Domain Ownership and Self Management**: Bizibla användare kan använda Adobe Admin Console för att hantera de domäner de vill att Bizible ska spåra. Detta ger självbetjäning till en tidigare manuell process och ger en konsekvent upplevelse av hur domänägarskap och spårning hanteras i olika Adobe Experience Cloud-program.

## Meddelanden {#announcements}

* **Uppdatera till inställningar för Universal ID för prenumeration**: För att ge stöd åt integreringen av Marketo Engage och Adobe-identitet för befintliga användare kommer alla Marketo Engage-prenumerationer att vara enhetliga i aktiveringen av stöd för universella ID. Mer information [finns här](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Product Release Webinar_**

[Webbinarium om Marketo Engage från augusti 2021](https://engage.marketo.com/August21_Release_Webinar.html)
