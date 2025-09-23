---
unique-page-id: 10096679
description: Exempel på händelseintegrering ON24 - Marketo Docs - produktdokumentation
title: Exempel på händelseintegrering ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Exempel på händelseintegrering ON24 {#example-on-event-integration}

Här är ett exempel på en händelse, inklusive kampanjer, för ett ON24-webbinarium. När du skapar en händelse måste du testa kampanjerna innan du kör dem.

## Skapa en ny händelse i marknadsföringsaktiviteter {#create-a-new-event-in-marketing-activities}

1. Välj **[!UICONTROL New]** > **[!UICONTROL New Program]**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Välj en **[!UICONTROL Campaign Folder]** där händelsen ska finnas.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Ange en **[!UICONTROL Name]** för händelsen.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Välj **[!UICONTROL Event]** som **[!UICONTROL Program Type]**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Välj **[!UICONTROL Webinar]** som **[!UICONTROL Channel]** för händelsen.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Bjud in (gruppkampanj)  {#invite-batch-campaign}

* **Smart lista** - Ange vem du vill bjuda in till händelsen.
* **Flöde**

   * Skicka e-post - Om det här är en lokal resurspost får den följande namnkonvention: EventName.EmailName. Du kan också använda globala e-postmeddelanden.
   * Ändra status i progression - Ange som webbinarium > Inbjuden.

* **Schema** - Ange datumet för den inbjudan som ska skickas.

## Registrering/bekräftelse (utlösarkampanj) {#registration-confirmation-trigger-campaign}

* **Smart lista**

   * Utlös kampanjen baserat på **[!UICONTROL Fills Out Form]**. Se till att du inkluderar landningssidan som formuläret använder med hjälp av **[!UICONTROL Add Constraint]**, särskilt om formuläret används på flera landningssidor.

>[!CAUTION]
>
>Du måste använda ett Marketo-formulär för att registrera personer för händelsen, eller ett icke-Marketo-formulär med rätt API-integrering för att skicka registreringsdata till Marketo. Detta är viktigt för att din [!UICONTROL Event Partner]-integrering ska lyckas. **Obs!** Om du använder ett Marketo-formulär på en landningssida som inte kommer från Marketo, kommer utlösaren att vara **[!UICONTROL Fills Out Form]** med [!UICONTROL Form Name].

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flöde**

   * **Ändra status i progression** - Ange som webbinarium > Registrerad. **VARNING**: Det här flödessteget krävs när du konfigurerar din underordnade kampanj. När en persons progressionsstatus ändras till **Registrerad**, skickar Marketo registreringsinformationen till ON24.

   * **Skicka e-post** - Bekräftelsemeddelande (inställt på **Funktion** så att personer som har registrerat sig fortfarande får det).

![](assets/image2015-12-22-15-3a52-3a9.png)

**Obs!** Om personen returneras med ett registreringsfel får han/hon ingen e-postbekräftelse.

## Påminnelse (gruppkampanj) {#reminder-batch-campaign}

* **Smart lista** - Filtrera med **Medlem i program** och ange status till **Registrerad**.

* **Flöde** - Skicka e-post (påminnelse-e-post).

**Obs!** Du kan använda en liknande kampanj för att skicka ett *annat* uppföljningsmeddelande till personer som har bjudits in men som inte har registrerat sig än.

## Uppföljningskampanj (batch- eller utlösarkampanj) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Utlös baserat på ändringar i programstatus.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flöde** - Skicka e-post. Använd alternativ för att skicka olika e-postmeddelanden baserat på programstatus.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Om Marketo ON24-nätverkskortshändelser](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
