---
description: Versionsinformation - augusti 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - augusti 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Versionsinformation: augusti 2021 {#release-notes-aug-21}

Följande funktioner finns i versionen från 21 augusti. Se om det finns funktioner i Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta Adobe Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den **20 augusti 2021**.

## Experience Automation {#experience-automation}

* **Marketo Engage-användarautentisering via Adobe-identitet**: Snart kommer nya Marketo Engage-användare med Enterprise-paket att registreras med Adobe ID användarautentiseringsuppgifter. Migrering av nuvarande användare till det integrerade identitetssystemet kommer inte att ske förrän i mitten av 2022 och inga åtgärder krävs förrän ytterligare varningar skickas. Med Adobe ID-användarautentisering kan IT-/säkerhetsadministratörer hantera flera Marketo Engage-produktinstanser tillsammans med andra Experience Cloud-lösningar samt konfigurera enkel inloggning via en gemensam konsol. Administratörer kan enkelt hantera användargrupper och användarrättigheter på ett och samma ställe.

* **Körbar kampanjkapsling**: Körbara kampanjer kan nu även anropa andra körbara kampanjer så att du kan kapsla in dem på upp till tre nivåer. Detta möjliggör ytterligare konsolidering av vanliga driftsflöden och förbättrar hanteringen av smarta kampanjer.

* **Åtgärd för enstaka flöde på personinformationssidan** (tillgänglig senast 9 september): Kör flödesåtgärder som att skicka e-post, ändra ägare eller någon annan smart kampanjåtgärd för enskilda personer från personinformationssidan med hjälp av flödesåtgärdsmenyn utan att växla till databasstödrastervyn.

* **[Export av anpassade aktiviteter](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Export av metadata har nu stöd för alla objekt och metadata som kan användas för att dela, analysera och utforma din prenumerationsdatamodell.

## API-förbättringar {#api-enhancements}

* **Skicka formulär-API**: När en e-postadress dupliceras i två eller flera lead-poster uppdaterar vi den senast uppdaterade posten i stället för att hoppa över helt. Ger paritet med Forms 2.0 API.

* **E-post-API:t**: Hämta e-postresurser för mästare eller utmanare. Hämta e-postresurser med datumintervallfilter.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **Förbättrad synlighet i lead-, kontakt-, konto- och säljprojektsaktiviteter för Salesforce CRM-användare**: Engagemang med potentiella kunder under långa försäljningscykler är mer informerat på grund av ett ökat antal engagemangsposter i [!DNL Sales Insight]. Intressanta ögonblick, webbaktivitet, e-post och poängflikar visar upp till 400 aktiviteter i objekten Lead, Kontakt, Konto och säljprojekt.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Begränsning av e-postanslutning (Beta)**: Förbättra e-postleveransen och skala personlig försäljningskommunikation med e-postanslutningsbegränsning för Sales Connect. Den nya tekniken hanterar automatiskt e-posttajmning för att skapa sömlösa upplevelser för [!DNL Exchange]- och Gmail-användare. Minska eller eliminera användningen av massutskick av e-postprogram från tredje part och skicka alla dina e-postmeddelanden från [!DNL Sales Connect] utan problem.

>[!NOTE]
>
>E-postbegränsning finns i Beta nu. [Läs mer](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Förbättrade insikter om försäljningsaktivitet**: Hämta och aktivera personaliserat engagemang baserat på ditt säljteams tidigare aktiviteter. Nya attribut som länken Försäljningssamtalsinspelning, Försäljningskampanjnamn och E-postärende kan användas i Marketo Engage smarta listor.  Dessa aktiviteter kan exporteras och rapporteras via Marketo Engage REST API eller gruppexport och är tillgängliga för filter och utlösare som ytterligare begränsningar för smarta listor.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn] Lead Gen Forms-integrering**: Nu kan marknadsförare utföra intäktsattribuering på konverteringar som inträffar när [!DNL LinkedIn] hämtar formulär genom sina Lead Gen Forms-annonsenheter. Dessa insikter kan sedan användas för att optimera formulärprestanda och investeringar i betalda medier. [!DNL LinkedIn] Lead Gen Forms är ett av [!DNL LinkedIn]s snabbast växande betalmediepresentationer och denna nya funktion ingår i vår befintliga [!DNL LinkedIn] Ads-integrering med [!DNL Bizible].

* **Förbättrad snabbkontrollpanel**: Vi har lagt till ett nytt snabbmätnings- och instrumentpanelsfilter för djupare insikter. Den här instrumentpanelen används av marknadsförare för att förstå hur snabbt leads och affärstillfällen kan komma i fas för steg och hur effektiva olika former av marknadsföring och säljengagemang är.

* **Ny kohort Waterfall Journey-instrumentpanel**: Detta gör att marknadsförarna kan se förloppet för en vald kohort genom en klassisk uppsättning efterfrågansvattenfall, vilket ger en snabb förståelse för konverteringsgrader och underförstådda stegvisa konverteringsorsaker på scen-för-steg-basis.

## [!DNL Bizible]-integrering med Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Det här avsnittet innehåller nya funktioner för användare av Bizible som har slutfört migreringen av Adobe Identity Management System (IMS). Om du har migrerats visas ditt nya Adobe ID i [!DNL Bizible]-inställningarna på fliken Adobe ID. Alla konton bör migreras före slutet av 2021.

* **[!DNL Bizible]Integrering med Adobe Privacy Service** (tillgängligt i september 2021): Integreringen av [!DNL Bizible] med Adobe Privacy Service centraliserar kompatibiliteten med viktiga sekretessregler (som GDPR) för Adobe Experience Cloud-program. Du kan nu utnyttja den här tjänsten och hantera alla sekretessförfrågningar centralt så att ändringsförfrågningar som kommer in i [!DNL Bizible] och andra Adobe-produkter återspeglas i alla program.

* **[!DNL Bizible]i Adobe Unified Shell**: [!DNL Bizible] När Adobe Unified Shell används får användarna nya funktioner som visas i programmets namnlist i [!DNL Bizible] och som ger bättre åtkomst till supportresurser och programväxling. Adobe Unified Shell hjälper dig att skapa en konsekvent upplevelse mellan [!DNL Bizible] och andra Adobe Experience Cloud-program.

* **[!DNL Bizible]Domänägarskap och självhantering**: [!DNL Bizible] -användare kan använda Adobe Admin Console för att hantera de domäner som de vill att [!DNL Bizible] ska spåra. Detta ger självbetjäning till en tidigare manuell process och ger en konsekvent upplevelse av hur domänägarskap och spårning hanteras i Adobe Experience Cloud-program.

## Meddelanden {#announcements}

* **Uppdatera till universella ID-inställningar för prenumeration**: Alla Marketo Engage-prenumerationer kommer att vara enhetliga när det gäller stöd för universella ID för att ge stöd för kommande Marketo Engage- och Adobe Identity-integrering för befintliga användare. Mer information [finns här](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webbseminarium om produktreleaser_**

[Augusti 2021 Marketo Engage Release Webinar](https://engage.marketo.com/August21_Release_Webinar.html)
