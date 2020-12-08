---
unique-page-id: 14352476
description: SFDC (Activity Type Field on Task) - Marketo Docs - Produktdokumentation
title: SFDC (Activity Type Field on Task)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# SFDC (Activity Type Field on Task) {#activity-type-field-on-tasks-sfdc}

Med hjälp av Sales Connect kan du logga dina e-postmeddelanden och samtal som en aktivitet i Salesforce. En viktig del av att ha värdefulla data i Salesforce är att låta typfältet fylla i rätt värde.

>[!NOTE]
>
>Loggning av e-postmeddelanden via BCC kommer inte att användas i listan Uppgiftstyp, utan fyller i textfältet automatiskt som e-post eftersom de levereras till Salesforce via din BCC-adress.

## Krav {#requirements}

* Anslutning till Salesforce
* Inget standardtypvärde har valts i listrutan Aktivitetstyp
* Samtal, svar och e-post måste alla finnas i listrutan Aktivitetstyp (skiftlägesfrågor)
* Ingen `Workflows` eller `Triggers` åtgärd för typfältets värde

## Inställningar {#setup}

Kontrollera först att du har rätt plocklistevärden på plats. Du behöver hjälp av din Salesforce-administratör för att göra ändringar i din lista.

1. Navigera till [Salesforce.com](http://Salesforce.com) och klicka på Inställningar i det övre högra hörnet.
1. Klicka på Anpassa.
1. Klicka på Aktiviteter.
1. Klicka på Aktivitetsfält.
1. Klicka på Text.
1. Du finns nu i listan över uppgiftstyper. Kontrollera att du inte har valt &#39;Standard&#39;.
1. Kontrollera att det finns ett typvärde för E-post, Ring och Svara.

Nu när detta är på plats börjar du se textfältet fylla i motsvarande värde för loggade e-postmeddelanden, samtal och svar. Dessa värden fylls **inte** i för påminnelseaktiviteter för Sales Connect.

>[!NOTE]
>
>Om du inte ser Svara som ett värde lägger du till det genom att klicka på **Nytt**. Svara är inte ett standardvärde i Salesforce.
