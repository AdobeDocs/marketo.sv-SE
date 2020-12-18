---
unique-page-id: 10096679
description: Exempel på ON24-händelseintegrering - Marketo Docs - produktdokumentation
title: Exempel på händelseintegrering ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Exempel på ON24-händelseintegrering {#example-on-event-integration}

Här är ett exempel på en händelse, inklusive kampanjer, för ett ON24-webbinarium. När du skapar en händelse måste du testa kampanjerna innan du kör dem.

## Skapa en ny händelse i marknadsföringsaktiviteter {#create-a-new-event-in-marketing-activities}

1. Välj **Nytt** > **Nytt program**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Välj en **kampanjmapp** där händelsen ska visas.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Ange ett **namn** för händelsen.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Välj **Event **som **programtyp**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Välj **Webinar **som **Channel **för händelsen.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicka på **Skapa**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Bjud in (gruppkampanj) {#invite-batch-campaign}

* **Smart lista**  - Ange vem du vill bjuda in till händelsen.
* **Flöde**

   * Skicka e-post - Om det här är en lokal resurspost får den följande namnkonvention: EventName.EmailName. Du kan också använda globala e-postmeddelanden.
   * Ändra status i progression - Ange som webbinarium > Inbjuden.

* **Schema**  - Ange datumet för den inbjudan som ska skickas.

## Registrering/bekräftelse (utlösarkampanj) {#registration-confirmation-trigger-campaign}

* **Smart List**

   * Utlös kampanjen baserat på **Fyller i formulär**. Se till att du inkluderar landningssidan som formuläret är aktivt på med **Lägg till begränsning**, särskilt om formuläret används på flera landningssidor.

>[!CAUTION]
>
>Du måste använda ett Marketo-formulär för att registrera personer för händelsen, eller ett icke-Marketo-formulär med rätt API-integrering för att skicka registreringsdata till Marketo. Detta är viktigt för att integreringen av din Event Partner ska lyckas. **OBS**: Om du använder ett Marketo-formulär på en icke-Marketo-landningssida kommer utlösaren att vara  **Fyll i** formulär med formulärnamnet.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flöde**

   * **Ändra status i progression**  - Ange som webbinarium > Registrerad. **VARNING**: Det här flödessteget krävs när du konfigurerar din underordnade kampanj. När en persons progressionsstatus ändras till **Registrerad**, skickar Marketo registreringsinformationen till ON24.

   * **Skicka e-post**  - Bekräftelsemeddelande (inställt på  **** Åtgärd, även att personer som har registrerat sig fortfarande får det).

![](assets/image2015-12-22-15-3a52-3a9.png)

**OBS**: Om personen returneras med ett registreringsfel får han/hon inte någon e-postbekräftelse.

## Påminnelse (gruppkampanj) {#reminder-batch-campaign}

* **Smart List** - Filtrera med  **Medlem i** program och ställ in statusen på  **Registrerad**.

* **Flow**  - Send Email (Reminder Email).

**OBS**: Du kan använda en liknande kampanj för att skicka ett  ** annat uppföljningsmeddelande via e-post till personer som var inbjudna men som inte har registrerat sig än.

## Uppföljningskampanj (batch- eller utlösarkampanj) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List**  - Utlösare baserad på förändringar i programstatus.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flöde**  - Skicka e-post. Använd alternativ för att skicka olika e-postmeddelanden baserat på programstatus.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [Om Marketo ON24-adapterhändelser](understanding-marketo-on24-adapter-events.md)

>



