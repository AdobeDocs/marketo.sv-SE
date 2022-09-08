---
unique-page-id: 10096679
description: Exempel på händelseintegrering ON24 - Marketo Docs - produktdokumentation
title: Exempel på händelseintegrering ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Exempel på händelseintegrering ON24 {#example-on-event-integration}

>[!IMPORTANT]
>
>Från och med augusti 2022 har ON24 inte längre stöd för nya Marketo-integreringar. Informationen i den här artikeln gäller endast befintliga användare.

Här är ett exempel på en händelse, inklusive kampanjer, för ett ON24-webbinarium. När du skapar en händelse måste du testa kampanjerna innan du kör dem.

## Skapa en ny händelse i marknadsföringsaktiviteter {#create-a-new-event-in-marketing-activities}

1. Välj **Nytt** > **Nytt program**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Välj en **Campaign-mapp** var evenemanget kommer att bo.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Ange **Namn** för händelsen.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Välj **Händelse** som **Programtyp**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Välj **Webbinarium** som **Kanal** för händelsen.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicka **Skapa**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Bjud in (gruppkampanj)  {#invite-batch-campaign}

* **Smart List** - Ange vem du vill bjuda in till händelsen.
* **Flöde**

   * Skicka e-post - Om det här är en lokal resurspost får den följande namnkonvention: EventName.EmailName. Du kan också använda globala e-postmeddelanden.
   * Ändra status i progression - Ange som webbinarium > Inbjuden.

* **Schema** - Ange datumet för den inbjudan som ska skickas.

## Registrering/bekräftelse (utlösarkampanj) {#registration-confirmation-trigger-campaign}

* **Smart List**

   * Utlös kampanjen baserat på **Fyller i formulär**. Se till att du inkluderar landningssidan som formuläret använder **Lägg till begränsning**, särskilt om formuläret används på flera landningssidor.

>[!CAUTION]
>
>Du måste använda ett Marketo-formulär för att registrera personer för händelsen, eller ett icke-Marketo-formulär med rätt API-integrering för att skicka registreringsdata till Marketo. Detta är viktigt för att integreringen av din Event Partner ska lyckas. **ANMÄRKNING**: Om du använder ett Marketo-formulär på en landningssida som inte kommer från Marketo kommer utlösaren att vara **Fyller i formulär** med formulärnamnet.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flöde**

   * **Ändra status i progression** - Ange som webbinarium > Registrerad. **FÖRSIKTIGHET**: Det här flödessteget krävs när du konfigurerar din underordnade kampanj. När en persons progressionsstatus ändras till **Registrerad**, skickar Marketo registreringsinformationen till ON24.

   * **Skicka e-post** - Bekräftelsemeddelande (ange som **Operativ** så att de som har registrerat sig fortfarande får prenumerationen).

![](assets/image2015-12-22-15-3a52-3a9.png)

**ANMÄRKNING**: Om personen returneras med ett registreringsfel får han/hon inte någon e-postbekräftelse.

## Påminnelse (gruppkampanj) {#reminder-batch-campaign}

* **Smart List** - Filtrera med **Medlem i programmet** och ange status till **Registrerad**.

* **Flöde** - Skicka e-post (påminnelsee-post).

**ANMÄRKNING**: Du kan använda en liknande kampanj för att skicka en *olika* uppföljningsmejl till personer som blivit inbjudna men som inte har registrerat sig än.

## Uppföljningskampanj (batch- eller utlösarkampanj) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Utlös baserat på förändringar i programstatus.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flöde** - Skicka e-post. Använd alternativ för att skicka olika e-postmeddelanden baserat på programstatus.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
