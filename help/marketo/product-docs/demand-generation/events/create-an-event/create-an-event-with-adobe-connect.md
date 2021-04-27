---
unique-page-id: 2949865
description: Skapa ett evenemang med Adobe Connect - Marketo Docs - produktdokumentation
title: Skapa ett evenemang med Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Skapa en händelse med Adobe Connect {#create-an-event-with-adobe-connect}

Synkronisering med Adobe Connect gör att ni kan hantera registrering och närvaro i ert webbinarium i Marketo, vilket säkerställer att engagemanget inte spåras.

>[!PREREQUISITES]
>
>* [Länka Adobe Connect och Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Skapa ett nytt händelseprogram](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


Kontrollera först att du har skapat ett möte eller seminarium i Adobe Connect. Om du behöver hjälp kan du läsa [Adobe Connect användarhandbok](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Möten och seminarier som du skapar i Adobe Connect måste skapas i den mapp som du angav när du angav dina inloggningsuppgifter i Marketo. När du har skapat ditt möte eller seminarium bör du notera all relevant logistisk information (till exempel telefonnumret) som du kan använda i bekräftelsemeddelandet och ICS-filen.

>[!CAUTION]
>
>Som händelsevärd måste du se till att ansluta inifrån programmet och **inte** via länken som skickas till deltagarna.

>[!NOTE]
>
>Vi stöder för närvarande inte Adobe Connect On-Site.

1. Välj **Händelseåtgärder** i startdelen av en ny händelse och **Händelseinställningar**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Om du inte ser **Händelseinställningar** i listrutan kontrollerar du att händelsens kanal har **Händelse med webbinariet** markerat under &quot;Gäller för&quot;.

1. Under **Event Partner** väljer du **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Välj ditt **inloggnings-ID** och välj din **Event**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Klicka på **Spara**.

   ![](assets/event-settings-overview.png)

   Snyggt! Ditt Adobe Connect-event har nu synkroniserats med ditt Marketo-event.

   >[!NOTE]
   >
   >De fält som Marketo skickar är: Förnamn, efternamn, e-postadress.

   >[!TIP]
   >
   >Om du vill infoga personens unika URL-adress i ett e-postmeddelande använder du den här variabeln: `{{member.webinar url}}`. När e-postmeddelandet skickas löser denna token automatiskt personens unika bekräftelse-URL från Adobe Connect.
   >
   >Ange din bekräftelse via e-post till **Operational** för att säkerställa att personer som registrerar sig och kan avbeställa prenumerationen fortfarande får sin bekräftelseinformation.

   Personer som registrerar sig för ditt webbinarium kommer att pushas till din webbinarileverantör via flödessteget Ändra programstatus när Ny status är inställd på&quot;Registrerad&quot;. Ingen annan status kommer att föra personen över. Se även till att du följer flödessteget Ändra programstatus 1 och Skicka e-postflöde 2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Undvik att använda kapslade e-postprogram för att skicka ut bekräftelsemeddelanden. Använd händelseprogrammets smarta kampanj i stället, som visas ovan.

   >[!TIP]
   >
   >Det kan ta upp till 48 timmar innan data visas i Marketo. Om du inte ser något efter att ha väntat så länge väljer du **Uppdatera från webbinariet Provider** på menyn Händelseåtgärder på fliken Sammanfattning för händelsen.

   >[!MORELIKETHIS]
   >
   >* [Lägg till Adobe Connect som en LaunchPoint-tjänst](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Redigera en händelsekanal](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

