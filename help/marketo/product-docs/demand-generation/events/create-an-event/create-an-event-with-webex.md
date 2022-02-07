---
unique-page-id: 2949863
description: Skapa en händelse med Webex - Marketo Docs - produktdokumentation
title: Skapa en händelse med Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
source-git-commit: 8813686a39852443bf200eda232fd5448c6aa414
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Skapa en händelse med Webex {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Lägg till webb som en LaunchPoint-tjänst](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Ange lämplig [flödesåtgärder](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) för att spåra engagemang
>* Kontrollera att du använder Webex-händelser (klassiska)


Skapa först en Webex-händelse i Webex Event Center. Marketo använder bara specifika inställningar och fält för din integrering, som vi kommer att gå igenom inom kort. Andra fält som du kanske vill konfigurera för WebBex beskrivs i [Användarhandbok för Webex Event Center](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage stöder endast händelser som skapats i WebBex-händelser (klassiska). Marketo stöder för närvarande inte händelser skapade i WebBex Events (nya).

## Grundläggande information {#basic-information}

* **Händelsenamn -** Det här namnet kan visas i Marketo.
* **Kryssrutan Ej listrerad**

   * Vi rekommenderar att du gör det **not** lista evenemanget. På så sätt kan alla registrera sig via Marketo landningssida. Personer som registrerar sig via en annan mekanism än Marketo visas i Marketo efter att evenemanget har avslutats OCH endast om de deltog i evenemanget.
   * Om du väljer att lista evenemanget visas det på sidan Lista över händelser för alla som besöker din Event Center-webbplats.

* **Registrering -** Markera den här rutan om du vill ange &quot;required&quot;. Du använder ett formulär/en landningssida från Marketo för att samla in registreringsinformation som skickas till Webex.
* **Händelsenord**- (valfritt) Om du använder det här fältet måste du ta med det i bekräftelsemeddelandet!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Datum och tid {#date-time}

* **Startdatum** - Ange ditt startdatum. Detta kommer att kunna visas i Marketo.

* **Starttid** - Ange din starttid. Detta kommer att kunna visas i Marketo.

* **Beräknad varaktighet** - Ange händelsens varaktighet. Detta kommer att kunna visas i Marketo.

* **Tidszoner** - Ange tillämpliga tidszoner. De kommer att kunna ses i Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Inställningar för ljudkonferens {#audio-conference-settings}

De här inställningarna finns endast i Webex. De används inte av eller kan inte visas i Marketo, men de kan vara viktiga för ditt webbinarium, så dubbelkontrollera dem!

## Händelsebeskrivning och -alternativ  {#event-description-options}

Följande alternativ används av eller kan visas i Marketo. Andra fält finns endast i Webex.

* **Beskrivning** - Ange en beskrivning. Detta kan visas men inte ändras i Marketo.
* **Enkät efter evenemanget** - Marketo kan för närvarande inte samla in information om en undersökning efter ett evenemang på webben.
* **Mål-URL** - (valfritt) Du kan ange URL-adressen till en Marketo-landningssida som fungerar som mål-URL-adressen som ska visas när sessionen är slut.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Deltagare och registrering {#attendees-registration}

Du styr inbjudningslistan, registreringsformuläret och andra e-postmeddelanden med hjälp av en Marketo Event. Andra funktioner stöds inte av Marketo, bland annat:

* **Högsta antal registranter** - För närvarande **not** som stöds med integreringen mellan Marketo och Webex.  Manuellt godkännande av registranter är tillgängligt med statusen Väntande godkännande och status i Marketo.

* **Registrerings-ID krävs** - Stöds för närvarande med Marketo-Webex-integreringen. Du kan använda Marketo för att skicka ut bekräftelsemeddelandet för ditt event. När personen registrerar sig får han/hon en unik URL som han/hon använder för att ange händelsen.

   >[!TIP]
   >
   >Om du vill fylla i bekräftelsemeddelandet med den här unika URL-adressen använder du följande token i e-postmeddelandet: `{{member.webinar url}}`. När bekräftelse-URL:en skickas, tolkas denna token automatiskt till personens unika bekräftelse-URL.
   >
   >Ange bekräftelsemeddelandet som **Operativ** för att säkerställa att personer som registrerar sig och kan avbeställa prenumerationen fortfarande får sin bekräftelseinformation.

* **Registreringslösenord** - (Valfritt) Stöds för närvarande inte med integreringen Marketo-Webex.
* **Godkännanderegler** - Stöds för närvarande inte med Marketo-Webex-integreringen. Men ni kan använda smarta kampanjer i Marketo för att styra godkännanden.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Presentatörer och paneler {#presenters-panelists}

Informationen som konfigureras i det här avsnittet skickas inte till Marketo.

### E-postmeddelanden {#email-messages}

Du kommer att använda Marketo för att skicka ut e-postmeddelanden till dina registranter, bekräftelsemeddelanden osv. Du behöver inte konfigurera något i det här avsnittet. Inaktivera (avmarkera) alternativen för e-postmeddelanden i Webex.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Integreringen av Marketo-Webex stöder inte sändning av bekräftelsemeddelanden från Webex. Bekräftelsen måste skickas via Marketo. När du har schemalagt evenemanget måste du kopiera händelseinformationen till bekräftelsemeddelandet från Marketo och ange e-postmeddelandet som **Operativ**.

Nu är vi redo att börja använda Marketo!

1. Markera händelsen som du skapade. Öppna **Händelseåtgärder** nedrullningsbar meny. Välj **Händelseinställningar.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Kanaltypen för den valda händelsen måste vara **webbinarium**.

1. Under **Evenemangspartner**, markera **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Under **Inloggning** väljer du din webbex-inloggning.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Under **Händelse** väljer du en nyligen skapad Webex-händelse. Välj sedan en valfri sida för säkerhetskopiering och klicka på **Spara**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Välj en valfri säkerhetskopieringssida för din Webex-händelse. Välj i listrutan över godkända Marketo-landningssidor eller ange webbadressen till en landningssida som inte är Marketo.

   >[!TIP]
   >
   >Ange en säkerhetskopieringssida för att dirigera en medlem till en viss sida om de klickar på deras anpassade händelse-URL före händelsens starttid.

   >[!NOTE]
   >
   >De fält som Marketo skickar är: Förnamn, efternamn, e-postadress.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge väljer du **Uppdatera från webbseminarieleverantör** på menyn Händelseåtgärder i **Sammanfattning** -fliken för din aktivitet.

Söt! Ditt Webex-event synkroniseras nu med ditt Marketo-event. Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget Ändra programstatus när Ny status är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att du följer flödessteget Ändra programstatus 1 och Skicka e-postflöde 2.

## Visa schemat  {#viewing-the-schedule}

Klicka på kalenderposten för aktiviteten i programschemavyn. Schemat visas till höger på skärmen.

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Om du vill ändra ditt evenemangsschema måste du redigera webbinariet på Webex.
