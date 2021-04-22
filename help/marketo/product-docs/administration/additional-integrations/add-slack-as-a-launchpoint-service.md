---
unique-page-id: 12983619
description: Lägg till Slack som en LaunchPoint-tjänst - Marketo Docs - Produktdokumentation
title: Lägg till Slack som en LaunchPoint-tjänst
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Lägg till Slack som en LaunchPoint-tjänst {#add-slack-as-a-launchpoint-service}

Det finns två meddelandetyper i integreringen med Slack:

* **Systemmeddelanden**: Få Slack-meddelanden om viktiga händelser i din Marketo-instans, som aviseringar om aktuella kampanjstatus och eventuella problem som kräver omedelbar åtgärd (CRM-fel och API-begränsningar).
* **Intressanta stunder**: När en Marketo Insight har utlösts av en känd person från ett försäljningskonto kan ledande ägare meddelas via Slack. Meddelanden innehåller information om lead samt detaljer om försäljningskontot.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du inte har Slack systemmeddelanden aktiverat kan du kontakta [Marketo support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Gå till **LaunchPoint** och klicka sedan på **Ny tjänst** under **Nytt**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Ange ett visningsnamn för integreringen med Slack. I listrutan **Service** väljer du **Slack**. Klicka på **Skapa**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Klicka på **Auktorisera**. Då öppnas Slack på en ny flik, där du fyller i behörigheten och ger Marketo tillstånd att hämta information från Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Ange arbetsytans URL-adress på den nya fliken Slack och klicka på **Fortsätt**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Ange dina inloggningsuppgifter för Slack och klicka på **Logga in**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. I listrutan **Skicka till** väljer du den kanal där du vill att meddelanden från Marketo ska skickas. Granska de begärda behörigheterna och klicka sedan på **Auktorisera**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Bekräftelseskärmen visas nedan. Fliken stängs automatiskt.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Uppdatera fliken Marketo och bekräfta att Slack nu visas som en aktiv tjänst i LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Meddelanden börjar nu att publicera i den kanal du valde i steg 6. De kommer att se ut ungefär så här:

   ![](assets/samplenotification.png)
