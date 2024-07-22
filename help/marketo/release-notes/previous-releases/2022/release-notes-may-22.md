---
description: Versionsinformation - maj 2022 - Marketo Docs - produktdokumentation
title: Versionsinformation - maj 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Versionsinformation: maj 2022 {#release-notes-may-22}

Här nedan hittar du alla funktioner som ingår i versionen från maj 22. Se om det finns funktioner i Adobe Marketo Engage Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att börja släppas den **6 maj 2022**, med en stegvis utrullning av återstående funktioner under de följande veckorna (om inget annat anges).

## Integrering med CRM {#native-crm-integration}

**[Integrering med CRM för vektorgrafik](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (begränsad tillgänglighet)**: Förbättra interaktionen med vårdpersonal genom att synkronisera aktiviteter mellan vektorgrafikCRM och Marketo Engage via inbyggd integrering. Tack vare den här integreringen kan marknadsförarna skapa mer personaliserade och sömlösa upplevelser över flera kanaler för hälso- och sjukvårdspersonal. Kontakta kontoteamet (din kontoansvarige) på Adobe om du är intresserad av att delta.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

**Chatbot-händelser för Dynamic Chat**: Utnyttja mer detaljerade beteendedata för webbbesökare som tid på sidan, tid på webbplatsen och procent för sidbläddring för att definiera när en chattdialog ska visas.

**PDF Embed för Dynamic Chat**: Öka engagemanget och dela meningsfullt innehåll genom att bädda in PDF i chattdialogrutor och mäta innehållets prestanda med hjälp av uppföljning av engagemangsaktiviteter.

**Utökat språkstöd för Dynamic Chat**: Dynamic Chat kommer nu också att finnas på franska, tyska, japanska, portugisiska och spanska. Chattdialogrutor kan även konfigureras på dessa språk.

**Uteslut URL:er för Dynamic Chat**: Kontrollera vilken av dina webbsidor som Dynamic Chat visas på med möjligheten att exkludera specifika URL:er från målvillkor.

**[Förbättringar av filtrering av punktaktivitet](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: Fortsätt att skydda databasens hälsa med möjlighet att identifiera båda beteenden baserat på dolda länkar, användaragenter eller IP-adresser och närhetsmönster, utöver den befintliga IAB-listan, utöver identifiering av matchningar. Visa startaktivitetsstatistik som gör att du kan förstå antalet båda aktiviteter som identifieras för varje typ.

**[STS Header för länkar för e-postspårning](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: Följ bästa säkerhetspraxis med möjlighet att använda säkerhetsrubriker för säker transport för att säkerställa att trafik till spårade länkar alltid är säker.

## Nästa generations upplevelse {#modern-ux}

**Växla växel som är standard för nästa generation av upplevelse**: Växlingsväxeln är standard för den nya upplevelsen på alla skärmar där den är tillgänglig, vilket gör det enklare för användare att upptäcka de uppdaterade designförbättringarna och användbarhetsförbättringarna.

**Uppdaterad skärm i nästa generation av upplevelse**:

Vi levererar detaljvy för e-postmallar i Design Studio i nästa generation av upplevelser, med uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion.

## Experience Automation {#experience-automation}

**Självbetjäningsflödessteg (forts. beta)**: Utöka anslutningen mellan Marketo Engage och resten av stacken med möjligheten att skapa anpassade flödessteg som kan användas i smarta kampanjer. Både användare och partners i Marketo Engage kan utnyttja den här funktionen för att möjliggöra användning av externa webbtjänster i utlösar-, batch- och körbara kampanjer (till skillnad från webbhookar som bara kan användas i utlösarkampanjer).

## API-förbättringar {#api-enhancements}

* **Utökad API-åtkomst för CRM-aktiverade prenumerationer**: Vi utökar API-åtkomst för prenumerationer som har en CRM-synkronisering aktiverad för att tillåta användare att hämta företag, säljprojekt och säljare från Marketo Engage.
* **Stöd för dolda datatyper i Forms**: Ger möjlighet att hantera dolda formulärfält via API.
* **Stöd för flera jämförelsevärden för isNot-formulär via regler**: Hantera synlighet för formulärfält baserat på om värdet för ett annat fält inte är ett av värdena i en given lista.
* **Tillåt inställning av Visa och Skickade värden i Välj listor separat**: Ange visningsvärdet och skicka värdet separat i ett fält. Visa till exempel namnet på ett hotell, men skicka ett internt ID till serverdelen.
* **Tillåt inställning av Inaktivera Open Tracking vid skapande eller uppdatering av e-post**: Skapa ett e-postmeddelande med öppen spårning inaktiverat.

## Meddelanden {#announcements}

**E-postverifiering och unikhet**: Från och med april påbörjas utrullningen av e-postverifieringen. I det läget kommer Marketo Engage-användares e-postadresser att kräva verifiering och unikhet (detta gäller inte endast API-användare). Katalogtjänstautentiserade användare får automatiskt sina e-postmeddelanden verifierade när deras prenumeration aktiveras med e-postverifiering.

Verifiering via e-post för prenumerationer med funktionen Inbjudan till användare, eller som har ett enda e-postmeddelande kopplat till flera användare, sammanfaller med majversionen. Prenumerationer som har ett enda e-postmeddelande kopplat till flera användare aktiveras med e-postverifiering och kräver att dessa användare löser konflikten och använder ett unikt e-postmeddelande per användare. När funktionen Logga in i inbjudan till användare är aktiverad måste användare som bjudits in via den här funktionen ha en unik e-postadress. För API-användare som bjudits in via den här funktionen behöver e-postadressen inte vara unik.

**Ändra beteende för arkivmapp**: I den här versionen är möjligheten att skapa nya resurser i arkivmappar inte längre tillgängligt från trädsnabbmenyerna. Menyalternativen för att skapa nya resurser döljs för alla resurser. [Läs mer här](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webbseminarium om produktreleaser_**

[Mars och maj 2022 Marketo Engage Release Webinar](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
