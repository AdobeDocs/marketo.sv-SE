---
unique-page-id: 14745982
description: Lägg till Workplace av Facebook som en LaunchPoint-tjänst - Marketo Docs - produktdokumentation
title: Lägg till Workplace av Facebook som en LaunchPoint-tjänst
exl-id: afcc1eca-8927-4a25-af9b-c18cef24b0ae
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Lägg till arbetsyta av Facebook som en LaunchPoint-tjänst {#add-workplace-by-facebook-as-a-launchpoint-service}

Det finns två meddelandetyper i Workplace-integreringen:

* **Systemmeddelanden**: Få Workplace-meddelanden om viktiga händelser i din Marketo-instans, som aviseringar om aktuella kampanjstatus och eventuella problem som kräver omedelbar åtgärd (CRM-fel och API-gränser).
* **Intressanta stunder**: När en Marketo Insight har utlösts av en känd person från ett försäljningskonto kan leadägare meddelas via Workplace. Meddelanden innehåller information om lead samt detaljer om försäljningskontot.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!PREREQUISITES]
>
>Om du inte har Workplace Notifications aktiverat kan du kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Gå till **LaunchPoint** och klicka sedan på **Ny tjänst** under **Nytt**.

   ![](assets/image2017-11-27-14-3a13-3a18-1.png)

1. Ange ett visningsnamn för integreringen av arbetsytan. I listrutan **Tjänst** väljer du **Arbetsplats av Facebook**. Klicka på **Skapa**.

   ![](assets/newservice.png)

1. Om du vill få systemmeddelanden och intressanta stunder låter du alternativen vara som de är. Klicka på **Skapa**.

   ![](assets/create.png)

1. Klicka på **Auktorisera**. Då öppnas Workplace på en ny flik, där du slutför behörigheten och ger Marketo behörighet att hämta information från Workplace.

   ![](assets/authorize.png)

1. På den nya fliken Workplace anger du ditt företags-e-postadress eller Workplace-användarnamn och klickar på **Fortsätt**.

   ![](assets/workplacelogin.png)

1. Ange dina uppgifter för arbetsytan och klicka på **Logga in**.

   ![](assets/workplacelogininfo.png)

1. I popup-fönstret Workplace väljer du en Facebook-grupp där du vill att meddelanden från Marketo ska publiceras (t.ex. partnerintegreringar). Klicka på **Installera**.

   ![](assets/installmarketo.png)

1. Bekräftelsemeddelandet visas nedan. Fliken stängs automatiskt.

   ![](assets/success.png)

1. Uppdatera fliken Marketo och bekräfta att Workplace nu visas som en aktiv tjänst i LaunchPoint.

   ![](assets/confirm.png)

   Meddelanden kommer nu att börja bokföras i den Facebook-grupp du valde i steg 7. De kommer att se ut ungefär så här:

   ![](assets/example.png)
