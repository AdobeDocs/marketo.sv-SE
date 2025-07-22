---
unique-page-id: 2949874
description: Skapa en händelse med  [!DNL GotoWebinar] - Marketo Docs - produktdokumentation
title: Skapa en händelse med  [!DNL GotoWebinar]
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Skapa en händelse med [!DNL GotoWebinar] {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Lägg till [!DNL GoToWebinar] som en [!DNL LaunchPoint] tjänst](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Ange lämpliga [flödesåtgärder](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) för att spåra engagemang

Skapa först ditt webbinarium i [!DNL GoToWebinar]. Vissa inställningar när du skapar [!DNL GoToWebinar] används av Marketo och vissa används bara av [!DNL GoToWebinar].

När du har skapat en Marketo-händelse och associerat [!DNL GoToWebinar] med den kan systemen dela registrerings- och närvaroinformation.

Nedan finns en lista över de inställningar som används av Marketo.

## Titel och beskrivning {#title-and-description}

**[!UICONTROL Title]** - ange namnet på webbinariet. Namnet kan visas i Marketo.

**[!UICONTROL Description]** (valfritt) - ange beskrivningen för webbinariet. Beskrivningen kan visas i Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Datum och tid {#date-time}

Ange följande information för ditt webbinarium så hämtas det till Marketo via adaptern. Om du ändrar den här informationen måste du klicka på länken **[!UICONTROL Refresh from Webinar Provider]** under **[!UICONTROL Event Actions]** för att Marketo ska kunna se ändringarna.

**[!UICONTROL Start Date]** - Ange ditt startdatum. Detta kommer att kunna visas i Marketo.

**[!UICONTROL Start Time]** - ange din starttid. Detta kommer att kunna visas i Marketo.

**[!UICONTROL End Time]** - ange sluttid. Detta kommer att kunna visas i Marketo.

**[!UICONTROL Webinar Time Zone]** - välj tillämplig tidszon. Den kan visas i Marketo.

**[!UICONTROL Type]** - inställt på **[!UICONTROL One Session]**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo stöder för närvarande inte återkommande webbinarier. Du måste konfigurera en session mellan varje Marketo Event och [!DNL GoToWebinar] webbinarium.

>[!TIP]
>
>Om du behöver ytterligare [!DNL GoToWebinar] hjälp kan du besöka deras [hjälpwebbplats](https://support.logmeininc.com/gotowebinar).

Nu ska vi hoppa in i Marketo!

1. Välj en händelse. Klicka på **[!UICONTROL Event Actions]** och välj **[!UICONTROL Event Settings]**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Kanaltypen för den valda händelsen måste vara **webbinarium**.

1. Välj **[!UICONTROL GoToWebinar]** i listan **[!UICONTROL Event Partner]**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Välj konto.

   ![](assets/rtaimage-2.png)

1. Välj webbinariet.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Underbar! Händelsen har synkroniserats och schemalagts av **[!DNL GoToWebinar]**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >De fält som Marketo skickar är: Förnamn, Efternamn, E-postadress. Dessa fält är obligatoriska och får inte vara tomma.

   >[!TIP]
   >
   >Om du vill fylla i bekräftelsemeddelandet med den här unika URL:en använder du följande token i e-postmeddelandet: `{{member.webinar url}}`. När bekräftelse-URL:en skickas, tolkas denna token automatiskt till personens unika bekräftelse-URL.
   >
   >Ange bekräftelsemeddelandet som **Operational** för att säkerställa att personer som registrerar sig och kan avbeställa prenumerationen fortfarande får sin bekräftelseinformation.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge väljer du **[!UICONTROL Refresh from Webinar Provider]** på [!UICONTROL Event Actions]-menyn på fliken **[!UICONTROL Summary]** för aktiviteten.

Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget [!UICONTROL Change Program Status] när [!UICONTROL New Status] är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att flödesteget [!UICONTROL Change Program Status] och [!UICONTROL Send Email] flödessteg 2 anges.

## Visa schemat  {#viewing-the-schedule}

Klicka på kalenderposten för aktiviteten i programschemavyn. Schemat visas till höger på skärmen.

>[!NOTE]
>
>Om du vill ändra ditt evenemangsschema måste du redigera webbinariet på [!DNL GoToWebinar].

![](assets/image2015-5-14-15-3a3-3a13.png)
