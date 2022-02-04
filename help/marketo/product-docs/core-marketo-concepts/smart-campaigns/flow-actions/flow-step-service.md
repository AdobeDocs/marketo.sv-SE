---
description: Flow Step Service - Marketo Docs - produktdokumentation
title: Flödesstegstjänst
hide: true
hidefromtoc: true
source-git-commit: 08767d476cf89eefe7223308945733c6f813a34d
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 0%

---

# Flödesstegstjänst {#flow-step-service}

>[!NOTE]
>
>Den här förhandsversionen är för närvarande endast tillgänglig för konton som är registrerade i självbetjäningsflödesstegprogrammet.

Självbetjäningsflödessteg är ett ramverk och en uppsättning funktioner för att skapa, publicera och integrera webbtjänster i smarta webbkampanjer i Adobe Marketo Engage. Handboken är avsedd för användare av Marketo Engage som vill installera och använda tjänster som redan har skapats och publicerats. For information on authoring and publishing your own service, please refer to the [GitHub repository for the Service Provider Interface](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface). A Proof-of-Concept Lookup Table implementation may be found [here](https://github.com/adobe/mkto-flow-lookup).

## Restriktioner och varningar före lansering {#pre-release-restrictions-and-warnings}

Den här funktionen är för närvarande i en sluten betaversion och har vissa användningsbegränsningar.

* This feature may only be used on Sandbox instances of Marketo Engage
* Anpassade och tredjepartsflödessteg är inte kompatibla med körbara kampanjer från och med Q4 2021. Detta planeras att fastställas under andra kvartalet 2022
* Marketo Sky UI should not be used at all on instances with this feature enabled

## Onboarding och Managing Services {#onboarding-and-managing-services}

För installation av ett anpassat flödessteg krävs administratörsbehörighet i Marketo (**Hantera webbhotell** i den 21 januari (Changing in the March 11th release). Apart from the Installation URL, all other aspects of a serviced may be edited after completing initial onboarding by drilling down into the service detail screen from the Service Providers grid.

## Installations-URL {#installation-url}

To begin installation, you&#39;ll need to first obtain the URL of the OpenAPI document that defines your service. Din tjänsteleverantör bör kunna ge dig detta och har vanligtvis en URL som slutar på `/openapi.json`. Fullständiga URL:er ser ut ungefär som `https://www.example.com/OpenAPI.json`. När du har den här URL:en går du till menyn Tjänsteleverantörer i ditt Admin Section.

Click **Next** to go to the Enter Service Credentials section.

![](assets/flow-step-service-1.png)

## Enter Service Credentials {#enter-service-credentials}

Marketo måste ha giltiga API-autentiseringsuppgifter för att komma åt den tjänst som installeras. Dessa inloggningsuppgifter bör du få från din tjänsteleverantör. Services have three different authentication options, so you may see one of three different prompts for credentials: **API Key** which has only one input field, **Basic Authentication** which requires a username and password and may also require a field called Realm, and **OAuth2** using the _Client Credentials_ grant, which requires a _Client ID_ and _Client Secret_.

>[!NOTE]
>
>OAuth2 kommer inte att vara tillgänglig förrän den 11 mars-utgåvan.

När du sparar dina inloggningsuppgifter försöker Marketo anropa tjänstens statusslutpunkt för att verifiera att de är giltiga. If the credentials provided are invalid, you&#39;ll see an error indicating this.

## Onboarding Guide (tillval) {#onboarding-guide}

Vissa tjänsteleverantörer kommer att inkludera ett valfritt steg i Onboarding Guide. Det här steget kommer att innehålla eventuella ytterligare instruktioner för att slutföra tjänstintroduktionen som är specifika för tjänsten.

## Fältmappning {#field-mapping}

För att kunna ta emot eller returnera data från ett visst lead-fält måste det fältet mappas. Mappning är ett obligatoriskt steg under introduktionen, men du kan alltid gå tillbaka och ändra mappningarna senare. There are two types of mappings that are configured in separate screens: **Outgoing Fields**, which are sent to the service when Marketo invokes the flow step, and **Incoming Fields** which are fields which may receive data from the service when it returns data to Marketo.

>[!NOTE]
>
>Genom att mappa ett utgående fält ger du Marketo tillstånd att överföra data från det fältet som är relaterade till leads som bearbetas av den associerade tjänsten. Se till att du har rätt juridisk status och behörighet att överföra dessa data till din tjänsteleverantör, eftersom dessa fält kan innehålla personligt identifierbar information som omfattas av dataintegritetsskydd, skydd och innehavslagstiftning.

Optional field mappings may be disabled without disruption to your service, but required mappings may not be removed or deactivated completely.

## Tjänststyrda mappningar {#service-driven-mappings}

Tjänster som har en fast uppsättning indata och utdata, som ett steg i händelseregistreringsflödet, använder **Tjänststyrda mappningar**. För den här typen av mappning tillhandahåller tjänsteleverantören både en datatyp och ett tips i form av ett API-namn. Om tipset matchar API-namnet för ett befintligt lead-fält fylls fältet automatiskt i i mappningsavsnittet. För fält utan matchande tips måste du fylla i mappningen manuellt från fältlistan med matchande datatyp. Mappings that are required must be populated to complete onboarding.

![](assets/flow-step-service-2.png)

## User-Driven Mappings {#user-driven-mappings}

Services that do not have a fixed set of inputs and outputs, like a date-formatting service, use **User-Driven Mappings**. Det innebär att varje inkommande och utgående fält måste konfigureras av en administratör.

![](assets/flow-step-service-3.png)

## Utgående fält {#outgoing-fields}

Outgoing fields are those which are sent to the Flow Step Service when that flow step is used in a smart campaign.

## Inkommande fält {#incoming-fields}

Inkommande fält är de som tjänsten Flow Step kan skriva data till.

## Konfigurationsalternativ (valfritt) {#configuration-options}

Vissa tjänster har antingen valfria eller obligatoriska globala konfigurationsalternativ. If any options are required, then a value must be set for all required options before saving or completing onboarding. Parametrar vars namn är i kursiv stil skickas till den anropade tjänsten som rubriker.

![](assets/flow-step-service-4.png)

## Retiring a Service {#retiring-a-service}

To facilitate transitions to new or alternative versions of a service, without disrupting active usage, services can be retired from the Service Providers menu. **Återkalla en tjänst** tar bort motsvarande flödessteg från paletten Smart Campaign-flöde, så att inga nya användningar av den kan skapas. In most cases, you should have a replacement service ready to replace the existing one when you choose to retire a service.

## Service Deprecation {#service-deprecation}

Ibland måste tryckeriet ersätta stegvisa tjänster som en normal del av programvarans livscykel. När en tjänsteleverantör meddelar detta fylls borttagningsdatumet och meddelandet i i rutnätsvyn för tjänsteleverantörer. Om du fortsätter att använda en tjänst som har blivit inaktuell kan det leda till avbrott i tjänsten om den inte längre svarar på förväntat sätt, eller slutar ta emot begäranden från Marketo Smart Campaigns, så du bör vara uppmärksam på eventuella meddelanden om borttagning av tjänst som du får och vidta lämpliga åtgärder för att ta bort eller ersätta åtgärder från tjänsten som fortfarande används.

## Using Third-Party and Custom Flow Steps {#using-third-party-and-custom-flow-steps}

Installerade flödessteg kan i stort sett användas på samma sätt som standardflödessteg. Alla flödesparametrar som definieras av tjänsten presenteras för slutanvändarna.

## Refreshing Picklists {#refreshing-picklists}

Marketo kommer att uppdatera valmöjligheterna för tjänster varje kväll, men det finns tillfällen när du behöver nya alternativ, som att skapa kampanjer. You can refresh these easily from any instance of your flow step using the refresh button, or by going to the Admin > Service Providers menu and clicking Refresh Picklist once you have selected your service.

## Checking Incoming Fields {#checking-incoming-fields}

Du kan kontrollera vilka inkommande fält som har konfigurerats för ett visst flödessteg genom att hålla muspekaren över verktygstipsikonen. This is useful for determining which fields might change when a lead flows through it, so you can configure choices in subsequent steps using those fields.

![](assets/flow-step-service-5.png)

## Inkommande fält och ändringar av datavärden {#incoming-fields-and-data-value-changes}

Unlike most other flow steps, ones implemented with the SSFS framework may write data back to lead fields which are mapped by an admin and record those changes as Data Value Change activities.  När ett flödessteg skriver data på det här sättet kommer alla dessa ändringar att slutföras innan Smart Campaign går vidare till efterföljande steg, så att alla data som skrivs kan användas i efterföljande flödesstegval.

## Tjänstloggar och statistik {#service-logs-and-statistics}

Varje tjänst för flödessteg har flera typer av loggning som är kopplade till den för att hjälpa till att övervaka hälsan och felsöka problem som rör integreringen.

## Service Statistics {#service-statistics}

I loggen för tjänststatistik sammanställs resultaten av anrop och återanrop för varje tjänst. De grupperas efter tid, nivå (segment eller post) och kod och anger antal och det senaste loggmeddelandet för varje mottagen kod. Kontrollpanelen är främst avsedd att underlätta övervakningen av tjänsternas hälsa.
