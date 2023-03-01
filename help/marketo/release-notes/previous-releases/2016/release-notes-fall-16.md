---
unique-page-id: 11384018
description: Versionsinformation -höst 16 - Marketo Docs - produktdokumentation
title: Versionsinformation - höst 16
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 4fa7e733a824af8d2fc0e3ba824b25f9bb985ccf
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Versionsinformation: Hösten &#39;16 {#release-notes-fall}

Följande funktioner finns i höstutgåvan 16. Se om det finns funktioner i din Marketo-utgåva. Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion.

## Prediktivt innehåll i e-post {#predictive-content-in-email}

Det finns en ny användarupplevelse i programmet Predictive Content som spårar, hanterar och rekommenderar ditt innehåll via våra maskininlärnings- och prediktiva algoritmer på webben och i e-postkanaler.

>[!NOTE]
>
>Alla kunder med Predictive Module aktiveras den 10 januari.

![](assets/shafe.png)

Nu kan du lägga till prediktivt innehåll i e-postmeddelandet. När e-postmeddelandet öppnas får mottagaren automatiskt relevant, rekommenderat innehåll som ökar engagemanget och konverteringsgraden.

![](assets/predictive.png)

## [Facebook Offline-konverteringar](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Tack vare integreringen med Facebook Offline Conversions skickas konverteringsdata i Marketo (för leads) automatiskt tillbaka till Facebook så att ert annonsteam bättre kan optimera annonskostnaderna. I den här Facebook Ad Manager-rapporten markeras offlinekonverteringarna.

![](assets/facebook.png)

## [Universellt ID](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Med ett universellt ID kan du komma åt flera Marketo-prenumerationer med en enda inloggning och snabbt växla mellan prenumerationer. Du kan använda en enda community-profil för alla dina prenumerationer.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Kontakta Marketo Support för att aktivera den här funktionen.

## Marketo kontobaserade marknadsföringsförbättringar {#marketo-account-based-marketing-enhancements}

Nu kan ni tilldela kontoteam till namngivna konton i kontobaserad marknadsföring (ABM), till exempel kontoägare, säljutvecklingsrepresentant, affärsutvecklingsrepresentant och kundframgångsansvarig. Du kan också skapa kontoägarspecifika kontolistor och skicka personliga ABM-rapporter varje vecka till kontoteamet.

![](assets/account-team-11-15-16.png)

**REST API**

I den här versionen kan du även hantera attribut och poäng för namngivna konton i ABM med Marketo REST API. Mer information om API:er finns på [Marketo Developers webbplats](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Förbättringar av granskningsspår](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

Granskningsspårning ger en omfattande historik över de ändringar som gjorts i din Marketo-prenumeration. Vi har lagt till ytterligare funktioner för spårning av program samt tagit del av viktig ändringsinformation för smarta kampanjer, smarta listor och ändringar som gjorts för användare och roller.

## [Nya behörigheter](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md) {#new-permissions}

**Låt e-postmeddelandet fungera**

Det var inte länge sedan du var tvungen att oroa dig för att användare ska skicka transaktionsmeddelanden via e-post till personer i din databas som har avbeställt prenumerationen. Du kan nu ange vilka användare som kan få ett e-postmeddelande att fungera eller redigera användbara e-postmeddelanden.

**Redigera kampanjbegränsningar**

Varför [kampanjbegränsningar](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) om du inte klarar dem? När du anger inställningarna för kampanjbegränsning för att begränsa antalet personer i databasen som kan användas för en enskild kampanj, kan du nu begränsa vilka användare som kan åsidosätta inställningarna när du schemalägger en kampanj.

## [Ljud för mobila push-meddelanden](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Ge dina iOS Push Notification ännu bättre detaljrikedom genom att aktivera ljud. Med den här nya funktionen kan du aktivera ett ljud när push-meddelanden visas på den mobila enheten.

>[!NOTE]
>
>* Enhetsägare kan välja att förhindra att ljud spelas upp i enhetsinställningarna, och apputvecklare kan ge enhetsägare alternativ i programmet för att förhindra att ljud spelas upp.
>* Ljud spelas automatiskt upp när ett push-meddelande visas på en Android-enhet.


![](assets/sound-for-push-notifications.png)

## [Säljinsikter kompatibel med Salesforce-kryptering](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight är nu kompatibelt med Salesforce Shield Encryption. Alla Sales Insight-kunder bör uppgradera till det senaste hanterade paketet (version 1.4359.2), som är [finns på Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API:er för namngivna konton](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

I den här versionen kan Marketo ABM-användare hantera namngivna konton via API:t för namngivna konton. Användare kan skapa, uppdatera och ta bort namngivna konton samt läsa och uppdatera ABM-poängen för namngivna konton.

## [Stöd för API:t för e-postredigeraren v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Hantera variabler och moduler för e-post i v2.0-format med Marketo REST API.

## [Ändringar i Marketo Salesforce Sync](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo Salesforce-integrering utvecklas för att förbättra det sätt på vilket Marketo-fält synkroniseras med Salesforce. I stället för att behöva synkronisera en stor grupp fält som du kanske behöver kan du nu välja vilka fält du vill inkludera och välja vilka. Läs vår dokumentation här för mer information: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
