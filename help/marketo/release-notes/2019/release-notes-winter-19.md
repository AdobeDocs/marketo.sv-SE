---
unique-page-id: 17727823
description: Versionsinformation -vinter '19 - Marketo Docs - Produktdokumentation
title: Versionsinformation -vinter '19
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# Versionsinformation: Vintern &#39;19 {#release-notes-winter}

Följande funktioner finns i vinterversionen 19. Se om din Marketo-utgåva har funktioner tillgängliga.

Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion, om sådana finns.

>[!NOTE]
>
>Facebook behöver nu ett Business Manager-konto för att kunna utnyttja din anpassade målgruppsintegrering. Din startpunktstjänst för Facebook *måste* kopplas till ett Business Manager-konto, annars kommer **integreringen inte att fungera efter 14 januari 2019**. Information om hur du skapar ett Business Manager-konto finns i [Facebook-hjälpen](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft uppmanar alla onlinekunder att uppgradera till den senaste versionen av Microsoft Dynamics. Om du integrerar din Marketo-instans med Dynamics Online måste du [uppgradera till den senaste versionen av Marketo-lösningen](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md) före den 31 **januari 2019** för att vara säker på att integreringen fortsätter att fungera.

>[!NOTE]
>
>Marketo uppgraderar OAuth-versionen för GoToWebinar från 1.0 till 2.0. Stödet för OAuth 1.0 kommer att upphöra i januari 2019. Om du använder GoToWebinar måste du autentisera dina inloggningar via LaunchPoint (i administrationsområdet) senast den 31 **januari 2019** för att integreringen ska fortsätta. Mer information finns på vår [communitysida](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Förbättringar av kärnplattformen {#core-platform-enhancements}

** [Email CC for Marketo Emails](../../product-docs/email-marketing/general/email-cc.md)**

Inkludera upp till fem CC-adresser per mottagare i e-postmeddelanden som skickas via Marketo.

**API**

* **Stöd för flera domäner för resurs-API:** Godkännande och kloning av resurser ger samma resultat i API:t och användargränssnittet.
* **Stöd för e-post-CC för resurs-API**: Användare som klonar, godkänner och bearbetar e-postmeddelanden via API:t behåller pariteten med gränssnittsinställningarna.

** [Munchkin v155 (beta)](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Endast API-läge**: Användarna kan nu bestämma när och hur de ska spåra medlemmar i sina databaser genom att tillåta att enkelsidiga webbappar uttryckligen anropar när de vill spela in en webbsida, istället för att förlita sig på Marketos automatiska spårning.
* **Hantering** av avanmälan: Hantera enkelt avanmälningar genom att matcha avanmälningsdomänen med Munchkins cookie-domän för spårning.
* **Domännivåbestämningsparameter**: Domäner med två bokstäver (dvs. &quot; [website.io](http://website.io)&quot;) spåras automatiskt i Marketo utan ytterligare installationskrav.

## Marketo Sales Engage {#marketo-sales-engage}

* **Anpassad Salesforce-profil**: Sales Engage har nu stöd för ett obegränsat antal anpassade profiler.

* **Salesforce-anpassning**: Genom att ta bort icke-kritiska anpassade aktivitetsfält kan användarna konfigurera säljengagemanget på CRM-plattformen mer effektivt.
* **E-posttjänst**: Få bättre levererbarhet och förbättrad svarsspårning, funktioner för schemalagd e-post och massutskick genom att ansluta till Microsoft Outlook (antingen via Office365 eller On-Prem via fliken E-postanslutning).
* **Nya administratörsinställningar**: Två administratörssidor har lagts till för att optimera din instans av Sales Engage

   * *Teamhantering* stöder en smidig process för kontokonfiguration genom att tillåta administratörer att redigera prenumerationer och team.
   * *Salesforce Admin Settings* hjälper team att konfigurera sin SFDC-synkronisering snabbare och enklare än någonsin.

* **OWA-plugin för Windows**: Med ett enda tillägg stöds alla Windows Office365-klienter i Sales Engage, vilket ger möjlighet att använda Live Feed i Outlook. Det nya plugin-programmet kommer att vara tillgängligt i Microsoft Store.
* **Aktivitetspublicering**: Synkronisera säljengagemanget med kärnplattformen Marketo för att utnyttja marknadsföringsinsikter i realtid.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Skyar släpps oftare. Följande funktioner och förbättringar förväntas släppas under det sista kvartalet/början av första kvartalet. Mer information och uppdateringar finns i vår [Sky-dokumentation](https://help.marketo.com/hc/en-us/articles/360012858573).

* **Valfri standardupplevelse**: Marketo-användare kan ange Marketo Sky som standardupplevelse om de har fått åtkomst av en administratör.

* **Omdesignad My Marketo**: Anpassa upplevelsen genom att lägga till widgetar som ger viktig information, meddelanden och länkar till de områden du besöker mest.

* **Design Studio - listvyer och detaljsidor**: Få bättre ordning och precision med filterbara och sökbara listvyer av mejl, landningssidor och formulär. På tillgångsinformationssidor finns viktig information om varje resurs, inklusive vilka program resursen används av, antalet utdrag som används och mycket annat.

* **Global sökning**: Marketo erbjuder nu en snabbare och robustare global sökfunktion på hela plattformen. Sökfrågor körs nu på alla tillgängliga arbetsytor och kan söka efter resurser (både aktiva och arkiverade), etiketter, kampanjer och program. Sökresultaten tillhandahålls via en övertäckning och varje resultat innehåller filplatshistoriken som anger var resursen finns.

* **Förbättrat användargränssnitt**: Nya ikoner, moduler och knappar, tillsammans med en ny färgpalett som speglar vår varumärkesuppdatering och gör Marketo Skyn ännu mer enastående och funktionell.

* **Förbättringar av e-postprogrammets användbarhet**: Vi fortsätter att gå mot en paritet i e-postprogrammens funktionalitet mellan vår klassiska Marketo Lead Management-plattform och den nya Marketo Skyn.
* **Event-With-Webinar-program**: Event-With-Webinar-program finns nu i Marketo Sky (Obs! endast GoToWebinar stöds i den här versionen med ytterligare integreringar som upprättas över tid).

## Kontobaserad marknadsföring {#account-based-marketing}

** [ABM Personabaserad segmentering och filtrering](../../product-docs/account-based-marketing/using-personas.md)**

Anpassa era ABM-kampanjer för specifika personer i namngivna konton. Funktionen ABM Persona skapar en standardjobbtitel baserad på leadsegmentering och tillåter konfiguration av ytterligare persona segmenteringar.

## Analyser {#analytics}

**Bizible**

* **Anpassade beräkningsfält**: Använd valfritt Bizible-attribut för att skapa anpassade fält som kan användas för instrumentpanelsrapportering och segmentering.

* **SOC II Type II-certifiering**: Ny certifiering av säkerhet och integritet bygger på typ I-ackreditering från tidigare i år.

## Webbanpassning {#web-personalization}

**[Lägg till underdomäner i kontoinställningar](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

För att hantera domäner och underdomäner effektivare kan användare nu lägga till underdomäner i sina RTP-kontoinställningar.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Uppdaterat MME Software Development Kit (SDK) för Android**

Vi har uppdaterat vårt SDK för Android till ett modernare, stabilare och skalbart ramverk som innehåller större flexibilitet och nya ingenjörsfunktioner. Apputvecklare för Android kan nu direkt använda Googles FCM ( [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) ) med denna nya SDK.

* [Utvecklarinstruktioner](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Frågor och svar för utvecklare](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Programutvecklare **måste** uppdatera till den nya versionen före den 31 mars 2019. Om du inte uppdaterar din SDK senast 31 mars 2019 kommer nya användare som hämtar din app efter detta datum inte att kunna få push-meddelanden förrän du uppdaterar till den senaste versionen av SDK. SDK-uppdateringen kräver inte att dina nuvarande mobilappsanvändare hämtar en ny version av din app.

## Ytterligare uppdateringar {#additional-updates}

**Extensible Webinar Platform**

Förutom vår produktrelease arbetar vårt partnerteam på ett nytt ramverk som gör det möjligt för webbinarier-leverantörer att bygga och underhålla sina egna integreringar med Marketo, vilket ger större flexibilitet när det gäller att uppdatera och förbättra sina lösningar och samtidigt ger marknadsförarna möjlighet att få ut så mycket som möjligt av de integreringar de valt.

Vi planerar att lansera vår nya plattform med leverantörer från fall till fall. Mer information finns i vår [programinformation](https://www.marketo.com/why-marketo/partners/technology/) eller kontakta er Marketkontakt.
