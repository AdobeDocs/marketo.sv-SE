---
unique-page-id: 17728023
description: Skapa en händelse med  [!DNL Zoom] - Marketo Docs - produktdokumentation
title: Skapa en händelse med  [!DNL Zoom]
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Skapa en händelse med [!DNL Zoom] {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Lägg till [!DNL Zoom] som en [!DNL LaunchPoint] tjänst](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Ange lämpliga [flödesåtgärder](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) för att spåra engagemang

Skapa först ditt webbinarium i [!DNL Zoom]. Vissa inställningar när du skapar [!DNL Zoom] används av Marketo och vissa används bara av [!DNL Zoom].

När du har skapat en Marketo-händelse och associerat ett [!DNL Zoom]-webbinarium med det kan systemen dela registrerings- och närvaroinformation. Hjälp med att skapa ett webbinarium finns i [Komma igång med [!DNL Zoom] webbinarier](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Ange följande information för ditt webbinarium så hämtas det till Marketo via adaptern. Om du ändrar något i den här informationen måste du klicka på länken&quot;Uppdatera från webbinarium-leverantör&quot; under Händelseåtgärder för att Marketo ska kunna se ändringarna.

**Titel och beskrivning**

* **Namn på webbinarium** - Ange namnet på webbinariet. Namnet kan visas i Marketo.

* **Beskrivning** (valfritt) - Ange beskrivningen för webbinariet. Beskrivningen kan visas i Marketo.

**Datum och tid**

* **Startdatum** - Ange ditt startdatum. Detta kommer att kunna visas i Marketo.

* **Starttid** - Ange starttid. Detta kommer att kunna visas i Marketo.

* **Varaktighet** - Ange längden. Starttiden och sluttiden visas i Marketo.

* **Tidszon** - Välj tillämplig tidszon. Detta kommer att kunna visas i Marketo.

* **Återkommande webbinarium**- Behåll avmarkerat.

* **Registrering** - Markera den här kryssrutan om du vill göra registreringen obligatorisk. Du använder ett Marketo-formulär/en landningssida för att samla in registreringsinformation som skickas till [!DNL Zoom].

>[!NOTE]
>
>Marketo stöder för närvarande inte återkommande webbinarier. Du måste konfigurera en session mellan varje Marketo Event och [!DNL Zoom] webbinarium.

![](assets/overview2.png)

>[!TIP]
>
>Det finns ytterligare fält som du konfigurerar i [!DNL Zoom] som INTE kommer att påverka integreringen. Mer information om dessa fält finns i [[!DNL Zoom] hjälpcentret för webbinariet](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar).

Nu ska vi hoppa in i Marketo!

1. Välj en händelse. Klicka på **[!UICONTROL Event Actions]** och välj **[!UICONTROL Event Settings]**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Kanaltypen för den valda händelsen måste vara **webbinarium**.

1. Välj **[!UICONTROL Zoom]** i listan **[!UICONTROL Event Partner]**.

   ![](assets/eventsettings1.png)

1. Välj det [!DNL Zoom]-konto som du vill associera aktiviteten med.

   ![](assets/selectaccount.png)

1. Välj webbinariet.

   ![](assets/selectevent.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/eventsettingssave.png)

   Underbar! Händelsen har synkroniserats och schemalagts av [!DNL Zoom].

   >[!NOTE]
   >
   >De fält som Marketo skickar är: Förnamn, Efternamn, E-postadress.

   >[!TIP]
   >
   >Om du vill fylla i bekräftelsemeddelandet med den här unika URL:en använder du följande token i e-postmeddelandet: `{{member.webinar url}}`. När bekräftelse-URL:en skickas, tolkas denna token automatiskt till personens unika bekräftelse-URL.
   >
   >Ange bekräftelsemeddelandet som **Operational** för att säkerställa att personer som registrerar sig och kan avbeställa prenumerationen fortfarande får sin bekräftelseinformation.

   Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget **[!UICONTROL Change Program Status]** när [!UICONTROL New Status] är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att flödesteget **[!UICONTROL Change Program Status]** och **[!UICONTROL Send Email]** flödessteg 2 anges.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge väljer du **Uppdatera från webbinariet Provider** på menyn Händelseåtgärder på fliken **Sammanfattning** i händelsen och klickar sedan på ikonen Uppdatera längst ned till höger på skärmen.
