---
unique-page-id: 12983619
description: Lägg till Slack som en LaunchPoint-tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Slack som en LaunchPoint-tjänst
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Lägg till Slack som en LaunchPoint-tjänst {#add-slack-as-a-launchpoint-service}

Det finns två meddelandetyper i integreringen med Slack:

* **Systemmeddelanden**: Få Slack-meddelanden om viktiga händelser i Marketo-instansen, som aviseringar om aktuella kampanjstatus och eventuella problem som kräver omedelbar åtgärd (CRM-fel och API-gränser).
* **Intressanta stunder**: När en Marketo Insight har utlösts av en känd person från ett försäljningskonto kan ledande ägare meddelas via Slack. Meddelanden innehåller information om lead samt detaljer om försäljningskontot.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du inte har Slack systemmeddelanden aktiverat kan du [kontakta support](http://docs.marketo.com/cdn-cgi/l/email-protection#1d6e686d6d726f695d707c6f76786972337e7270).

1. Gå till **LaunchPoint** och klicka sedan på **Ny tjänst** under **Ny** tjänst.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Ange ett visningsnamn för integreringen med Slack. I listrutan **Tjänst** väljer du **Slack**. Klicka på **Skapa**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Klicka på **Auktorisera**. Då öppnas Slack på en ny flik, där du fyller i behörigheten och ger Marketo tillstånd att hämta information från Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Ange arbetsytans URL-adress på fliken Slack och klicka på **Fortsätt**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Ange dina inloggningsuppgifter för Slack och klicka på **Logga in**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. I listrutan **Skicka till** väljer du den kanal där du vill att meddelanden från Marknad ska bokföras. Granska de begärda behörigheterna och klicka sedan på **Auktorisera**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Bekräftelseskärmen visas nedan. Fliken stängs automatiskt.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Uppdatera fliken Marketo och bekräfta att Slack nu visas som en aktiv tjänst i LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Meddelanden börjar nu att publicera i den kanal du valde i steg 6. De kommer att se ut ungefär så här:

   ![](assets/samplenotification.png)

