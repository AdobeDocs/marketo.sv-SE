---
unique-page-id: 17727823
description: Versionsinformation -vinter '19 - Marketo Docs - produktdokumentation
title: Versionsinformation -vinter '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Versionsinformation: Vinter 19 {#release-notes-winter}

Följande funktioner finns i vinterversionen 19. Se om det finns funktioner i Marketo Edition.

Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion, om sådana finns.

>[!NOTE]
>
>[!DNL Facebook] behöver nu ett Business Manager-konto för att kunna utnyttja din anpassade målgruppsintegrering. [!DNL Facebook]-startpunktstjänsten *måste* kopplas till ett Business Manager-konto, annars kommer **integreringen inte att fungera efter 14 januari 2019**. Mer information om hur du konfigurerar ett Business Manager-konto finns i [[!DNL Facebook] hjälpen](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft uppmanar alla onlinekunder att uppgradera till den senaste versionen av [!DNL Microsoft Dynamics]. Om du integrerar din Marketo-instans med [!DNL Dynamics Online] måste du [uppgradera till den senaste versionen av Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) före **31 januari 2019** för att vara säker på att integreringen fortsätter att fungera.

>[!NOTE]
>
>Marketo uppgraderar OAuth-versionen för GoToWebinar från 1.0 till 2.0. Stödet för OAuth 1.0 kommer att upphöra i januari 2019. Om du använder GoToWebinar måste du autentisera dina inloggningar via LaunchPoint (i administrationsområdet) senast den **31 januari 2019** för att integreringen ska fortsätta. Mer information finns på vår [communitysida](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Förbättringar av kärnplattformen {#core-platform-enhancements}

**[E-post för CC för Marketo-e-post](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Inkludera upp till fem CC-adresser per mottagare i e-postmeddelanden som skickas via Marketo.

**API**

* **Stöd för domäner med flera varumärken för resurs-API:** Godkännande och kloning av resurser ger samma resultat i API:t och användargränssnittet.
* **Stöd för e-post i CC för resurs-API**: Användare som klonar, godkänner och bearbetar e-post via API:t behåller pariteten med gränssnittsinställningarna.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Läge endast för API**: Användare kan nu bestämma när och hur de ska spåra medlemmar i sina databaser genom att tillåta att enkelsidiga webbprogram anropar när de vill spela in en webbsida, istället för att förlita sig på Marketo automatiska spårning.
* **Avanmälningshantering**: Hantera enkelt avanmälningar genom att matcha den avanmälda cookie-domänen med den [!DNL Munchkin] spårande cookie-domänen.
* **Domännivåbestämningsparameter**: Domäner med två bokstäver (d.v.s. [website.io](https://website.io)) spåras automatiskt i Marketo utan ytterligare konfigurationskrav.

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]Anpassad profil**: Försäljningsengagemanget har nu stöd för ett obegränsat antal anpassade profiler.

* **[!DNL Salesforce]Anpassning**: Genom att ta bort icke-kritiska anpassade aktivitetsfält kan användare konfigurera försäljningsengagemanget på CRM-plattformen mer effektivt.
* **E-posttjänst**: Få bättre levererbarhet och förbättrad svarsspårning, funktioner för schemalagd e-post och massutskick av e-post genom att ansluta till [!DNL Microsoft Outlook] (antingen via Office365 eller på plats via fliken E-postanslutning).
* **Nya administratörsinställningar**: Två administratörssidor har lagts till för att optimera försäljningsengagemangsinstansen

   * *Teamhantering* stöder en smidig kontokonfigurationsprocess genom att tillåta administratörer att redigera prenumerationer och team.
   * *Med Salesforce Admin Settings* kan team konfigurera sina SFDC-synkroniseringar snabbare och enklare än någonsin.

* **OWA-plugin för[!DNL Windows]**: Med ett enda tillägg stöds alla [!DNL Windows Office365]-klienter i Sales Engage, vilket ger möjlighet att använda Live Feed i Outlook. Det nya plugin-programmet finns i Microsoft Store.
* **Activity Pusher**: Synkronisera Sales Engage med Marketo huvudplattform för att utnyttja marknadsföringsinsikter i realtid.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky] versioner inträffar oftare. Följande funktioner och förbättringar förväntas släppas under det sista kvartalet/början av första kvartalet. Mer information och uppdateringar finns i [Sky-dokumentationen](https://help.marketo.com/).

* **Valfri standardupplevelse**: Marketo-användare kan ange [!DNL Marketo Sky] som standardupplevelse om de har fått åtkomst av en administratör.

* **Förnyad Min Marketo**: Anpassa din upplevelse genom att lägga till widgetar som ger viktig information, meddelanden och länkar till de områden du besöker mest.

* **Design Studio - listvyer och detaljsidor**: Få bättre ordning och precision med filterbara och sökbara listvyer av e-postmeddelanden, landningssidor och formulär. På tillgångsinformationssidor finns viktig information om varje resurs, inklusive vilka program resursen används av, antalet utdrag som används och mycket annat.

* **Global sökning**: Marketo erbjuder nu en snabbare och robustare global sökfunktion på hela plattformen. Sökfrågor körs nu på alla tillgängliga arbetsytor och kan söka efter resurser (både aktiva och arkiverade), etiketter, kampanjer och program. Sökresultaten tillhandahålls via en övertäckning och varje resultat innehåller filplatshistoriken som anger var resursen finns.

* **Förbättrat användargränssnitt**: Nya ikoner, moduler och knappar, tillsammans med en ny färgpalett som speglar vår varumärkesuppdatering och gör [!DNL Marketo Sky] ännu mer enastående och funktionellt.

* **Förbättringar av e-postprogrammets användbarhet**: Vi fortsätter att gå mot en paritet i e-postprogrammets funktionalitet mellan vår klassiska Marketo Lead Management-plattform och den nya [!DNL Marketo Sky] -upplevelsen.
* **Event-With-Webinar-program**: Event-With-Webinar-program är nu tillgängliga i [!DNL Marketo Sky] (Obs! Endast GoToWebinar stöds i den här versionen, med ytterligare integreringar upprättade över tid).

## Account-Based Marketing {#account-based-marketing}

**[ABM Personabaserad segmentering och filtrering](/help/marketo/product-docs/target-account-management/using-personas.md)**

Anpassa era ABM-kampanjer för specifika personer i namngivna konton. Funktionen ABM Persona skapar en standardjobbtitel baserad på leadsegmentering och tillåter konfiguration av ytterligare persona segmenteringar.

## Analytics  {#analytics}

**[!DNL Bizible]**

* **Anpassade beräknade fält**: Använd valfritt [!DNL Bizible]-attribut för att skapa anpassade fält som kan användas för instrumentpanelsrapportering och segmentering.

* **SOC II Type II-certifiering**: Ny säkerhets- och sekretesscertifiering bygger på Type I-ackreditering från tidigare i år.

## [!DNL Web Personalization] {#web-personalization}

**[Lägg till underdomäner i kontoinställningarna](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

För att hantera domäner och underdomäner effektivare kan användare nu lägga till underdomäner i sina RTP-kontoinställningar.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Uppdaterat MME Software Development Kit (SDK) för Android**

Vi har uppdaterat vår SDK för Android till ett modernare, stabilare och skalbart ramverk som innehåller större flexibilitet och nya tekniska funktioner. Android apputvecklare kan nu direkt använda Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) med denna nya SDK.

* [Utvecklarinstruktioner](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Frågor och svar om utvecklare](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Programutvecklare **måste** uppdatera till den nya versionen före den 31 mars 2019. Om du inte uppdaterar din SDK senast den 31 mars 2019 kommer nya användare som hämtar din app efter detta datum inte att kunna få push-meddelanden förrän du uppdaterar till den senaste versionen av SDK. SDK-uppdateringen kräver inte att dina nuvarande mobilappsanvändare hämtar en ny version av din app.

## Ytterligare uppdateringar {#additional-updates}

**Plattform för utbyggbart webbinarium**

Förutom vår produktrelease arbetar vårt partnerteam på ett nytt ramverk som gör det möjligt för webbinarier-leverantörer att bygga och underhålla sina egna integreringar med Marketo, vilket ger större flexibilitet när det gäller att uppdatera och förbättra sina lösningar och samtidigt ger marknadsförarna möjlighet att få ut så mycket som möjligt av de integreringar de valt.

Vi planerar att lansera vår nya plattform med leverantörer från fall till fall. Mer information finns i vår [programinformation](https://www.marketo.com/why-marketo/partners/technology/) eller kontakta din Marketo-kontakt.
