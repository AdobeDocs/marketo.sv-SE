---
unique-page-id: 2949865
description: Skapa ett evenemang med Adobe Connect - Marketo Docs - produktdokumentation
title: Skapa ett evenemang med Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Skapa ett evenemang med Adobe Connect {#create-an-event-with-adobe-connect}

Synkronisering med Adobe Connect gör att ni kan hantera registrering och närvaro i ert webbinarium i Marketo, vilket säkerställer att engagemanget inte spåras.

>[!PREREQUISITES]
>
>* [Länka Adobe Connect och Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

Kontrollera först att du har skapat ett möte eller seminarium i Adobe Connect. Om du behöver hjälp kan du läsa [Adobe Connect användarhandbok](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Möten och seminarier som du skapar i Adobe Connect måste skapas i den mapp som du angav när du angav dina inloggningsuppgifter i Marketo. När du har skapat ditt möte eller seminarium bör du notera all relevant logistisk information (t.ex. telefonnumret) som du kan använda i bekräftelsemeddelandet och ICS-filen.

>[!CAUTION]
>
>Som händelsevärd måste du se till att ansluta inifrån appen och **inte** via länken som skickas till deltagarna.

>[!NOTE]
>
>Vi stöder för närvarande inte Adobe Connect On-Site.

1. Välj **[!UICONTROL Event Actions]** och sedan **[!UICONTROL Event Settings]** hemma för en ny händelse.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Om du inte ser **[!UICONTROL Event Settings]** i listrutan kontrollerar du att händelsens kanal har **[!UICONTROL Event with Webinar]** markerat under [!UICONTROL Applies to].

1. Välj **[!UICONTROL Event Partner]** under **[!UICONTROL Adobe Connect]**.

   ![](assets/event-settings-adobe-connect.png)

1. Välj ditt **[!UICONTROL Login]**-ID och välj din **[!UICONTROL Event]**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/event-settings-overview.png)

   Snyggt! Ditt Adobe Connect-event har nu synkroniserats med ditt Marketo-event.

   >[!NOTE]
   >
   >De fält som Marketo skickar är: Förnamn, Efternamn, E-postadress.

   >[!TIP]
   >
   >Om du vill infoga personens unika URL i ett e-postmeddelande använder du den här token: `{{member.webinar url}}`. När e-postmeddelandet skickas löser denna token automatiskt personens unika bekräftelse-URL från Adobe Connect.
   >
   >Ange bekräftelsemeddelandet som **Operational** för att säkerställa att personer som registrerar sig och kan avbeställa prenumerationen fortfarande får sin bekräftelseinformation.

   Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget [!UICONTROL Change Program Status] när [!UICONTROL New Status] är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att flödesteget [!UICONTROL Change Program Status] och [!UICONTROL Send Email] flödessteg 2 anges.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du fortfarande inte ser något efter att ha väntat så länge väljer du **[!UICONTROL Refresh from Webinar Provider]** på menyn Händelseåtgärder på fliken Sammanfattning för händelsen.

   >[!MORELIKETHIS]
   >
   >* [Lägg till Adobe Connect som en [!DNL LaunchPoint] tjänst](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Redigera en händelsekanal](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
