---
unique-page-id: 10096675
description: Skapa underordnade kampanjer och lokala resurser - Marketo Docs - Produktdokumentation
title: Skapa underordnade kampanjer och lokala resurser
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---


# Skapa underordnade kampanjer och lokala resurser {#create-child-campaigns-and-local-assets}

Skapa era barnkampanjer och lokala resurser med Design Studio.

## Landningssida och formulär {#landing-page-and-form}

För att säkerställa att personer är korrekt registrerade med ON24 måste följande fält inkluderas i Marketo-formuläret:

* Förnamn
* Efternamn
* E-postadress

Du kan även överföra följande fält till ON24:

* Företag
* Befattning

Med rätt flödessteg i registreringskampanjen kommer personerna att flyttas till ON24 och markeras som registrerade. Du kan lägga till andra fält i formuläret och informationen hämtas i Marketo som en del av personinformationsposten.

>[!CAUTION]
>
>För att integreringen ska lyckas måste du antingen använda ett Marketo-formulär för att registrera dina medarbetare för Event, eller ett icke-Marketo-formulär med rätt API-integrering för att skicka registreringsdata till Marketo.

## E-post och URL-token {#emails-and-url-tokens}

Skapa inbjudan, bekräftelse, uppföljning och tack för dina e-postmeddelanden med Marketo.

## Marketo-bekräftelse - e-postadress och URL-token {#marketo-confirmation-email-and-url-token}

Använd Marketo för att skicka bekräftelsemeddelandet för din händelse. När en person registrerar sig får han eller hon en unik URL som kan användas för att ange händelsen.

>[!NOTE]
>
>Om du vill fylla i bekräftelsemeddelandet med den här unika URL-adressen använder du följande token i e-postmeddelandet: `{{member.webinar url}}`. När du skickar ut en bekräftelse-URL matchas denna token automatiskt mot personens unika bekräftelse-URL.
>
>Ange typen av bekräftelsemeddelande som **Operational** för att se till att alla som registrerar får sin bekräftelseinformation, även om de avbeställer prenumerationen.

>[!TIP]
>
>Du kan konfigurera ON24 för att skicka ut bekräftelser, påminnelser eller uppföljningsmeddelanden. Se [ON24 Help Site](https://webcastelitehelp.on24.com) för mer information.

## Krav för registrering av underordnad kampanj {#registration-child-campaign-requirements}

Händelser innehåller en eller flera underordnade kampanjer som alla tillsammans kan flytta personer genom programstatusarna och som gör att du kan spåra hur din händelse fungerar.

Exempel på underordnade kampanjer är en inbjudningskampanj, en registreringskampanj och uppföljningskampanjer.

>[!CAUTION]
>
>För att adaptern ska kunna utföra sitt arbete MÅSTE du skapa en registreringskampanj. Den här kampanjen måste utlösas av personen som fyller i ett formulär och det första steget måste ändra personens programstatus till **Registrerad**. Kampanjen skickar sedan ett bekräftelsemeddelande via e-post. Mer information finns i resten av den här artikeln.

**Registrering/bekräftelse (utlösarkampanj)**

* Smart List
* Utlösare baserad på **Fyller i formulär**. Se till att du inkluderar landningssidan som formuläret är aktivt på med **Lägg till begränsning**, särskilt om samma formulär används på flera landningssidor.

>[!CAUTION]
>
>Du måste använda ett Marketo-formulär för att registrera dina medarbetare för händelsen, eller ett icke-Marketo-formulär med rätt API-integrering för att skicka registreringsdata till Marketo. Detta är viktigt för att integreringen av din händelsepartner ska lyckas.

>[!NOTE]
>
>Om du använder ett Marketo-formulär på en icke-Marketo-startsida är utlösaren **Fyller i formulär** med formulärnamnet.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flöde**

* **Ändra programstatus**  - Ange som webbinarium -> Registrerad.

Det här flödessteget krävs som STEG FÖR FÖRSTA FLÖDE när du konfigurerar din underordnade kampanj. När en persons programstatus ändras till Registrerad skickar Marketo registreringsinformationen till ON24. Ingen annan status kommer att föra personen över.

* **Skicka e-post**  - Bekräftelsemejl. Ange det här e-postmeddelandet som **Operational** så att personer som har registrerat sig fortfarande får det.

Flödessteget **Skicka e-post** MÅSTE vara det andra steget. Bekräftelsemeddelandet innehåller `{{member.webinar url}}`, som fylls i med information som skickas tillbaka till Marketo från ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Ordningen för dessa flödessteg är viktig eftersom åtgärderna utförs i Marketo i den ordning som de utförs. **Ändra programstatus**-steget skickar personen till ON24 för registrering och en unik URL genereras. När detta har inträffat kan du skicka ut bekräftelsemeddelandet som innehåller denna unika URL-adress med hjälp av `{{member.webinar URL}}`-token.
>
>Om personen returneras med ett registreringsfel får han/hon ingen e-postbekräftelse.

Nästa steg är att [testa din ON24-händelseintegrering](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Om Marketo ON24-adapterhändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [Exempel på händelseintegrering ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Om status för webbinarium](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

