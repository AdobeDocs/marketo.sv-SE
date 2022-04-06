---
description: Aktuell versionsinformation - Marketo Docs - produktdokumentation
title: Aktuell versionsinformation
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 621bb7db9485ef1cc559b5b161d5acb606bc4903
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Versionsinformation: Maj 2022 {#release-notes-may-22}

Här nedan hittar du alla funktioner som ingår i versionen från maj 22. Se om det finns funktioner i din Adobe Marketo Engage-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![stjärna](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att lanseras den **6 maj 2022**, med en stegvis utrullning av återstående funktioner under de följande veckorna (om inget annat anges).

## Integrering med CRM {#native-crm-integration}

**Integrering av veeva CRM (begränsad tillgänglighet)**: Förbättra engagemanget hos hälso- och sjukvårdspersonal genom att synkronisera aktiviteten mellan Veeva CRM och Marketo Engage via inbyggd integrering. Tack vare den här integreringen kan marknadsförarna skapa mer personaliserade och sömlösa upplevelser över flera kanaler för hälso- och sjukvårdspersonal. Kontakta din Customer Success Manager om du är intresserad av att delta.

## Flerkanalsmarknadsföring {#cross-channel-orchestration}

**Chatbot Events for Dynamic Chat**: Utnyttja mer detaljerade beteendedata för webbbesökare som t.ex. tid på sidan, tid på webbplatsen och procent för sidrullning för att definiera när en chattdialog ska visas.

**PDF Embed for Dynamic Chat**: Öka engagemanget och dela meningsfullt innehåll genom att bädda in PDF i chattdialogrutor och mäta innehållets prestanda med hjälp av uppföljning av engagemangsaktiviteter.

**Utökat språkstöd för dynamiskt chatt**: Användargränssnittet Dynamic Chat finns nu även på franska, tyska, japanska, portugisiska och spanska. Chattdialogrutor kan även konfigureras på dessa språk.

**Uteslut URL:er för dynamiskt chatt**: Styr vilken av dina webbsidor Dynamic Chat ska visas med möjligheten att utesluta specifika URL:er från kriterier för målanpassning.

**Förbättrad filtrering av e-poststartaktivitet**: Fortsätt att skydda databasens hälsa med möjligheten att identifiera båda beteenden baserat på dolda länkar, användaragenter eller IP-adresser och närhetsmönster, utöver den befintliga IAB-listan, matchar identifiering. Visa startaktivitetsstatistik som gör att du kan förstå antalet båda aktiviteter som identifieras för varje typ.

**STS Header for Email Tracking Links**: Följ vedertagna säkerhetsstandarder med möjlighet att lägga in säkra transportsäkerhetsrubriker för att säkerställa att trafik till spårade länkar alltid är säker.

## Nästa generations upplevelse {#next-generation-experience}

**Växla som standard till nästa generations upplevelse**: Växlingsknappen kommer att vara standard för den nya upplevelsen på alla skärmar där den är tillgänglig, vilket gör det enklare för användarna att upptäcka de uppdaterade designförbättringarna och användbarhetsförbättringarna.

**Uppdaterad skärm i nästa generation**:

Vi levererar detaljvy för e-postmallar i Design Studio i nästa generation av upplevelser, med uppdaterade design- och användarvänlighetsförbättringar som är tillgängliga via växlingsfunktion.

## Experience Automation {#experience-automation}

**Självbetjäningsflödessteg (forts. beta)**: Utöka anslutningsmöjligheterna mellan Marketo Engage och resten av högen med möjligheten att skapa anpassade flödessteg som kan användas i smarta kampanjer. Både användare och partners i Marketo Engage kan utnyttja den här funktionen för att möjliggöra användning av externa webbtjänster i utlösar-, batch- och körbara kampanjer (till skillnad från webbhookar som bara kan användas i utlösarkampanjer).

## API-förbättringar {#api-enhancements}

* **Utökad API-åtkomst för CRM-aktiverade prenumerationer**: Vi utökar API-åtkomsten för prenumerationer som har en CRM-synkronisering aktiverad så att användare kan hämta företag, säljprojekt och säljare från Marketo Engage.
* **Stöd för&quot;dolda&quot; datatyper i Forms**: Ger möjlighet att hantera dolda formulärfält via API.
* **Stöd för flera jämförelsevärden för isNot-formulär via regler**: Hantera synlighet för formulärfält baserat på om värdet för ett annat fält inte är ett av värdena i en given lista.
* **Tillåt inställning av Visa och Skickade värden i Välj listor separat**: Ange visningsvärdet och det skickade värdet separat i ett fält. Visa till exempel namnet på ett hotell, men skicka ett internt ID till serverdelen.
* **Tillåt inställning av Inaktivera Open Tracking vid skapande eller uppdatering av e-post**: Skapa ett e-postmeddelande med öppen spårning inaktiverat.

## Meddelanden {#announcements}

**E-postverifiering och unikhet**: Från och med april påbörjas utrullningen av e-postverifieringen. I det läget kommer Marketo Engage-användares e-postadresser att kräva verifiering och unikhet (detta gäller inte endast API-användare). Katalogtjänstautentiserade användare får automatiskt sina e-postmeddelanden verifierade när deras prenumeration aktiveras med e-postverifiering.

Verifiering via e-post för prenumerationer med funktionen Inbjudan till användare, eller som har ett enda e-postmeddelande kopplat till flera användare, sammanfaller med majversionen. Prenumerationer som har ett enda e-postmeddelande kopplat till flera användare aktiveras med e-postverifiering och kräver att dessa användare löser konflikten och använder ett unikt e-postmeddelande per användare. När funktionen&quot;Logga in i inbjudan till användare&quot; är aktiverad måste användare som bjudits in via den här funktionen ha en unik e-postadress. För API-användare som bjudits in via den här funktionen behöver e-postadressen inte vara unik.

**_Product Release Webinar_**

Besök oss den 11 maj 2022 kl. 9.00 PT/12.00 ET för en [live webbinarium](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} som hanteras av vårt produktteam där du kan lära dig att använda alla de senaste produktinnovationerna.
