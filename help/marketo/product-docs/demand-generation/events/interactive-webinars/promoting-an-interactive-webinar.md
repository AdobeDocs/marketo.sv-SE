---
description: Marknadsför ett interaktivt webbinarium - Marketo Docs - produktdokumentation
title: Marknadsför ett interaktivt webbinarium
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Marknadsför ett interaktivt webbinarium {#promoting-an-interactive-webinar}

Att marknadsföra ett interaktivt webbinarium liknar att marknadsföra ett partnerwebbinarium via Launchpoint. När du skapar ett händelseprogram för interaktiva webbinarier kan du lägga till medlemmar antingen genom att köra en kampanj eller importera medlemmar till programmet. Om du vill kontrollera vilka medlemmar som har lagts till i händelseprogrammet för interaktiva webbinarier klickar du på fliken **[!UICONTROL Members]**.

![](assets/promoting-an-interactive-webinar-1.png)

## Översikt {#overview}

När medlemmarna har lagts till eller importerats kan du skapa en e-postkampanj i händelseprogrammet Interactive Webinar för att skicka en inbjudan till alla programmedlemmar och ändra deras status till&quot;inbjudna&quot; när e-postmeddelandet har levererats.

>[!NOTE]
>
>Om du vill lägga till en kollega eller presentatör som målgruppsmedlem i det interaktiva webbseminariets Event Program måste du använda ett annat e-post-ID för dem, annars får de felmeddelandet&quot;this email is already registered&quot;.

E-postmeddelandet kan innehålla specifik information om programmet, samt en URL för landningssida som skulle dirigera om mottagaren till en viss sida där mer information om webbinariet (t.ex. innehåll, presentatörsinformation osv.) kan läggas till. Denna landningssida kan skapas som en lokal resurs i händelseprogrammet för interaktiva webbinarier.

Du kan begära registrering för det här webbinariet genom att aktivera ett formulär på landningssidan och länka formulärklickningarna till aktiverad registrering i händelseprogrammet för interaktiva webbinarier. En kampanj som använder formulärinlämning som utlösare och ändrar programstatus från&quot;inbjuden&quot; till&quot;registrerad&quot;.

>[!NOTE]
>
>Övergången från&quot;inbjuden&quot; till&quot;registrerad&quot; är inte automatisk i interaktiva webbinarier eftersom det kan finnas flera utlösare som skapar övergången.

När en medlem har varit med i det&quot;registrerade&quot; programmet i ett händelseprogram för interaktiva webbinarier registreras det automatiskt i det webbinarium som skapats i Adobe Connect. Registreringsdata som Förnamn, Efternamn och E-post-ID överförs sedan till Adobe Connect. Det innebär att när användaren ansluter sig till webbinariet som deltagare blir informationen tillgänglig för presentatören eller värden under webbinariet.

Inom några minuter efter registreringen fylls URL:en för webbinariet för medlemmen i på fliken Medlemmar. Om du inte hittar kolumnen för webbinariets URL kontrollerar du att kolumnen har lagts till i vyn. Det här är en personlig URL för varje registrerad medlem som kan ange webbinariet vid schemalagd tidpunkt utan att någon autentisering krävs. Token som utbyts internt tar hand om medlemmarnas autentisering.

Du kan använda `{{member.webinar url}}` [token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} för att inkludera webbinariets URL till enskilda medlemmar i en e-postkampanj för att meddela att de har registrerats i händelsen och för att använda den kopplade URL:en för att ange webbinariet vid den schemalagda tidpunkten. Kalendertoken kan användas i samma e-postkampanj för att säkerställa att webbinariet kan läggas till i medlemmarnas kalendrar.

Länkarna finns till höger på fliken Översikt i ditt Event Program för att skapa en landningssida samt en e-postkampanj. Resten av kampanjerna för en händelse är desamma som för partnerwebbinarier som använder integreringen med Launchpoint.

![](assets/promoting-an-interactive-webinar-2.png)

Med interaktiva webbinarier kan du begära registrering före, under eller efter ett webbinarium. I samtliga fall behöver du bara dela webbinariets URL med leadet. När du klickar på länken innan webbinariet börjar skickas de till en startsida som är före webbinariet. När du klickar på det under webbinariet kommer de till det pågående webbinariet. Klicka på det när webbinariet tar dem till en inspelning av webbinariet.

## Tokens för interaktiva webbinarier {#interactive-webinars-tokens}

Använd variabler för att marknadsföra interaktiva webbinarier i e-postmeddelanden utan att manuellt behöva lägga till webbinarier. Detta förbättrar den övergripande effektiviteten eftersom alla ändringar som görs i webbinariets metadata (som webbinariets titel, startdatum osv.) automatiskt återspeglas i dina resurser.

![](assets/promoting-an-interactive-webinar-3.png)

>[!NOTE]
>
>Interaktiva webbinaritoken stöds för närvarande inte i landningssidor.

**Lista över tokens**

<table><thead>
  <tr>
    <th>Token</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>program.webinarCapacity</td>
    <td>Maximalt antal deltagare som kan delta i det interaktiva webbinariet.</td>
  </tr>
  <tr>
    <td>program.webinarDuration</td>
    <td>Den varaktighet som det interaktiva webbinariet är schemalagt för.</td>
  </tr>
  <tr>
    <td>program.webinarEndDate</td>
    <td>Slutdatumet för det schemalagda interaktiva webbinariet.</td>
  </tr>
  <tr>
    <td>program.webinarEndTime</td>
    <td>Den schemalagda sluttiden för det interaktiva webbinariet.</td>
  </tr>
  <tr>
    <td>program.webinarGenericURL</td>
    <td>Den generiska inspelnings-URL som kan delas med publiken efter webbinariet. Den här URL:en används inte för att delta i webbinariet live och spårar inte målgruppens aktivitet.</td>
  </tr>
  <tr>
    <td>program.webinarLanguage</td>
    <td>Det språk på vilket webbinariet ska genomföras.</td>
  </tr>
  <tr>
    <td>program.webinarStartDate</td>
    <td>Startdatum för det schemalagda interaktiva webbinariet.</td>
  </tr>
  <tr>
    <td>program.webinarStartTime</td>
    <td>Den schemalagda starttiden för det interaktiva webbinariet.</td>
  </tr>
  <tr>
    <td>program.webinarTimezone</td>
    <td>Den tidszon som Interactive Webinar är schemalagd i.</td>
  </tr>
  <tr>
    <td>program.webinarTitle</td>
    <td>Titeln på det interaktiva webbinariet som är synligt för läsarna på webbseminariet Screens.</td>
  </tr>
</tbody></table>
