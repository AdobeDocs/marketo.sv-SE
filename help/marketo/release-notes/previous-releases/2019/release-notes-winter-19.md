---
unique-page-id: 17727823
description: Versionsinformation -vinter '19 - Marketo Docs - produktdokumentation
title: Versionsinformation -vinter '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Versionsinformation: Vintern &#39;19 {#release-notes-winter}

Följande funktioner finns i vinterversionen 19. Se om det finns funktioner i din Marketo-utgåva.

Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion, om sådana finns.

>[!NOTE]
>
>Facebook behöver nu ett Business Manager-konto för att kunna utnyttja er anpassade målgruppsintegrering. Din Facebook LaunchPoint-tjänst *måste* associeras med ett Business Manager-konto eller **integreringen inte längre fungerar efter 14 januari 2019**. Om du vill konfigurera ett Business Manager-konto går du till [Hjälp om facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft uppmanar alla onlinekunder att uppgradera till den senaste versionen av Microsoft Dynamics. Om du integrerar din Marketo-instans med Dynamics Online måste du [uppgradera till den senaste versionen av Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) före **31 januari 2019** för att säkerställa att integreringen fortsätter att fungera.

>[!NOTE]
>
>Marketo uppgraderar OAuth-versionen för GoToWebinar från 1.0 till 2.0. Stödet för OAuth 1.0 kommer att upphöra i januari 2019. Om du använder GoToWebinar måste du autentisera dina inloggningar på nytt via LaunchPoint (i administrationsområdet) med **31 januari 2019** för att säkerställa att integreringen fortsätter att fungera. Mer information finns i [Community-sida](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Förbättringar av kärnplattformen {#core-platform-enhancements}

**[Email CC for Marketo e-mail](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Inkludera upp till fem CC-adresser per mottagare i e-postmeddelanden som skickas via Marketo.

**API**

* **Stöd för flera domäner för resurs-API:** Godkännande och kloning av resurser ger samma resultat i API:t och användargränssnittet.
* **Stöd för e-post-CC för resurs-API**: Användare som klonar, godkänner och bearbetar e-postmeddelanden via API:t behåller pariteten med gränssnittsinställningarna.

**[Munchkin v155 (beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Läge med endast API**: Användarna kan nu bestämma när och hur de ska spåra medlemmar i sina databaser genom att tillåta att enkelsidiga webbappar uttryckligen anropar när de vill spela in en webbsida, istället för att förlita sig på Marketo automatiska spårning.
* **Hantering av avanmälan**: Hantera enkelt avanmälningar genom att matcha avanmälningsdomänen med Munchkins cookie-domän för spårning.
* **Domännivåbestämningsparameter**: Domäner med två bokstäver (dvs. &quot; [website.io](https://website.io)&quot;) spåras automatiskt i Marketo utan ytterligare installationskrav.

## Marketo Sales Engage {#marketo-sales-engage}

* **Anpassad profil för Salesforce**: Sales Engage har nu stöd för ett obegränsat antal anpassade profiler.

* **Salesforce-anpassning**: Genom att ta bort icke-kritiska anpassade aktivitetsfält kan användarna konfigurera säljengagemanget på CRM-plattformen mer effektivt.
* **E-posttjänst**: Få bättre levererbarhet och förbättrad svarsspårning, funktioner för schemalagd e-post och massutskick genom att ansluta till Microsoft Outlook (antingen via Office365 eller On-Prem via fliken E-postanslutning).
* **Nya administratörsinställningar**: Två administratörssidor har lagts till för att optimera din instans av Sales Engage

   * _Teamhantering_ har stöd för en smidig process för kontokonfiguration genom att administratörer kan redigera prenumerationer och team.
   * _Administratörsinställningar för Salesforce_ hjälper team att konfigurera sin SFDC-synkronisering snabbare och enklare än någonsin.

* **OWA-plugin för Windows**: Med ett enda tillägg stöds alla Windows Office365-klienter i Sales Engage, vilket ger möjlighet att använda Live Feed i Outlook. Det nya plugin-programmet finns i Microsoft Store.
* **Verksamhetspublicering**: Synkronisera säljengagemanget med Marketo kärnplattform för att utnyttja marknadsföringsinsikter i realtid.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Skyar släpps oftare. Följande funktioner och förbättringar förväntas släppas under det sista kvartalet/början av första kvartalet. Mer information och uppdateringar finns i [Sky-dokumentation](https://help.marketo.com/).

* **Valfri standardupplevelse**: Marketo-användare kan ange Marketo Sky som standardupplevelse om de har fått åtkomst av en administratör.

* **Omdesignat min Marketo**: Anpassa upplevelsen genom att lägga till widgetar som ger viktig information, meddelanden och länkar till de områden du besöker mest.

* **Design Studio - listvyer och detaljsidor**: Få bättre ordning och precision med filterbara och sökbara listvyer av mejl, landningssidor och formulär. På tillgångsinformationssidor finns viktig information om varje resurs, inklusive vilka program resursen används av, antalet utdrag som används och mycket annat.

* **Global sökning**: Marketo erbjuder nu en snabbare och robustare global sökfunktion på hela plattformen. Sökfrågor körs nu på alla tillgängliga arbetsytor och kan söka efter resurser (både aktiva och arkiverade), etiketter, kampanjer och program. Sökresultaten tillhandahålls via en övertäckning och varje resultat innehåller filplatshistoriken som anger var resursen finns.

* **Förbättrat användargränssnitt**: Nya ikoner, moduler och knappar, tillsammans med en ny färgpalett som speglar vår varumärkesuppdatering och gör Marketo Skyn ännu mer enastående och funktionell.

* **Förbättringar av e-postprogrammets användbarhet**: Vi fortsätter att gå mot en paritet i e-postprogrammens funktionalitet mellan vår klassiska Marketo Lead Management-plattform och den nya Marketo Skyn.
* **Event-With-Webinar-program**: Event-With-Webinar-program finns nu i Marketo Sky (Obs! endast GoToWebinar stöds i den här versionen med ytterligare integreringar som upprättas över tid).

## Account-Based Marketing {#account-based-marketing}

**[ABM Personabaserad segmentering och filtrering](/help/marketo/product-docs/target-account-management/using-personas.md)**

Anpassa era ABM-kampanjer för specifika personer i namngivna konton. Funktionen ABM Persona skapar en standardjobbtitel baserad på leadsegmentering och tillåter konfiguration av ytterligare persona segmenteringar.

## Analyser {#analytics}

**Bizible**

* **Anpassade beräknade fält**: Använd valfritt Bizible-attribut för att skapa anpassade fält som kan användas för instrumentpanelsrapportering och segmentering.

* **SOC II Type II-certifiering**: Ny certifiering av säkerhet och integritet bygger på typ I-ackreditering från tidigare i år.

## Webbanpassning {#web-personalization}

**[Lägg till underdomäner i kontoinställningar](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

För att hantera domäner och underdomäner effektivare kan användare nu lägga till underdomäner i sina RTP-kontoinställningar.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Uppdaterat MME Software Development Kit (SDK) för Android**

Vi har uppdaterat vårt SDK för Android till ett modernare, stabilare och skalbart ramverk som innehåller större flexibilitet och nya ingenjörsfunktioner. Apputvecklare i Android kan nu använda Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) med denna nya SDK.

* [Utvecklarinstruktioner](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Frågor och svar för utvecklare](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Apputvecklare **måste** uppdatering till den nya versionen före 31 mars 2019. Om du inte uppdaterar din SDK senast 31 mars 2019 kommer nya användare som hämtar din app efter detta datum inte att kunna få push-meddelanden förrän du uppdaterar till den senaste versionen av SDK. SDK-uppdateringen kräver inte att dina nuvarande mobilappsanvändare hämtar en ny version av din app.

## Ytterligare uppdateringar {#additional-updates}

**Extensible Webinar Platform**

Förutom vår produktrelease arbetar vårt partnerteam på ett nytt ramverk som gör det möjligt för webbinarier-leverantörer att bygga och underhålla sina egna integreringar med Marketo, vilket ger större flexibilitet när det gäller att uppdatera och förbättra sina lösningar samtidigt som marknadsförarna får ut så mycket som möjligt av de integreringar de valt.

Vi planerar att lansera vår nya plattform med leverantörer från fall till fall. Mer information finns i [programinformation](https://www.marketo.com/why-marketo/partners/technology/) eller kontakta Marketo.
