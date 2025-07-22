---
unique-page-id: 2949863
description: Skapa en händelse med  [!DNL Webex] - Marketo Docs - produktdokumentation
title: Skapa en händelse med  [!DNL Webex]
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Skapa en händelse med [!DNL Webex] {#create-an-event-with-webex}

När du har skapat ett webbinarium i Webex måste du synkronisera ditt event med Marketo Engage.

>[!PREREQUISITES]
>
>* [Lägg till [!DNL Webex] som en [!DNL LaunchPoint] tjänst](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Ange lämpliga [flödesåtgärder](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) för att spåra engagemang

## Schemalägg ditt webbinarium {#schedule-your-webinar}

Du schemalägger din aktivitet och väljer önskade inställningar i [Webex](https://www.webex.com/){target="_blank"}. Endast följande information kan visas i Marketo: namn på webbinarium, start-/slutdatum och -tid, tidszon och beskrivning. Mer information om webbinarier [finns här](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Grundläggande information {#basic-information}

* **[!UICONTROL Event Name]-** Det här namnet kan visas i Marketo.
* **[!UICONTROL Unlisted Checkbox]**
* **Ämne**: Det här är ditt händelsenamn och kan visas i Marketo.
* **Datum och tid**: Start-/slutdatum, start-/sluttid, varaktighet och tidszon kan visas i Marketo.
* **Maximalt antal deltagare**: Det maximala antalet deltagare avgör vilka Webex-funktioner som stöds.
* **Webbsändningsvy för deltagare**: Markera detta om du vill att ditt webbinarium ska direktuppspelas till alla deltagare.
* **Panellistor**: Bjud in specifika personer att bli panelister i ditt webbinarium.
* **Dagordning för webbinarium**: Fyll i detta om du vill ange kontext i den e-postinbjudan som skickas till panellistor.

### Säkerhet {#security}

![](assets/create-an-event-with-webex-2.png)

* **Webbinarlösenord**: (valfritt) Om du använder det här fältet måste du ta med det i bekräftelsemeddelandet.
* **Lösenord för panellista**: (valfritt) Om du använder det här fältet måste du ta med det på din webbseminariedagordning.
* **Kräv konto**: Begränsar deltagare till endast de som har Webex-konton.

### Alternativ för ljudanslutning {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Ljudanslutningstyp**: Välj hur deltagare i webbinariet ska ansluta till ljuddelen i webbinariet.
* **Ton för in- och avslutning**: Välj det ljud du vill att användare ska använda när någon går in i eller ut ur webbinariet (telefonljudanslutning krävs).
* **Panellistan Ljud av**: Välj önskade inställningar för tyst i panelistan.

### Avancerade alternativ {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Automatisk inspelning**: Markera detta om du vill att webbinariet ska spelas in automatiskt.
* **Practice session**: Markera detta om du vill att en övningssession ska startas när webbinariet börjar.
* **Brytningssessioner**: Med brytningssessioner kan du förtilldela paneler och deltagare innan webbinariet startar, eller tillåta dem att ansluta under webbinariet.
* **Webinar-serie**: Om du lägger till i en webbinarieserie kan andra se ditt webbinarium oavsett om det är offentligt eller inte.
* **Registrering**: Kräver att deltagarna registrerar sig och får värdgodkännande innan de går med.
* **Påminnelse via e-post**: Välj en påminnelse via e-post från 15 minuter innan webbinariet startar upp till två dagar.
* **Alternativ för webbinarium**: Avgör vilka funktioner som är tillgängliga för deltagare i webbinariet.
* **Deltagarbehörigheter**: Deltagarbehörigheter avgör vilka åtgärder som är tillgängliga för webbinära deltagare.

>[!NOTE]
>
>Integreringen av Marketo-Webex stöder inte sändning av bekräftelsemeddelanden från Webex. Bekräftelsen måste skickas via Marketo. När du har schemalagt evenemanget måste du kopiera händelseinformationen till bekräftelsemeddelandet från Marketo och ange e-postmeddelandet som _Användbart_.

## Synkronisera ditt evenemang med Marketo Engage {#sync-your-event-with-marketo-engage}

1. I Marketo söker du efter och väljer önskat Event Program. Välj **Händelseinställningar** i listrutan **Händelseåtgärder**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Kanaltypen för den valda händelsen måste vara **webbinarium**.

1. I listrutan **Event Partner** väljer du **Webbseminarier**.

   ![](assets/create-an-event-with-webex-6.png)

1. I listrutan **Inloggning** väljer du din Webex-inloggning.

   ![](assets/create-an-event-with-webex-7.png)

1. I listrutan **Händelse** väljer du din Webex-händelse.

   ![](assets/create-an-event-with-webex-8.png)

1. Din webbseminarieinformation fylls i. Klicka på **Spara**.

   ![](assets/create-an-event-with-webex-9.png)

Ditt Webex-event har nu synkroniserats med ditt Marketo Event Program. Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget _Ändra programstatus_ när den nya statusen är &quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se till att flödessteg 1 för _Ändra programstatus_ och flödessteg 2 för _Skicka e-post_.

## Saker att notera {#things-to-note}

* Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd ert Event Program Smart Campaign i stället.

* Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge klickar du på **Uppdatera från webbinariet Provider** i listrutan **Händelseåtgärder** på fliken **Sammanfattning** i ditt Event-program.
